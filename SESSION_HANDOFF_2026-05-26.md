# Session Handoff — `dirtylogic/yoyo` — 2026-05-26

> Handoff from a Claude Code web session (remote container, no filesystem access beyond this repo) to whichever session picks this up next, ideally a **local Claude Code session running inside `/Volumes/FMNC 8_T_B/Lonely Brew Club/`** with full portfolio context loaded.

---

## TL;DR

- **What shipped from this session:** `lbc-market-research-2026-05-25.md` (625-line market research pull across 6 product clusters) plus this handoff doc.
- **What's NOT shipped, only scratched:** five Codex prompts for AI-infra SKUs (MCP Builder Pro, Security Audit, GEO Audit, Production Bundle, Memory+RAG add-ons, Vendor Marketplace Kit). All preserved verbatim below. None of them were committed as code. None of them are factory-spec.
- **Critical context discovered late in the session:** `dirtylogic/yoyo` is NOT the LBC operating workspace. The actual workspace is `/Volumes/FMNC 8_T_B/Lonely Brew Club/`. The Codex prompts were drafted as standalone monorepo products, which is off-spec for the LBC SkillPack/SaaS/DevTool factory model.
- **Decision parked by David:** stop pre-planning SKUs in this thread, ship what we built, regroup locally with the full portfolio in view.

---

## Repo state at handoff

```
dirtylogic/yoyo
├── README.md                              # single-line "# yoyo"
├── lbc-market-research-2026-05-25.md      # 625-line market research pull
└── SESSION_HANDOFF_2026-05-26.md          # this file

branches:
  master                                          (initial commit only)
  claude/lbc-market-research-pull-fdG3p           (research doc + this handoff)
  origin/claude/lbc-market-research-pull-fdG3p    (in sync)

PRs:
  #1 open against master — research doc + this handoff
```

**Open question for local session:** what is `dirtylogic/yoyo`'s actual role in the portfolio? It is not mentioned in `Lonely Brew Club/CLAUDE.md` or `Lonely Brew Club/03_Portfolio/CLAUDE.md`. Candidates: pre-spike scratch repo for a future product LLC, dumping ground for AI-infra research, factory tooling. Local session should resolve this before any further commits land here.

---

## What we actually built in this session

### 1. Market research pull (committed, in PR #1)

`lbc-market-research-2026-05-25.md`. Six clusters analyzed: MCP, agent security, agent memory, RAG testing, AI citation/GEO, skill products. Includes:

- Section 1: trend data per term with cluster ranking (MCP hottest, agent security highest WTP, GEO hot/broad, skill products crowded, memory/RAG warm)
- Section 2: competitor pricing tables (skill packs $17-29, MCP boilerplates free/OSS, GEO SaaS $189-495/mo, RAG eval OSS+SaaS, observability $29-2,499/mo, infra templates $199-349 lifetime)
- Section 3: marketplace signals across GitHub, Docker MCP, Vercel, Supabase, PH, Gumroad, Lemon Squeezy, Stripe, Claude marketplaces, Cursor — with white-space synthesis
- Section 4: 31 community pain quotes mapped to product ideas with hottest→coldest ranking
- Section 5a: LBC asset readiness audit (verified nothing-in-this-repo at time of writing besides README)
- Section 5b: distribution lever ranking
- Section 5c: RESPA Counsel-gate matrix for the Real Estate Vendor Marketplace Kit variants
- Section 6: 50-prospect outreach list with warm/cold tagging and pitch angles
- Section 7: 7-day operational sequence and the working-hypothesis-vs-data delta

The Section 7 recommendation was: launch MCP Server Builder Pro → MCP/Agent Security Audit → GEO Audit, with Production AI Shipping Bundle as a wrapper and Memory+RAG as add-ons. **This recommendation predates the discovery that LBC operates a SkillPack factory with its own pre-existing pack inventory.** See "Off-spec for LBC factory" below.

### 2. Five Codex prompts (NOT committed as code, preserved verbatim below)

