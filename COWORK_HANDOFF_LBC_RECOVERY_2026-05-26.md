# Cowork Handoff — LBC Workspace Recovery — 2026-05-26

**For:** the next Claude Code (Cowork) session, opened locally in `/Volumes/FMNC 8_T_B/Lonely Brew Club/`
**From:** a Claude Code web session running against `dirtylogic/yoyo` (no filesystem access to LBC, only relaying through pasted Codex transcripts)
**Goal:** untangle the Codex shipping run from 2026-05-25 night, push the remaining product branches to `github.com/djpjronline-netizen/lbc`, fix repo bloat, and re-anchor everything to the LBC factory model.

---

## Read first

1. `CLAUDE.md` (workspace root) — operating contract, identity, voice, hard rules
2. `03_Portfolio/CLAUDE.md` — three-category factory model (SaaS, DevTool, SkillPack, PersonalInfra), pre-LLC pipeline, capital allocation
3. This file
4. The yoyo repo PR #1 at `github.com/dirtylogic/yoyo/pull/1` — contains the foundational market research doc + the previous session's handoff with the five verbatim Codex prompts

Then **diagnose before touching anything.** My summary below is based on relayed Codex transcripts, not direct observation. Verify.

---

## Diagnostic commands (run first, do not skip)

```bash
cd "/Volumes/FMNC 8_T_B/Lonely Brew Club"

# What worktrees exist?
git worktree list

# What branches exist locally and where do they point?
git branch -vv

# What's on each branch, in order?
git log --oneline --all --decorate -50

# What's the remote situation?
git remote -v

# What's uncommitted right now?
git status

# How big is the repo?
du -sh .git
```

Save the output. Read it. Then compare against the summary in the next section before deciding what to fix first.

---

## Last-known state (as relayed from Codex transcripts, 2026-05-25 evening)

### GitHub remote

- Origin: `https://github.com/djpjronline-netizen/lbc.git`
- Only `main` was pushed.
- **Push warning was real:** an 82.6MB `workerd` binary inside `products/mcp-server-builder-pro/node_modules/` got committed. GitHub accepted it but flagged it. Every future clone now drags this binary.

### Branch state on your Mac (likely)

| Branch | What's on it | On GitHub? | Notes |
|---|---|---|---|
| `main` | MCP Server Builder Pro (8 commits) + GEO Audit (5 commits). Lives in `lonely-brew-geo` worktree. | YES | Was renamed from `claude/geo-audit` via `git branch -M main` in that worktree. |
| `claude/mcp-server-builder-pro` | MCP Builder Pro template + landing + LS webhook fulfillment + ops. 8 commits. | NO | Base for everything that came after. |
| `claude/production-ai-bundle` | Production Bundle SKU + **the Security Audit's first commit `920613f` accidentally landed here**. | NO | Branch hygiene broken. See "Security Audit branch mix-up" below. |
| `claude/memory-rag-addons` | Memory Kit + RAG Regression Harness. | NO | |
| `claude/agent-security-audit` | **Empty.** Codex created it via `git checkout -b` but the first commit landed on `claude/production-ai-bundle` instead. Codex paused on detecting the mismatch. | NO | Safe to delete: `git branch -D claude/agent-security-audit`. |
| `claude/geo-audit` | Gone. Was renamed to `main` in the lonely-brew-geo worktree. | (as main) | |
| `claude/vendor-marketplace-kit` | Does not exist. Codex returned a 5-line plan but never executed it before the session ended. | NO | |

### Worktrees

- Main worktree: `/Volumes/FMNC 8_T_B/Lonely Brew Club` — was on `claude/memory-rag-addons` or similar at last observation; has substantial uncommitted state from the production-bundle and memory-rag work that didn't get staged before branch switches.
- Secondary worktree: `/Volumes/FMNC 8_T_B/lonely-brew-geo` — holds `main` checked out. This is why `git branch -M main` from the main worktree was rejected.
- There may be additional worktrees. Run `git worktree list` to confirm.

### Codex-related ambient noise

- `~/.codex/plugins/cache/openai-curated/twilio-developer-kit/.../twilio-enterprise-knowledge/SKILL.md` has a description longer than 1024 characters. Cosmetic warning. Either patch the SKILL.md description or live with the warning.
- PostToolUse hook is invoking `scripts/post_write_codex_agent_guardrail.py` which doesn't exist. Spammy but non-blocking. Either create the script or remove the hook from `.codex/config.toml`.
- Several MCP servers failed to start: context-pack, mcp-search, MCP_DOCKER, atlassian (not logged in), github (needs PAT). Not blocking shipping; fix when you have time.
- SessionStart hook had a stale claude-mem context dump (172k tokens of memories about `lbc-platform` directory from a different earlier session — that directory is unrelated to this work). The claude-mem Claude Desktop OAuth token is expired. Re-login via Claude Desktop to refresh if you want fresh observations.

---

## Issue punch list (priority order)

### P0 — Repo bloat must be fixed before more merges

The 82.6MB `workerd` binary in `main`'s history will balloon every clone and PR review. Fix it before opening any PRs:

```bash
# Verify the bloat
git rev-list --objects --all | git cat-file --batch-check='%(objecttype) %(objectsize) %(rest)' | sort -k2 -n -r | head -20

# Install git-filter-repo if needed
pip install git-filter-repo

# Make sure top-level .gitignore covers node_modules
echo "node_modules/" >> .gitignore
echo ".wrangler/" >> .gitignore
git add .gitignore && git commit -m "chore: ignore node_modules and .wrangler" || true

# Backup first
git tag pre-filter-backup
git branch backup-pre-filter

# Remove all node_modules from all history
git filter-repo --path-glob '**/node_modules/**' --invert-paths --force

# Force-push the cleaned main
git push --force origin main
```

If `main` is checked out in the `lonely-brew-geo` worktree, you'll need to either remove that worktree first (`git worktree remove ../lonely-brew-geo`) or run the filter-repo against a fresh clone. Filter-repo against worktree-locked branches is fragile.

### P1 — Push the unpushed feature branches

Each product gets its own remote branch + PR. Easier review, isolated rollback, factory-spec discipline:

```bash
git push -u origin claude/mcp-server-builder-pro
git push -u origin claude/production-ai-bundle
git push -u origin claude/memory-rag-addons
# do NOT push claude/agent-security-audit — it's empty
```

Then open four PRs against `main`:
- MCP Server Builder Pro
- Production AI Shipping Bundle
- Memory + RAG add-ons
- (Security Audit — see next item)

### P2 — Resolve the Security Audit branch mix-up

`920613f feat(site): add security audit intake landing and intake API` is sitting on `claude/production-ai-bundle` instead of its own branch. Two options:

**Option A (clean, recommended):** redo the Security Audit fresh.
1. Reset `production-ai-bundle` to drop the stray commit:
   ```bash
   git checkout claude/production-ai-bundle
   git rebase --onto 920613f^ 920613f
   git push --force-with-lease origin claude/production-ai-bundle
   ```
2. Delete the empty agent-security-audit branch:
   ```bash
   git branch -D claude/agent-security-audit
   ```