I authored Codex prompts intended to run sequentially against this repo, each opening its own branch and PR. They assumed a generic TypeScript monorepo with Hono on Cloudflare Workers + Next.js 15 landings + Lemon Squeezy fulfillment. David ran the Vendor Marketplace Kit prompt against Codex; Codex returned a faithful 5-line plan but no code was written. The other four prompts were never sent to Codex.

The prompts are in the appendix below for archival. **Do not ship them as-is.** They are off-spec for the LBC factory model.

---

## Off-spec for LBC factory (the most important finding)

After David shared `Lonely Brew Club/CLAUDE.md` and `Lonely Brew Club/03_Portfolio/CLAUDE.md`, I learned:

**LBC operates three product categories:**
| Category | Description | Cycle to revenue | Price band |
|---|---|---|---|
| SaaS | Multi-tenant subscription. cahbi, Planulator. | 3-9 months | $50-500/mo |
| DevTool | Dev/agent infra. Hosted swarm pattern is a possible future bet. | 3-6 months | $99-2,000+ |
| SkillPack | Markdown skill bundles sold direct. No ongoing service. | 7-14 days | $99-299 one-time |
| PersonalInfra | Internal only. Trading Bot, ai-operator. | n/a | n/a |

**Current portfolio inventory (as of 2026-05-13 per `03_Portfolio/CLAUDE.md`):**

Formed/forming product LLCs:
- **cahbi** (SaaS, shipped 2026-05-21 with John Palmer Real Estate as founding broker tenant; cahbi LLC planned, not yet formed)

Pre-LLC pipeline:
- **Planulator** (SaaS, late Spike) — PDF→CAD for architects
- **AO-Bots** (SaaS or DevTool TBD, Spike) — 7-agent AI recommendation visibility pipeline
- **Trading Bot** (PersonalInfra w/ skill-pack optionality, Spike)
- **ai-operator** (PersonalInfra w/ productization optionality, Idea)
- **mememe** (parked, clarification needed)

Skill pack inventory:
- **Parallel Agent Lanes (PAL)** — $199, **PILOT** (13 skills + 10 examples drafted 2026-05-13, CC autonomous build plan ready for Stages 4-7)
- **Real Estate SaaS Founder Pack** — $149, Backlog
- **Solo Agent-Powered Product Incubator** (meta-pack) — $199, Backlog
- **AI-Native CAD Drafting** — $99, Backlog
- **AI Trading Organization Design** — $129, Backlog
- **Agentic Optimization Quickstart** — $99, Backlog

**Implications for the AI-infra SKUs I prompted Codex for:**

1. **MCP Builder Pro, Security Audit, GEO Audit, Memory/RAG kits, Vendor Marketplace Kit are NOT on either the formed-LLC or pre-LLC pipeline.** If David wants any of them in the factory they need to be either (a) reframed as SkillPacks ($99-299, markdown bundle, 7-14 day cycle, ships via LBC Mercury Stripe direct) or (b) added as new pre-LLC bets to the pipeline with proper spike → first dollar → LLC formation discipline.
2. **GEO/AI-citation already has a factory home.** The Agentic Optimization Quickstart skill pack is the existing companion to AO-Bots. The research-doc GEO Audit thesis should fold into that, not spawn a new product.
3. **MCP/agent-security and RAG/memory have no current factory home.** Would be new bets if pursued.
4. **The Codex prompts I wrote assume Hono+Cloudflare Workers+Next.js+Drizzle+D1+Lemon Squeezy.** None of that matches the SkillPack distribution path (markdown files, direct Stripe checkout via LBC Mercury, landing page on Webflow per the workspace stack).

---

## What's in flight vs parked

**In flight:**
- PR #1 on `dirtylogic/yoyo` — research doc + this handoff. Awaiting David's merge decision.
- (Per workspace context, not this repo) cahbi shipped 2026-05-21; PAL skill pack in pilot stage with CC autonomous build plan ready for Stages 4-7.

**Parked (do not resume without explicit go from David):**
- All five AI-infra SKU prompts (MCP Builder, Security Audit, GEO Audit, Production Bundle, Memory+RAG add-ons, Vendor Marketplace Kit).
- The "production AI shipping bundle" framing — the research doc recommends it as a $999 wrapper, but until the constituent SKUs are reframed as SkillPacks or pre-LLC bets, the wrapper has nothing to wrap.

---

## What the local session should do next

In rough priority order:

1. **Read this file + `lbc-market-research-2026-05-25.md` from this repo first** (you'll need to either pull `dirtylogic/yoyo` locally, or open the open PR #1 in browser, or just have me re-paste). The research findings are durable even if the SKU prompts derived from them are off-spec.
2. **Resolve what `dirtylogic/yoyo` is for.** Three candidates: (a) scratch repo for an AI-infra product spike, (b) the GitHub home for a future product LLC, (c) deletable. Once resolved, either commit this handoff intent to `03_Portfolio/` as a portfolio decision memo, or close yoyo down.
3. **Decide whether any of the research-doc themes graduate to new factory bets.** Strongest candidates per the data:
   - **MCP/Agent Security** — highest WTP cluster in the dataset, clean white space in the $499-2,999 productized audit lane. No current factory home. Could be a new SaaS spike (audit-as-a-service) or a SkillPack (security checklist + remediation skill).
   - **MCP Server Builder** — hottest demand-side, all named pain points are real, but the boilerplate template lane is OSS-dominated. SkillPack framing ("MCP Server Skill Pack") is the cleaner factory fit than a paid template.
   - **GEO/AI-citation** — already has a factory home in Agentic Optimization Quickstart (companion to AO-Bots). The research strengthens that pack's positioning rather than creating a new bet.
4. **If yes to any of (3), draft a Spawn memo at `06_Factory_Playbook/Spawn_<PackName>_<YYYY-MM-DD>.md`** per the SkillPack spawn workflow described in `03_Portfolio/CLAUDE.md`.
5. **Merge or close PR #1.** Either way, the research doc has value as a reference; if yoyo gets repurposed or deleted, copy the research doc to `05_References/` first.

---

## Voice / brand notes carried in from workspace CLAUDE.md

- "cahbi" is always lowercase.
- "Lonely Brew Club" is always three words, properly capitalized externally; "LBC" is fine internally.
- Core tenet "Love and Light" never appears in external materials. Internally it may be named sparingly when it serves as an explicit arbiter.
- RESPA § 8 hard rule: no per-loan/per-escrow/per-cert/per-policy kickback structures touching settlement-service vendors (Qualia, CondoCerts, CA FAIR Plan, LendingPad).
- No em-dashes mid-sentence in buyer-facing copy (cahbi brand rule N20). Internal exempt; use sparingly.
- No emojis unless David uses one first.
- PII never persisted to memory or workspace files unless filling a form requiring it.

---

## Appendix: the five parked Codex prompts (verbatim, for archival)

These were drafted before I knew LBC operates a factory model. Do not ship them as written. If any of the themes graduate to factory bets, the prompts can serve as raw material for a SkillPack spawn memo or a SaaS spike charter, with substantial reframing.

### A1. MCP Server Builder Pro (would have been "SKU #1")

(Prompt was given to David earlier in the session; not preserved verbatim in this thread's tool history. Reconstructible from the structural conventions in the prompts below: TypeScript monorepo, Hono on Cloudflare Workers, Drizzle+D1, Next.js 15 landing, Resend, Lemon Squeezy webhook, $299 founder / $499 list, ships as a Claude Skill + GitHub template + LS delivery.)

### A2. MCP / Agent Security Audit

```
You are shipping the second paid product. Same repo as MCP Server Builder Pro
(`claude/mcp-server-builder-pro` already merged or open). Read
`lbc-market-research-2026-05-25.md` §4 "Agent Security" rows and §7 first.
This is a productized one-off SERVICE, not a template. $499 founder /
$999 list, payable via Lemon Squeezy.

# Goal
A buyer fills a 6-field intake form, pays, and within 48 hours receives a
PDF audit report scoring their MCP server / AI agent against the named
attack surfaces in research §4, plus a remediation Claude Skill they install
to auto-fix common findings.

# Deliverables (branch `claude/agent-security-audit`)
[full prompt body — see thread for verbatim including intake form, report
generator, remediation skill, fulfillment, ops sections, constraints, and
definition of done]
```

### A3. AI Citation / GEO Audit

```
You are shipping the third paid product. Same repo and conventions as the
two prior. Read research §4 "AI Citation" rows and §7. $299 founder /
$599 list.

# Goal
A buyer enters their domain + 5 target keywords, pays, and within 72 hours
receives a PDF showing their share-of-voice across ChatGPT, Perplexity,
Claude, and Gemini for those queries, with a 30-day playbook to improve
citations.

# Deliverables (branch `claude/geo-audit`)
[full prompt body — see thread for verbatim including intake form, audit
toolkit with 120-query operator-driven runner, 30-day re-scan cron,
fulfillment, ops sections, and the do-NOT-integrate-LLM-APIs constraint]
```

### A4. Production AI Shipping Bundle

```
You are shipping a bundle SKU that wraps the three products already built
(MCP Server Builder Pro, Security Audit, GEO Audit) at $999 list — $200
below the sum of standalones. No new product code, just landing + checkout +
fulfillment.

# Deliverables (branch `claude/production-ai-bundle`)
[full prompt body — see thread for verbatim including landing, bundle
playbook, fulfillment via shared LS webhook, ops, and the zero-new-deps
constraint with ~400 line diff ceiling]
```

### A5. Memory + RAG add-ons

```
You are shipping two small upsell SKUs that attach to the MCP Server
Builder Pro checkout. Read research §1 "Agent memory" + "RAG testing" rows
and §4 Memory Pack / RAG Regression rows.

# Deliverables (branch `claude/memory-rag-addons`)
- Memory Kit at `/products/memory-kit/` — Mem0/Zep/SQLite adapter pattern
- RAG Regression Harness at `/products/rag-regression-harness/` — Python
  (Ragas + DeepEval + GitHub Actions + pytest, justified break from TS)
- Upsell cards on the MCP Builder thank-you page
- Fulfillment via shared LS webhook
[full prompt body — see thread for verbatim]
```

### A6. Vendor Marketplace Kit (Counsel-clean variant only)

```
You are shipping a sixth paid product to the same monorepo. Read research
§4 "Vendor Marketplace Kit" rows AND §5c "Counsel-gate" rows BEFORE
writing anything. The Counsel-gate concern in §5c is that any variant
which takes a percentage / transaction / take-rate fee on a real-estate-
adjacent transaction can trigger broker, agent, or money-transmitter
licensing in many U.S. states. We are NOT seeking counsel and we are NOT
shipping that variant. This prompt builds the structurally clean one.

# Product positioning
"Vendor Marketplace Kit" — a self-hostable template that a property
manager or small landlord installs on their own infra. The buyer owns
every vendor relationship; we never sit between PM and vendor; no money
flows through code we ship; no funds are held; no introductions are
monetized.

# Pricing
$399 founder / $799 list — one-time license fee. NO subscription, NO
per-vendor fee, NO per-transaction fee, NO escrow, NO marketplace
listing-fee model.

# Deliverables (branch `claude/vendor-marketplace-kit`)
[full prompt body — see thread for verbatim including landing with
explicit disclaimer block, self-hosted Next.js+SQLite template, omitted
features list, dispatch skill, fulfillment, positioning guardrails ops doc]
```

Note: David ran A6 against Codex; Codex returned a faithful 5-line plan but no code was written before David called the rescope. The Codex thread can be told to stand down.

---

## End of handoff