3. Re-run the Security Audit Codex prompt (preserved verbatim in yoyo's `SESSION_HANDOFF_2026-05-26.md` appendix A2). Codex only got the first section in (intake page) before the branch mismatch — running it fresh gives you all five sections (A-E) on the right branch.

**Option B (lazy):** rename `claude/production-ai-bundle` to `claude/bundle-and-security` and let the PR be a mixed feature. Reviewable but ugly. Don't do this unless time is short.

### P3 — Vendor Marketplace Kit not yet built

Codex returned a 5-line plan and stopped. The Counsel-clean Vendor Marketplace Kit prompt is preserved verbatim in yoyo's `SESSION_HANDOFF_2026-05-26.md` appendix A6. Run it when you decide whether vendor-kit belongs in the factory at all (see P5).

### P4 — Worktree cleanup

You likely have two active worktrees plus dirty state in the main worktree. After all branches are pushed, consider:

```bash
# Drop the GEO worktree (its work is now on main)
git worktree remove "../lonely-brew-geo"

# Stash anything in the main worktree you haven't committed
git stash push -u -m "pre-cowork-cleanup"

# Verify clean state
git status
```

### P5 — Reconcile what Codex built with the LBC factory model

This is the most important item, and the most easily skipped. **None of the products Codex shipped have a row in `03_Portfolio/CLAUDE.md`.** They were built as standalone monorepo SKUs against research-doc prompts, but the LBC factory operates on three categories (SaaS, DevTool, SkillPack) with explicit cadence, kill criteria, and capital allocation rules.

For each of the four products built (MCP Builder Pro, GEO Audit, Production Bundle, Memory+RAG), the factory needs a decision:

| Product | Likely factory home | Action |
|---|---|---|
| MCP Server Builder Pro | SkillPack ($299 one-time) OR DevTool spike | Add to `03_Portfolio/CLAUDE.md` pipeline table; write a Spawn memo at `06_Factory_Playbook/Spawn_MCPBuilderPro_<date>.md` |
| GEO Audit | Could fold into the existing **Agentic Optimization Quickstart** skill pack (companion to AO-Bots) OR stand alone as a productized service. The research doc points toward standalone @ $299/$599. | Decide ownership: AO-Bots companion or own bet. |
| Production Bundle | Positioning SKU, not a factory product. Just a Lemon Squeezy bundle. | Document as a "bundle SKU" in `03_Portfolio/CLAUDE.md` notes, not a separate row. |
| Memory + RAG Add-ons | SkillPack pair ($99/$149 each). Two distinct packs or one combined? | Decide; add rows. |
| Vendor Marketplace Kit (if built) | DevTool ($399 one-time, self-hosted). RESPA-clean per the prompt's §5c guardrails. | Per `Hard Rule 3` in the workspace CLAUDE.md, flag any RESPA-adjacent positioning to counsel before launch — even though the Counsel-clean variant is structurally safe. |

**Hard rule reminder from `03_Portfolio/CLAUDE.md`:** LLC formation triggers at **first dollar paid**, not on shipping. So these four products do NOT need LLCs yet. They sit in the pre-LLC pipeline table until they generate revenue.

### P6 — Voice / brand audit of the landing pages Codex shipped

Codex generated four landing pages without knowing the cahbi brand rules. Pages need a copy pass against `CLAUDE.md` rules:

- **No em-dashes mid-sentence in buyer-facing copy** (cahbi brand rule N20). Codex used em-dashes liberally in the research doc; if any of that leaked into landing copy, fix.
- **"cahbi" always lowercase.** Unlikely to appear in these landings but check.
- **"Lonely Brew Club" always three words, properly capitalized externally.** If any landing mentions LBC by name, full form.
- **Core tenet "Love and Light" never appears in external materials.** Verify it didn't slip into FAQ copy.
- **No emojis** unless explicitly allowed. Codex tends to add them.
- **No manufactured urgency.** Per the tenet: "Buyer-facing copy never weaponizes fear · uses possibility-framing not loss-framing."

```bash
# Quick em-dash audit
grep -rn "—" site/app/*/page.tsx site/app/products/*/page.tsx products/*/README.md

# Quick emoji audit
grep -rPn "[\x{1F300}-\x{1FAFF}]" site/app/ products/
```

### P7 — Sync the research doc into the LBC repo

The market research that drove all five Codex prompts lives in `dirtylogic/yoyo/lbc-market-research-2026-05-25.md`, not in the LBC repo. Copy it into LBC for self-containment:

```bash
# From a checkout of yoyo, or download from the PR
curl -L "https://raw.githubusercontent.com/dirtylogic/yoyo/claude/lbc-market-research-pull-fdG3p/lbc-market-research-2026-05-25.md" \
  -o "05_References/lbc-market-research-2026-05-25.md"

git add 05_References/lbc-market-research-2026-05-25.md
git commit -m "docs: import market research from yoyo for self-containment"
```

Also worth copying: `dirtylogic/yoyo/SESSION_HANDOFF_2026-05-26.md` for the verbatim Codex prompt appendix.

### P8 — Decide yoyo's fate

`dirtylogic/yoyo` is not in either workspace CLAUDE.md or `03_Portfolio/CLAUDE.md`. It contains the research doc + two handoff docs and nothing else. Once the research is mirrored into LBC (P7), yoyo can be archived. Or kept as a deliberate scratch repo if you want a non-LBC sandbox for AI-infra experiments. Your call.

### P9 — Codex environment cleanup (low priority)

- Fix or remove `scripts/post_write_codex_agent_guardrail.py` reference in `.codex/config.toml`
- Patch the twilio-enterprise-knowledge SKILL.md description to ≤1024 chars (or accept the warning forever)
- Re-login Claude Desktop to refresh the claude-mem OAuth token if you want fresh observation context
- Decide whether to keep claude-mem's autoload of 172k tokens of unrelated `lbc-platform` history in every session start — that's a lot of noise per turn

---

## Useful context from the prior session

### The five Codex prompts (verbatim) are archived

Read them from `dirtylogic/yoyo/SESSION_HANDOFF_2026-05-26.md` Appendix A1–A6 in PR #1. The Security Audit prompt (A2) and Vendor Marketplace Kit prompt (A6) are still relevant. The Production Bundle (A4) and Memory+RAG (A5) prompts have already been executed.

### The "research-doc recommendations predate factory discovery" caveat

The research doc's §7 recommendation says: launch MCP Server Builder Pro → MCP/Agent Security Audit → GEO Audit. That recommendation was written before the prior session learned that LBC operates a SkillPack/SaaS/DevTool factory. Re-read the recommendation against the factory model — the products are still strong bets, they just need factory-category assignments before launch (see P5).

### What the prior session got wrong

I (the previous Claude Code session) told the user "Codex saved nothing" based on observing only the yoyo repo. That was incorrect — Codex was running in the LBC workspace and committed substantial product code to local branches. None of it was pushed at that time. The four feature branches plus `main` exist because of that local work.

I (the previous Claude Code session) also wrote five Codex prompts assuming a standalone monorepo structure (`/products/<name>/`, `/site/`, etc.) without knowing LBC operates a factory. Codex followed those prompts faithfully, which means the four products shipped use that monorepo structure rather than being formatted as factory SkillPacks. P5 above is where you fix this.

---

## What "done" looks like

By the end of this Cowork session:

- [ ] `main` history has no node_modules or large binaries
- [ ] All four product branches pushed to GitHub with one PR each
- [ ] Security Audit either reset cleanly OR re-run from scratch on its own branch
- [ ] Vendor Marketplace Kit decision: build, defer, or skip
- [ ] Each shipped product has a row in `03_Portfolio/CLAUDE.md` pipeline table
- [ ] At least one Spawn memo written for the product you're priming for first-dollar-paid
- [ ] Landing pages voice/brand passed against `CLAUDE.md` rules
- [ ] Research doc mirrored into `05_References/` or equivalent
- [ ] Yoyo fate decided (archive, retire, or keep)
- [ ] Worktree state clean
- [ ] Codex hook script either created or unreferenced

Push status update to the user when each P-item lands. Don't batch.

---

## One last thing

Before doing anything destructive (filter-repo, force-push, branch reset, worktree remove): make sure you've talked to David. The branch state is messy but every branch has real work on it. Confirm before you reshape history.

End of handoff.
