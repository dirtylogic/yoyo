# LBC Product Market Research Pull — 2026-05-25

> Buyer-signal pull across 6 product clusters (MCP, agent security, agent memory, RAG testing, AI citation/GEO, skill products). Sources cited inline; honest "no data accessible" flags where pulls were auth-walled or rate-limited. Compiled from 5 parallel research streams plus repo inventory.

---

## 1. Trend Data

- **Term:** model context protocol
- **Cluster:** MCP
- **12-month direction:** rising (sharply)
- **90-day direction:** rising
- **Breakout queries / related topics:** "MCP OAuth 2.1", "MCP registry", "MCP enterprise adoption", "MCP CVEs"
- **Regional skew:** US ~27% of global query volume; Japan #2; India #3 (Anthropic opened India office Q1 2026)
- **Evidence link(s):** https://www.digitalapplied.com/blog/mcp-adoption-statistics-2026-model-context-protocol  ·  https://www.digitalapplied.com/blog/mcp-97-million-downloads-model-context-protocol-mainstream  ·  https://zuplo.com/mcp-report
- **Takeaway:** Peak buyer attention. SDK at 97M downloads, 78% of enterprise AI teams have ≥1 MCP agent in prod. A $99–$999 MCP-themed skill pack launching this week lands in the highest-intent window of the year.

- **Term:** MCP server
- **Cluster:** MCP
- **12-month direction:** rising
- **90-day direction:** rising
- **Breakout queries / related topics:** "best MCP servers 2026", "self-hosted MCP server", "MCP server template", "private MCP server"
- **Regional skew:** US dominant; strong India enterprise growth; Japan unusually high consumer (Figma/Notion/Playwright MCPs)
- **Evidence link(s):** https://mcpmanager.ai/blog/most-popular-mcp-servers/  ·  https://bloomberry.com/blog/we-analyzed-1400-mcp-servers-heres-what-we-learned/  ·  https://workos.com/blog/everything-your-team-needs-to-know-about-mcp-in-2026
- **Takeaway:** "How do I build/pick/secure an MCP server" is the dominant buyer query. Templates and audit packs at $199–$499 are well-aligned to current pain.

- **Term:** MCP marketplace
- **Cluster:** MCP
- **12-month direction:** rising
- **90-day direction:** rising (but fragmenting)
- **Breakout queries / related topics:** "MCP registry", "MCP Hubs", "Smithery", "PulseMCP", "MCP discovery"
- **Regional skew:** US-led; UK/EU emerging via Zuplo/WorkOS audience
- **Evidence link(s):** https://www.mcpbundles.com/blog/best-mcp-servers  ·  https://mcpmarket.com/  ·  https://medium.com/@adnanmasood/inside-the-fractured-world-of-ai-agent-marketplaces-da80e7e03dd0
- **Takeaway:** Ecosystem is fractured across 8+ marketplaces — operators are confused about where to list. A "which MCP marketplace to launch on" decision-guide / audit ($299–$599) has clear pull.

- **Term:** MCP tools
- **Cluster:** MCP
- **12-month direction:** rising
- **90-day direction:** flat-to-rising (now a generic term)
- **Breakout queries / related topics:** "MCP tools for Claude", "MCP tools list", "best MCP tools 2026"
- **Regional skew:** US/India dev-heavy
- **Evidence link(s):** https://github.com/tolkonepiu/best-of-mcp-servers  ·  https://www.taskade.com/blog/mcp-servers
- **Takeaway:** High volume, lower intent — searchers want free lists. Use as top-of-funnel; monetization sits one layer down (templates, security, integration audits).

- **Term:** MCP security
- **Cluster:** MCP / Agent security
- **12-month direction:** rising (steepest curve in the MCP cluster)
- **90-day direction:** rising sharply
- **Breakout queries / related topics:** "MCP CVE", "MCP tool poisoning", "MCP OAuth 2.1", "MCP supply chain"
- **Regional skew:** US-heavy; strong UK/EU enterprise interest (Gravitee, NeuralTrust audiences)
- **Evidence link(s):** https://www.practical-devsecops.com/mcp-security-vulnerabilities/  ·  https://www.ox.security/blog/mcp-supply-chain-advisory-rce-vulnerabilities-across-the-ai-ecosystem/  ·  https://thehackernews.com/2026/01/three-flaws-in-anthropic-mcp-git-server.html
- **Takeaway:** 30+ CVEs in a single 60-day window, 492 publicly-exposed unauthenticated MCP servers found by Trend Micro. Highest willingness-to-pay in the report — audits and hardening packs can comfortably price at $499–$999.

- **Term:** AI agent security
- **Cluster:** Agent security
- **12-month direction:** rising
- **90-day direction:** rising
- **Breakout queries / related topics:** "agent identity", "agent permissions", "agentic AI governance", "non-human identity"
- **Regional skew:** US/UK/Israel security-vendor heavy
- **Evidence link(s):** https://www.gravitee.io/blog/state-of-ai-agent-security-2026-report-when-adoption-outpaces-control  ·  https://www.darktrace.com/blog/state-of-ai-cybersecurity-2026-92-of-security-professionals-concerned-about-the-impact-of-ai-agents  ·  https://www.kiteworks.com/cybersecurity-risk-management/ai-agent-security-incidents-2026/
- **Takeaway:** 88% of orgs reported confirmed/suspected agent incidents in the past year, 92% of security pros concerned. CISO buyer present and budget-flush — premium audit SKU justified.

- **Term:** prompt injection
- **Cluster:** Agent security
- **12-month direction:** rising
- **90-day direction:** rising
- **Breakout queries / related topics:** "indirect prompt injection", "tool poisoning", "Morris II worm", "OWASP LLM Top 10"
- **Regional skew:** US-led; strong academic skew (arXiv, Google research)
- **Evidence link(s):** https://markaicode.com/prompt-injection-attacks-ai-security-2026/  ·  https://sqmagazine.co.uk/prompt-injection-statistics/  ·  https://unit42.paloaltonetworks.com/model-context-protocol-attack-vectors/
- **Takeaway:** Wiz tracked +340% YoY attempts; OWASP names it the #1 AI threat for 2026. A prompt-injection red-team / audit pack at $499–$999 has clear demand.

- **Term:** AI agent permissions
- **Cluster:** Agent security
- **12-month direction:** rising (newer term — steeper relative growth)
- **90-day direction:** rising
- **Breakout queries / related topics:** "non-human identity", "over-permissioned agents", "agent IAM", "agent least privilege"
- **Regional skew:** US enterprise security
- **Evidence link(s):** https://www.token.security/blog/the-2026-data-breach-investigations-report-confirms-it-identity-is-the-control-plane-for-agentic-ai  ·  https://www.cyberark.com/resources/blog/ai-agents-and-identity-risks-how-security-will-shift-in-2026  ·  https://venturebeat.com/security/cisco-crowdstrike-rsac-2026-agent-identity-iam-gap-maturity-model
- **Takeaway:** Gartner placed agent IAM at top of 2026 cybersec trend list; 51% of orgs cite over-permissioning as top pain. A "permissions audit + least-privilege template pack" at $299–$799 fits.

- **Term:** AI agent memory
- **Cluster:** Agent memory
- **12-month direction:** rising
- **90-day direction:** rising
- **Breakout queries / related topics:** "LongMemEval", "agent memory layer", "Cloudflare Agent Memory", "temporal knowledge graph"
- **Regional skew:** US-led; SF/Bay-Area startup cluster
- **Evidence link(s):** https://mem0.ai/blog/state-of-ai-agent-memory-2026  ·  https://atlan.com/know/best-ai-agent-memory-frameworks-2026/  ·  https://hermesos.cloud/blog/ai-agent-memory-systems
- **Takeaway:** Cloudflare's April 2026 private-beta launch is the inflection moment. A "memory architecture decision pack" or Mem0/Zep migration template at $199–$499 should sell.

- **Term:** persistent memory AI
- **Cluster:** Agent memory
- **12-month direction:** rising (lower base)
- **90-day direction:** rising
- **Breakout queries / related topics:** "long-term memory agent", "vector memory", "Mem0 vs Zep"
- **Regional skew:** US, India developer audiences
- **Evidence link(s):** https://byteiota.com/persistent-memory-for-ai-agents-2026-implementation/  ·  https://mem0.ai/blog/ai-memory-benchmarks-in-2026
- **Takeaway:** Lower search volume than "AI agent memory" but higher intent — tutorial-style buyers. Implementation skill pack at $99–$299 fits.

- **Term:** agent memory
- **Cluster:** Agent memory
- **12-month direction:** rising
- **90-day direction:** rising
- **Breakout queries / related topics:** "agent memory benchmark", "agent memory framework"
- **Regional skew:** US/EU
- **Evidence link(s):** https://dev.to/vektor_memory_43f51a32376/the-state-of-ai-agent-memory-in-2026-what-the-research-actually-shows-3aja  ·  https://vectorize.io/articles/best-ai-agent-memory-systems
- **Takeaway:** Same buyer as "AI agent memory" — use as a secondary keyword. Bundle into a single memory-architecture SKU.

- **Term:** Mem0
- **Cluster:** Agent memory
- **12-month direction:** rising
- **90-day direction:** rising
- **Breakout queries / related topics:** "Mem0 vs Zep", "Mem0 alternatives", "Mem0 LangGraph"
- **Regional skew:** US/India (YC-backed, heavy Indian dev community)
- **Evidence link(s):** https://github.com/mem0ai/mem0  ·  https://virtuslab.com/blog/ai/git-hub-all-stars-2  ·  https://atlan.com/know/mem0-alternatives/
- **Takeaway:** 51,800+ stars, 21 framework integrations. Branded "Mem0 integration template" or "Mem0 production pack" at $99–$299 rides clear branded search demand.

- **Term:** RAG evaluation
- **Cluster:** RAG testing
- **12-month direction:** rising
- **90-day direction:** rising
- **Breakout queries / related topics:** "Ragas", "DeepEval", "LLM-as-judge", "context precision"
- **Regional skew:** US/EU enterprise AI; India strong via Maxim AI / Atlan audiences
- **Evidence link(s):** https://blog.premai.io/rag-evaluation-metrics-frameworks-testing-2026/  ·  https://atlan.com/know/llm-evaluation-frameworks-compared/  ·  https://www.braintrust.dev/articles/best-rag-evaluation-tools
- **Takeaway:** Mature search term — buyers know what they want. A pre-built Ragas+DeepEval starter / gold-set template at $199–$499 should convert.

- **Term:** RAG testing
- **Cluster:** RAG testing
- **12-month direction:** rising
- **90-day direction:** rising
- **Breakout queries / related topics:** "RAG CI/CD", "RAG pytest", "RAG gold set"
- **Regional skew:** US/EU dev
- **Evidence link(s):** https://testquality.com/llm-regression-testing-pipeline/  ·  https://www.getmaxim.ai/articles/top-5-tools-to-evaluate-rag-performance-in-2026/
- **Takeaway:** Practitioner-leaning. GitHub Actions + pytest RAG-testing template ($99–$299) is a clean fit.

- **Term:** RAG regression
- **Cluster:** RAG testing
- **12-month direction:** rising (low base — narrower term)
- **90-day direction:** rising
- **Breakout queries / related topics:** "RAG regression test", "RAG baseline drift", "LLM regression"
- **Regional skew:** US engineering teams
- **Evidence link(s):** https://testquality.com/llm-regression-testing-pipeline/  ·  https://blog.premai.io/rag-evaluation-metrics-frameworks-testing-2026/
- **Takeaway:** Highest-intent term in the RAG cluster — buyers already have RAG in prod and feel pain. Premium $499–$799 audit/setup SKU justified.

- **Term:** RAG eval framework
- **Cluster:** RAG testing
- **12-month direction:** flat-to-rising
- **90-day direction:** flat (consolidating around Ragas/DeepEval)
- **Breakout queries / related topics:** "Ragas vs DeepEval", "TruLens", "Phoenix"
- **Regional skew:** US/EU
- **Evidence link(s):** https://callsphere.ai/blog/rag-evaluation-frameworks-2026-ragas-trulens-deepeval  ·  https://deepchecks.com/best-rag-evaluation-tools/
- **Takeaway:** Comparison-stage buyers. Best monetized as a comparison guide funneling into a setup template.

- **Term:** AI citation
- **Cluster:** AI citation
- **12-month direction:** rising
- **90-day direction:** rising
- **Breakout queries / related topics:** "AI citation tracker", "ChatGPT citations", "Perplexity citations", "Reddit citations"
- **Regional skew:** US marketing-agency heavy; UK/AU growing
- **Evidence link(s):** https://www.averi.ai/blog/ai-citation-tracking-chatgpt-perplexity-claude  ·  https://topify.ai/blog/ai-citation-tracking-platform  ·  https://www.pixelmojo.io/blogs/how-to-track-ai-citations-chatgpt-perplexity-claude-gemini
- **Takeaway:** Marketing/SEO buyer with budget. "Get-cited" playbook or audit at $299–$799 lands well.

- **Term:** AI search optimization
- **Cluster:** AI citation
- **12-month direction:** rising
- **90-day direction:** rising
- **Breakout queries / related topics:** "AI Overviews optimization", "ChatGPT SEO", "Perplexity SEO"
- **Regional skew:** US/UK/IN agency markets
- **Evidence link(s):** https://www.semrush.com/blog/best-ai-seo-tools/  ·  https://sapt.ai/insights/ai-search-optimization-complete-guide-chatgpt-perplexity-citations
- **Takeaway:** Highest-volume term in the citation cluster. Use as lead-gen; bundle skill pack with citation tracking deliverables.

- **Term:** answer engine optimization
- **Cluster:** AI citation
- **12-month direction:** rising
- **90-day direction:** rising
- **Breakout queries / related topics:** "AEO tools", "AEO vs SEO", "AEO checklist"
- **Regional skew:** US/UK
- **Evidence link(s):** https://blog.hubspot.com/marketing/answer-engine-optimization-trends  ·  https://scrunch.com/blog/best-answer-engine-optimization-aeo-generative-engine-optimization-geo-tools-2026
- **Takeaway:** HubSpot/Semrush amplifying the term — strong buyer awareness. AEO audit pack at $299–$599 fits.

- **Term:** generative engine optimization
- **Cluster:** AI citation
- **12-month direction:** rising (steepest in this cluster)
- **90-day direction:** rising
- **Breakout queries / related topics:** "GEO benchmark", "GEO vs SEO", "GEO tools", "Profound", "Peec"
- **Regional skew:** US-led; G2 Winter 2026 reports show US/UK/CA strongest
- **Evidence link(s):** https://searchengineland.com/mastering-generative-engine-optimization-in-2026-full-guide-469142  ·  https://www.convertmate.io/research/geo-benchmark-2026  ·  https://www.tryprofound.com/blog/best-generative-engine-optimization-tools
- **Takeaway:** Hottest term in the cluster. AI search traffic reportedly 4.4x conversion of organic and +527% YoY. GEO audit/template product at $499–$999 commands premium pricing.

- **Term:** GEO SEO
- **Cluster:** AI citation
- **12-month direction:** rising (lower base, ambiguous with geography)
- **90-day direction:** rising
- **Breakout queries / related topics:** "GEO SEO meaning", "GEO vs SEO 2026"
- **Regional skew:** US
- **Evidence link(s):** https://www.emarketer.com/content/faq-on-geo-aeo--where-ai-search-seo-overlap-2026  ·  https://traffictorch.net/blog/posts/state-of-seo-geo-2026/
- **Takeaway:** Educational-stage term. Use as top-of-funnel for a GEO audit SKU; do not price the lead magnet.

- **Term:** Claude skills
- **Cluster:** Skill products
- **12-month direction:** rising sharply
- **90-day direction:** rising (Skills v2 dropped — clear spike)
- **Breakout queries / related topics:** "Claude Skills v2", "/batch skill", "Anthropic Agent Skills", "SKILL.md"
- **Regional skew:** US dev-heavy; growing IN/UK
- **Evidence link(s):** https://www.anthropic.com/news/skills  ·  https://github.com/anthropics/skills  ·  https://thenewstack.io/agent-skills-anthropics-next-bid-to-define-ai-standards/
- **Takeaway:** Anthropic skills repo at 135K+ stars; Skills v2 just launched. This term is the single most aligned to LBC's product line — launch directly into the spike.

- **Term:** Claude Code skills
- **Cluster:** Skill products
- **12-month direction:** rising
- **90-day direction:** rising
- **Breakout queries / related topics:** "best Claude Code skills", "Claude Code plugin marketplace", "/skill"
- **Regional skew:** US dev
- **Evidence link(s):** https://www.agensi.io/learn/best-claude-code-skills-2026  ·  https://claudemarketplaces.com/  ·  https://www.firecrawl.dev/blog/best-claude-code-skills
- **Takeaway:** 170K+ monthly visitors to marketplace directories. Premium skill pack at $99–$299 with a clear vertical hook (security, RAG, GEO) lands cleanly.

- **Term:** AI skill marketplace
- **Cluster:** Skill products
- **12-month direction:** rising (new term)
- **90-day direction:** rising
- **Breakout queries / related topics:** "Skills.sh", "SkillsMP", "Agensi", "LobeHub skills"
- **Regional skew:** US; new EU/IN entrants
- **Evidence link(s):** https://www.agensi.io/learn/best-ai-agent-skills-marketplaces-2026  ·  https://skillsmp.com/  ·  https://lobehub.com/skills
- **Takeaway:** Marketplaces are proliferating (8+ now). A multi-marketplace "list-everywhere" launch playbook adds defensible value; consider $199 deployment add-on.

- **Term:** AI agent templates
- **Cluster:** Skill products
- **12-month direction:** rising
- **90-day direction:** rising
- **Breakout queries / related topics:** "agent template library", "operator template", "pre-built AI agents"
- **Regional skew:** US/IN enterprise automation
- **Evidence link(s):** https://ezintegrations.ai/ai-agent-templates-enterprise-top20/  ·  https://www.digitalapplied.com/blog/ai-agent-marketplaces-2026-discovery-distribution  ·  https://arahi.ai/blog/best-ai-agents-for-business-2026
- **Takeaway:** Buyer expects 1,500+ template platforms already exist — differentiate on niche/vertical (security, RAG, GEO). Operator template bundles at $199–$599 fit.

> *Google Trends UI not directly accessible — directional reads above derived from 2026 publication volume, GitHub star counts, vendor reports (Wiz, Trend Micro, Cisco, Gartner-cited), and marketplace-traffic figures. No hard Trends index numbers fabricated.*

### Cluster ranking — hottest to coldest

1. **MCP** — Hottest. 97M SDK downloads, 78% enterprise adoption, +18% MoM server registry growth; protocol at peak buyer attention and ambiguity is highest (best monetization window).
2. **Agent security** — Very hot, highest willingness-to-pay. 88% of orgs reporting incidents, +340% YoY prompt injection attempts, Gartner #1 cybersec trend — premium audit SKUs justified here over any other cluster.
3. **AI citation / GEO** — Hot and broadest marketing buyer. 527% YoY AI search traffic growth, mature spend channels (agencies already buy SEO tools) — best fit for $299–$799 audit/playbook SKUs.
4. **Skill products** — Hot but crowded. Skills v2 launch is a real spike, but 8+ marketplaces and 800K+ scraped skills mean differentiation/niche is mandatory.
5. **Agent memory + RAG testing** (tied) — Warm, practitioner buyer, smaller TAM. Best as add-on SKUs ($99–$299) bundled with MCP or security packs rather than standalone hero products.

---

## 2. Competitor Examples

### AI skill packs

| Product | Category | Price | Buyer | Promise | Link | Notes |
|---|---|---:|---|---|---|---|
| Premium Claude Skills Collection (Usama Akram) | AI skill packs | ~$27 | Solo AI ops / agencies | "50 AI Specialists, complete operating system for AI business" | usamaakrm.gumroad.com/l/premium-claude-skills | Info product; lifetime updates; no refund stated |
| Claude Skills Pack (ThinkAIPrompt) | AI skill packs | $17 | ChatGPT/Claude power users | "30 skill files, install once, use forever" | thinkaiprompt.gumroad.com/l/claude-skills | Info product; cross-model |
| Claude Code Prompt Pack (Maxtendies) | AI skill packs | $19 | Working devs | "50+ battle-tested dev prompts" | maxtendies.gumroad.com/l/claude-code-prompt-pack | Info product |
| Cursor Rules Pack v2 (Olivia Craft) | AI skill packs | $29 | Devs in 14 stacks | "50 production-tested .cursorrules" | oliviacraftlat.gumroad.com/l/wyaeil | Info product; "no-brainer" pricing |
| Cursor Doctor Pro | AI skill packs | ~$15–25 | Cursor users | "Fix Cursor output failures" | nedcodes.gumroad.com/l/cursor-doctor-pro | Info product |
| AI Agent Complete Bundle (10 tools) | AI skill packs | $29 (from $119) | Indie builders | "10 premium tools, templates & guides" | aiagenttools.gumroad.com/l/riwdzt | Bundle/info |
| Agensi Skills Marketplace | AI skill packs | Per-skill $5–$50 | Devs wanting vetted skills | "8-point security scan on every skill, creators keep 80%" | agensi.io | Marketplace; security-vetted |

### MCP products

| Product | Category | Price | Buyer | Promise | Link | Notes |
|---|---|---:|---|---|---|---|
| PaidMCP Boilerplate (Alby) | MCP products | Free / OSS | MCP builders adding paywall | "Boilerplate paid MCP server with PaidMCP" | github.com/getAlby/paidmcp-boilerplate | Free template — no paid kit found |
| iannuttall/mcp-boilerplate | MCP products | Free (was paid) | Devs shipping remote MCP w/ auth | "Remote MCP boilerplate w/ user auth + Stripe paid tools" | github.com/iannuttall/mcp-boilerplate | Was sold, now open-sourced — signals weak willingness-to-pay at template tier |
| f/mcp-startup-boilerplate | MCP products | Free | MCP startups | "OAuth2 + Stripe subscription tools out of the box" | github.com/f/mcp-startup-boilerplate | Free |
| Runlayer (Enterprise MCPs/Skills/Agents) | MCP products | contact sales | Enterprises | "Enterprise MCP gateway + skills + agent governance" | runlayer.com | SaaS; gated pricing |
| MintMCP Gateway | MCP products | contact sales | Enterprises | "SOC-2 Type II MCP gateway, removes need to audit MCP infra" | mintmcp.com | SaaS; gated |
| Builder Pack #1 (Multi-Agent ADK + MCP) | MCP products | ~$49 | Devs building agent stacks | "ADK, A2A, MCP servers, Streamlit, Cloud Run scripts" | gumroad.com/u/iyjcgzxr | Info/template hybrid |

### AI SEO / GEO audits

| Product | Category | Price | Buyer | Promise | Link | Notes |
|---|---|---:|---|---|---|---|
| Profound (Starter / Growth) | AI SEO/GEO | $82.50/mo–$332.50/mo (annual) → now $399/mo+ | Enterprise marketers | "Track ChatGPT/AEO visibility, 50–100 prompts" | tryprofound.com | SaaS; moved upmarket in 2026 |
| Otterly.AI Lite / Standard / Premium / Pro | AI SEO/GEO | $29 / $189 / $489 / $989 mo | SMB → mid-market | "Track brand mentions + cited URLs across 6 AI engines" | otterly.ai/pricing | SaaS; lowest priced public tool |
| Peec AI Starter / Pro / Advanced | AI SEO/GEO | $95 / $245 / $495 mo | Marketing teams + SEO agencies | "AI search analytics, 50–350 prompts × 3 models" | peec.ai/pricing | SaaS |
| Scrunch AI (Agency / Business) | AI SEO/GEO | from $300/mo | Agencies | "GEO/AEO monitoring across 7+ AI engines" | scrunch.com | SaaS |
| Goodie AI Pro | AI SEO/GEO | $495/mo | Brands | "Enterprise GEO monitoring" | higoodie.com | SaaS |
| Bluefish AI | AI SEO/GEO | contact sales (invite only) | Fortune 500 | "Agentic marketing platform across all major AI engines" | bluefishai.com | Gated enterprise |
| One-time GEO audit (typical agency) | AI SEO/GEO | $1,500–$7,500 one-time | Brand marketing leads | "10-prompt audit → 5-platform engagement" | thedigitalelevator.com · soar.sh | Service offering |
| AI Labs Audit (SEO/AEO/GEO) | AI SEO/GEO | $149 one-time | SMBs | "260+ checks across 7 categories, 3-day turnaround" | ailabsaudit.com | Productized service; rare low-price entry |
| GEO retainer (mid-market) | AI SEO/GEO | $2,000–$10,000/mo | Mid-market marketers | "Ongoing AEO/GEO content + monitoring" | thedigitalelevator.com | Service |

### RAG / eval tooling

| Product | Category | Price | Buyer | Promise | Link | Notes |
|---|---|---:|---|---|---|---|
| Confident AI (Starter / Premium / Team) | RAG/eval | $19.99 / $79.99 per user/mo + custom | LLM teams using DeepEval | "Full eval suite, custom metrics, online evals, CI/CD" | confident-ai.com/pricing | SaaS; DeepEval is free OSS |
| DeepEval (OSS) | RAG/eval | Free (Apache-2.0) | Devs | "LLM eval framework, RAGAS metrics included" | deepeval.com | OSS — funnel into Confident AI |
| Patronus AI (Base / Enterprise) | RAG/eval | $25/mo / custom | Enterprises | "Automated eval/monitoring for LLM systems & agents" | patronus.ai | SaaS |
| Ragas | RAG/eval | Free (OSS) | RAG builders | "Faithfulness, answer relevancy, context precision metrics" | ragas.io | OSS; no paid tier |
| TruLens | RAG/eval | Free (MIT) / Snowflake enterprise | RAG/agent teams | "OTel traces + built-in eval metrics" | trulens.org | OSS + enterprise-gated |

### Agent observability

| Product | Category | Price | Buyer | Promise | Link | Notes |
|---|---|---:|---|---|---|---|
| Langfuse Core / Pro / Enterprise | Agent observability | $29 / $199 / $2,499 mo | Indie → mid-market → enterprise | "Tracing, evals, prompts, datasets" | langfuse.com/pricing | SaaS + OSS self-host |
| LangSmith Plus / Enterprise | Agent observability | $39/seat/mo + $2.50/1k traces over 10k | LangChain teams | "Tracing, evals, prompt mgmt" | langchain.com/pricing | SaaS; per-seat |
| Braintrust Pro / Enterprise | Agent observability | $249/mo flat / custom | Eval-heavy teams | "Unlimited seats, 5GB processed, 50k scores" | braintrust.dev/pricing | SaaS; no per-seat |
| Helicone Pro / Team / Enterprise | Agent observability | $79 / $799 / custom mo | API/LLM ops | "Unlimited seats, alerts, HQL, 1-month retention" | helicone.ai/pricing | SaaS |
| Arize Phoenix (AX Pro / Enterprise) | Agent observability | $50/mo / custom | LLM app teams | "50k spans, 10GB, 15-day retention; OSS Phoenix free" | phoenix.arize.com/pricing | SaaS + OSS |
| Galileo Pro / Enterprise | Agent observability | $100/mo / custom | AI app teams | "50K traces, RBAC, advanced analytics" | galileo.ai/pricing | SaaS; Cisco acquired May 2026 |
| Maxim AI Pro / Business / Enterprise | Agent observability | $29 / $49/seat/mo / custom | Devs shipping agents | "Eval + observability, prompt experiments, agent sim" | getmaxim.ai/pricing | SaaS; cheapest per-seat |
| Logfire (Pydantic) | Agent observability | Free 10M spans / $2 per 1M after | Python devs | "OTel-native, no seat fees" | pydantic.dev | SaaS; usage-only |

### AI infra templates

| Product | Category | Price | Buyer | Promise | Link | Notes |
|---|---|---:|---|---|---|---|
| ShipFast | AI infra templates | $199 one-time | Indie founders | "Idea to deployed SaaS in <1 day; Stripe + Clerk + Next.js" | shipfa.st | Template; lifetime |
| Makerkit (Pro / Teams) | AI infra templates | $349 / $649 lifetime | Solo → small team | "Production-ready Next.js SaaS w/ multi-tenancy, billing, auth" | makerkit.dev | Template |
| supastarter (Next.js) | AI infra templates | $299–$349 | B2B teams | "Next.js + Supabase, multi-tenancy, i18n, RBAC, 5 payment providers" | supastarter.dev | Template |
| Next.js + Supabase SaaS Starter (ajraou) | AI infra templates | ~$49–$79 | Indie devs | "Next.js 14, Supabase auth, Tailwind, dashboard + landing" | ajraou.gumroad.com/l/nextjs-saas-starter | Template |
| Plug & Play Express + Supabase Boilerplate | AI infra templates | ~$15–$29 | Solo devs | "JWT auth, CRUD factory, clean structure" | youssufsolodev.gumroad.com/l/api-boilerplate | Template |
| Cloudflare agents-starter | AI infra templates | Free (only Neurons) | Cloudflare devs | "Chat agent w/ tools, scheduling, vision on Workers AI" | github.com/cloudflare/agents-starter | OSS template |
| Vercel AI Templates / Chatbot starter | AI infra templates | Free (Vercel Pro $20/user/mo) | Next.js devs | "Hackable Next.js AI chatbot, swap providers" | vercel.com/templates/ai | OSS; monetized via hosting |
| n8n Ultimate Templates (Usama) | AI infra templates | $30 (anchored $100) | Automation builders | "4,000+ ready-to-use n8n + AI agent workflows" | usamaakrm.gumroad.com/l/n8n-templates | Info/template |
| n8n Automation Megapack (vfocus) | AI infra templates | ~$27–$47 | Operators | "261 curated automation templates" | vfocus.gumroad.com/l/mrjajc | Info/template |

### Pricing pattern read

- **Modal price by category**
  - AI skill packs: **$17–$29 one-time** (Gumroad info-product band); marketplace per-skill $5–$50.
  - MCP products: **Free OSS** dominates; paid offerings are gated enterprise gateways (no public price).
  - AI SEO/GEO audits: SaaS modal **$189–$495/mo**; one-time audits cluster **$1,500–$5,000**; retainers **$2,000–$10,000/mo**.
  - RAG/eval tooling: free OSS + SaaS at **$20–$80/seat/mo** entry, enterprise custom.
  - Agent observability: entry SaaS **$29–$100/mo**, team **$199–$799/mo**, enterprise **$2,499/mo+**.
  - AI infra templates: **$199–$349 one-time lifetime** is gravity (ShipFast/Makerkit/supastarter); Gumroad indie $15–$79.

- **Info-product band ($29–$199):** AI skill packs, Cursor rules packs, n8n template packs, Gumroad SaaS boilerplates, low-end infra templates.
- **Mid-tier SaaS band ($20–$200/mo):** agent observability entry tiers (Langfuse Core, LangSmith Plus, Maxim Pro, Helicone Pro, Galileo Pro, Arize AX Pro), GEO monitoring entry (Otterly Standard, Peec Starter), RAG eval entry (Confident AI Starter, Patronus Base).
- **Service-priced band ($500–$5k+):** GEO/AEO one-time audits ($1.5k–$7.5k), agent security audits ($500–$2k pre-implementation, $3k–$15k compliance scope), GEO retainers ($2k–$10k/mo).

- **White space — no clear paid offerings**
  - **Paid MCP starter kits / MCP security audit packs**: every named MCP boilerplate is free/OSS; enterprise gateways are sales-led. A productized "MCP security audit" at $499–$2,999 has no obvious incumbent — **strong white space**.
  - **AI-citation (GEO) audit as a $99–$999 productized one-off**: the $149 SEOscore product is the only sub-$500 example; everything else is $1.5k+ service or $189+/mo SaaS. A $299–$799 one-time GEO audit is largely uncontested.
  - **RAG eval kits as one-time downloadables**: dominated by OSS + SaaS. A "RAG eval kit / harness" at $99–$299 has no clear seller.
  - **Agent observability info-products**: zero — entire category is SaaS-only.
  - **Productized agent security audits at $999–$5k**: only general pre-implementation pricing exists; no named productized offer.

- **Refund norms:** Gumroad/Lemon Squeezy default to 30-day refund window unless seller opts out; SaaS = no refunds, cancel-anytime; boilerplates (ShipFast, Makerkit, supastarter) = no refunds once downloaded; GEO audits = pay-on-delivery; enterprise = annual contracts, no public refund clauses.

---

## 3. Marketplace Signals

| Platform | Search term | Count/examples | Notable winners | Gap |
|---|---|---:|---|---|
| GitHub | `mcp-server` topic | ~14,000+ MCP servers ecosystem-wide; modelcontextprotocol/servers ~79K stars | modelcontextprotocol/servers, github/github-mcp-server, punkpeye/awesome-mcp-servers, microsoft/mcp, mcpdotdirect/template-mcp-server | Polished commercial MCP templates (auth, billing, observability baked in) — most repos are bare scaffolds |
| GitHub | `MCP server template` | Dozens of templates | mcpdotdirect/template-mcp-server, mclenhard/mcp-server-template, Next.js MCP template, FastMCP template | Vertical templates (legal, healthcare, finance MCPs) with compliance docs |
| GitHub | `agent memory` / `Mem0` | mem0ai/mem0 ~48–52K stars | mem0ai/mem0, rohitg00/agentmemory, NirDiamant/Agent_Memory_Techniques | Production-ready memory eval kits with benchmarks pre-wired |
| GitHub | `RAG eval` / `RAG evaluation` | 10+ active frameworks; RAGAS dominant | RAGAS, vectara/open-rag-eval, YHPeter/Awesome-RAG-Evaluation | Turnkey "drop-in eval kit for your RAG stack" with prebuilt dashboards |
| GitHub | `prompt injection` / `AI agent security` | 78-study meta-analysis 2021-2026; multiple toolkits | liu00222/Open-Prompt-Injection (447★), Vigil (480★), OpenClaw AI Red Teaming | Productized audit-as-a-service for SMB teams; OSS exists, packaged audits do not |
| GitHub | `claude skills` / `claude-code-skills` | 1000+ skills aggregated | alirezarezvani/claude-skills (329), anthropics/skills, ComposioHQ/awesome-claude-skills | Curated paid vertical bundles (e.g., "GEO audit skill pack") |
| Docker MCP Catalog | MCP servers | 300+ verified servers; ~97M monthly SDK downloads (Mar 2026) | Playwright (1M+ dl), Grafana (500K+ dl), Brave Search (100K+ dl), Context7, Desktop Commander, MongoDB, Notion, GitHub Official, AWS Core | No "audit/security/eval" focused MCP servers in top tier — open slot |
| Vercel Templates | AI / chatbot / RAG | `/templates/ai` 403 to scraper; AI SDK 74% framework share | Vercel AI Chatbot, ai-sdk-rag (Drizzle+Postgres), azure-ai-rag-chatbot, mongodb-rag-app, LangChain+Next.js | Paid premium agent templates — Vercel templates are nearly all free; no eval/security templates visible |
| Supabase | pgvector / AI starters | Handful of official examples | Headless Vector Search, Next.js Vector Search, Image Search w/ CLIP, HuggingFace Inference, OpenAI Completions Edge Function | Supabase + MCP server combo starter; auth-gated RAG eval starter |
| Product Hunt | MCP / AI agents (last 60d) | Active daily launches | Agentation (434 upvotes, #1 PoD), CraftBot (263), Cloudflare Site Agent-Ready (252), Weavable (233), Superlines (332 — AI SEO) | GEO/AI-citation tools launching but few audit-deliverable products |
| Product Hunt | RAG / AI SEO / GEO | Cluster of 2026 launches | Superlines (332), Profound, Gauge, Otterly AI, Geoptie | One-off paid audit reports ($99–$999); current tools are subscription SaaS |
| Gumroad | AI prompt/skill packs | Hundreds of listings; bestseller category | Prompt Pack 365 2026, Art of ChatGPT (6,288+ buyers), PromptPack (5K+ prompts), Claude Code + Antigravity skill packs (launched May 2026) | Developer-grade skill/MCP packs at $99–$999 — most inventory is $19–$79 consumer prompts |
| Lemon Squeezy | AI templates / dev kits | Active but no public bestseller list; $19–$79 typical | themes.lemonsqueezy.com directory, SaaS boilerplates index, uiPress case (600% sales lift) | Mid-priced ($199–$499) MCP/agent dev kits |
| Stripe seller pages | Direct payment links | No public marketplace; Agentic Commerce Suite launched 2026 | Stripe Link wallet for AI agents, Machine Payments Protocol | N/A — Stripe is rails, not a marketplace |
| Claude marketplaces | Paid Claude skills | 8 major marketplaces by Q2 2026; ClaudeSkills.ai (90% to seller); ClaudeSkills.info (658+ free); Agent37, SkillsMP, KissMySkills | Agent37 (one-day skill-to-product), KissMySkills, ClaudeSkills.ai | Auth-walled on listings; emerging paid layer — RAG/security/GEO niches mostly unfilled |
| Cursor community | Paid templates/workflows | No native paid marketplace; MCP integrations free | Pro/Pro+ tiers include MCP/skills/hooks; no template storefront | Big distribution gap — no native paid pack channel |
| Codex / agent-security launches | Audit tools | Microsoft RAMPART + Clarity + Agent Governance Toolkit (OSS, Apr-May 2026); Alter (zero-trust); Winfunc (AI pentest) | RAMPART, Clarity, Mindgard, Alter, Winfunc | Productized one-shot audit reports for $99–$999 — current vendors are enterprise SaaS |

### Marketplace gap synthesis

**Demand-side activity loudest:** GitHub (mem0 ~50K stars, ~14K MCP servers, ~97M monthly MCP SDK downloads), Docker MCP Catalog (Playwright 1M+ downloads), Product Hunt where MCP/agent-context launches routinely clear 200+ upvotes (Agentation 434, Superlines 332, CraftBot 263). Buyers are present and the GEO/AI-citation lane is actively forming (Superlines, Profound, Gauge, Otterly, Azoma, Wellows).

**Supply gap widest** for: (a) paid RAG eval kits and agent-security audit deliverables — OSS exists (RAGAS, Vigil, RAMPART) but no one is selling a packaged $199–$499 audit report; (b) vertical Claude skill bundles in the security/GEO/RAG lanes — claudeskills.info has 658+ free skills but paid niche packs are sparse; (c) Cursor has no paid pack channel at all.

**Fastest distribution lever for a solo seller this week:** Claude skills marketplaces — specifically ClaudeSkills.ai (Stripe Connect, 90% to seller, no infra) paired with a Product Hunt launch and a Gumroad fallback. The agent-skill ecosystem grew from 1 to 8 marketplaces in ~6 months and pricing norms are still being set, so first-movers in security/GEO/RAG-eval niches can anchor the $99–$999 bracket before incumbents arrive.

> *Access notes: vercel.com/templates/ai, producthunt.com category pages, claudeskills.ai, and claudemarketplaces.com all returned 403 to scraping — data above is from search-result snippets and aggregator sites (hunted.space, agensi.io, agent37.com). Treat counts as directional, not exact.*

---

## 4. Community Pain Quotes

| Source | Quote/paraphrase | Pain | Product idea |
|---|---|---|---|
| [GitHub modelcontextprotocol#205](https://github.com/modelcontextprotocol/modelcontextprotocol/issues/205) | "Every MCP server developer needs to implement the discovery, registration, authorization and token endpoints." | Building a production MCP server forces you to re-implement an entire OAuth authorization server; spec is solid but unworkable for solo devs. | MCP Server Builder |
| [GitHub open-webui#14121](https://github.com/open-webui/open-webui/discussions/14121) | "A single MCP client instance is shared across all OpenWebUI users, resulting in a shared authentication context." | No per-user auth flow — every user ends up using the same credentials, blocking real multi-tenant deployments. | MCP Server Builder |
| [GitHub LibreChat#12564](https://github.com/danny-avila/LibreChat/discussions/12564) | "The connection fails permanently with `invalid_token` until the tokens expire by TTL in the database." | Token recovery in MCP OAuth is broken — no manual re-auth path, users get permanently locked out. | MCP Server Builder |
| [HN Ask: What did you hate building an MCP server](https://news.ycombinator.com/item?id=44519400) | Paraphrase: "Anthropic's low-level server felt too low-level" — devs say the SDK forces them to write boilerplate that should be one decorator. | Reference SDK abstraction too thin; people want a higher-level builder. | MCP Server Builder |
| [HN: Manually discovering MCP servers](https://news.ycombinator.com/item?id=44756018) | Paraphrase: "Manually searching for MCP servers, reading docs, and configuring them feels time-consuming and not 'agentic'." | No usable marketplace/discovery layer — install UX is still copy-paste JSON. | MCP Server Builder |
| [Medium: Why your MCP server is a security disaster](https://medium.com/data-science-collective/why-your-mcp-server-is-a-security-disaster-waiting-to-happen-660577d8077c) | Paraphrase: dev spent 4 hours on RFC 9728 / PKCE, shelved auth work, shipped with a static API key — Astrix found 53% of 5,200 MCP servers do the same. | Proper MCP auth is a months-long backend project; ecosystem is silently insecure. | MCP Server Builder |
| [HN: Prompt injection via tool descriptions / MCP Guardian](https://news.ycombinator.com/item?id=47075424) | Paraphrase: "MCP tool descriptions are invisible to users but function as instructions to the LLM — a tool can contain hidden text the LLM follows because it can't distinguish them from legitimate ones." | Tool-description injection is a real attack surface and nobody scans MCPs at install time. | Agent Security |
| [HN Ask: state of multimodal prompt injection defence 2026](https://news.ycombinator.com/item?id=47689822) | Paraphrase from OP: "Most tools like Lakera Guard, LLM Guard, and Azure Prompt Shields are still text-only — there haven't been many production-grade defences for image/audio/document injection." | Buyers actively asking "what tool should I use?" for multimodal injection and finding the market empty. | Agent Security |
| [HN: Remote MCP servers can do prompt injection](https://news.ycombinator.com/item?id=44019225) | Paraphrase from thread: developers warning that remote MCPs can instruct a local agent to exfiltrate data, and no client today blocks it. | Agent exfiltration via remote tool calls is a known unsolved risk. | Agent Security |
| [Microsoft Security Blog, May 2026](https://www.microsoft.com/en-us/security/blog/2026/05/07/prompts-become-shells-rce-vulnerabilities-ai-agent-frameworks/) | Paraphrase: RCE chains in LangChain, AutoGen, CrewAI reachable via indirect prompt injection — argues for "argument separators, capability brokers, and runtime sandboxes." | "We don't have a safe default sandbox" is a recurring complaint. | Agent Security |
| [HN: Show Runtime Defense Against Prompt Injection in Supabase MCP](https://news.ycombinator.com/item?id=44649167) | Paraphrase: Supabase users in comments said "I had no idea a service-role MCP could be tricked into dumping the whole DB" until the Trail of Bits writeup. | Buyers admit they did not understand the blast radius of agent tool permissions. | Agent Security |
| [HN Ask: MCP server for long-term memory?](https://news.ycombinator.com/item?id=44442810) | OP paraphrase: "I want an MCP server that gives Claude long-term memory across sessions — what are people actually using?" Top reply: "I just tell Claude to maintain its own memories in a collection of markdown files via CLAUDE.md." | Current answer is duct-tape; users explicitly asking for a real persistent memory product. | Memory Pack |
| [GitHub mem0ai/mem0](https://github.com/mem0ai/mem0) | Repo tagline + tracker: "Universal memory layer for AI Agents" — 30k+ stars, hundreds of issues asking for cross-app sync, user-level memory controls, selective forgetting. | Mass demand signal: people pulling memory packages because base assistants forget. | Memory Pack |
| [GitHub NousResearch/hermes-agent#3943](https://github.com/NousResearch/hermes-agent/issues/3943) | Paraphrase: "Cross-agent memory is a gap — if a developer uses Hermes for some tasks and Claude Code or Cursor for others, the memory is split." | Users want one memory pack that follows them across Claude, Cursor, ChatGPT — none exists. | Memory Pack |
| [Atlan: Best AI Agent Memory Frameworks 2026](https://atlan.com/know/best-ai-agent-memory-frameworks-2026/) | Paraphrase: community is shopping — "Choose Mem0 for personalization, Zep for temporal, Letta for long-running" — but no consensus winner. | Buyer in active comparison mode; market fragmented. | Memory Pack |
| [GitHub gastownhall/beads](https://github.com/gastownhall/beads) | Repo pitch: "A memory upgrade for your coding agent" replacing "messy markdown plans with a dependency-aware graph." | Validates "markdown plan that the agent re-reads" is the current bad-but-default solution. | Memory Pack |
| [GitHub vectara/open-rag-eval](https://github.com/vectara/open-rag-eval) | Project tagline: "RAG evaluation without 'golden answers'" — README cites that "building a golden dataset is the #1 blocker our customers report." | Golden-dataset construction is the explicit pain people open-source around. | RAG Regression |
| [GitHub community#182015 (LangChain bloat)](https://github.com/orgs/community/discussions/182015) | "It's slower, bloated, and has bugs that are known but still have not been fixed." | Devs frustrated with the dominant RAG stack; receptive to a leaner eval/regression tool. | RAG Regression |
| [arXiv 2511.04502 — RAGalyst](https://arxiv.org/pdf/2511.04502) | Paraphrase: "Existing evaluation frameworks rely on heuristic-based metrics that fail to capture domain-specific nuances." | Domain-specific RAG eval unsolved — buyers in regulated industries actively shopping. | RAG Regression |
| [Towards AI: Why Most RAG Projects Fail in Production](https://towardsai.net/p/machine-learning/why-most-rag-projects-fail-in-production-and-how-to-build-one-that-doesnt) | Paraphrase: "Pipelines that work in notebooks often collapse in production. Without evaluation, RAG becomes guess-and-ship." | "Guess-and-ship" is exact buyer pain language for a regression product. | RAG Regression |
| [Braintrust: Best RAG Evaluation Tools in 2026](https://www.braintrust.dev/articles/best-rag-evaluation-tools) | Paraphrase: "You need evaluation loops, feedback workflows, regression tests, and A/B experiments so improvements do not introduce new failures." | Confirms "RAG regression" as a named category buyers are actively googling. | RAG Regression |
| [ReddiReach: ChatGPT Recommends Competitors (2026)](https://www.reddireach.com/blog/why-chatgpt-recommends-your-competitors) | Paraphrase from SaaS founders quoted: "Your competitor's three-month-old r/sysadmin comment can become the entire foundation of how ChatGPT describes your product category for the next six months." | Concrete, measurable bleeding — pipeline loss attributed to AI recommendation bias. | AI Citation |
| [Medium: Startup Guide to AEO & GEO 2026](https://medium.com/@oleksii_citedme/your-startups-guide-to-aeo-geo-in-2026-429c799e68b5) | Paraphrase: "Nearly half of B2B buyers now start vendor research by asking AI rather than searching Google — if you're invisible in AI answers, you miss half your potential pipeline." | Founders publicly asking how to audit/fix AI visibility. | AI Citation |
| [HubSpot AEO Grader](https://www.hubspot.com/aeo-grader/share-of-voice) | Product page existence is the signal: HubSpot built a free Share-of-Voice grader because customers were demanding it. | Top-of-funnel demand validated by incumbent putting a free tool out. | AI Citation |
| [Sona: Best LLM SEO Tracker Tools 2026](https://www.sona.com/blog/best-llm-seo-tracker-tools-in-2026-compared) | Paraphrase: "Reddit discussion in r/AIToolTesting confirms strong community demand for affordable LLM SEO tracking, with real users validating the $39–$79/mo tier as the practical entry point." | Buyers naming a price they will pay — clearest "I would pay for this" signal in the dataset. | AI Citation |
| [Alex Birkett: How to Measure AI Share of Voice](https://alexbirkett.com/ai-share-of-voice/) | Paraphrase from comments: "I run a fixed list of 15–20 queries weekly and record which week a competitor replaces me." | Marketers stitching their own GEO audits — SaaS gap. | AI Citation |
| [Academy of AI: 10 Claude Prompts That Pay Daily](https://academyofai.substack.com/p/claude-prompts-that-pay-everyday) | Paraphrase from comments: creators reporting "$19 AI Resume Booster Pack," "$1,500/mo from Freelancer Workflow Prompts" — no native distribution channel for Claude Skills specifically. | People monetizing prompts on Gumroad/PromptBase but Claude Skills format has no marketplace. | Skill Pack Builder |
| [Medium: I Built 17 Claude Skills That Make Money](https://medium.com/write-a-catalyst/i-built-17-claude-skills-that-actually-make-money-fe58cc4ad37c) | Paraphrase: "Building small, specific skills... has resulted in consistent, boring, real money." Author distributes via personal Gumroad — laments lack of a Claude-native store. | Direct buyer language: "I would pay to skip building this skill myself." | Skill Pack Builder |
| [HowDoIUseAI: Turn Claude Skills into Revenue](https://www.howdoiuseai.com/blog/2026-03-11-how-to-turn-claude-skills-into-revenue-generating-) | Paraphrase: "Selling files gives away your IP the moment someone downloads them... hosted access is the path forward." | Sellers explicitly asking for a hosted/licensed Skill Pack runtime — the missing product. | Skill Pack Builder |
| [PromptBase Alternatives 2026](https://medium.com/@divyaptr/7-alternatives-to-promptbase-to-buy-or-sell-ai-prompts-13dea4d1cb6) | Paraphrase: PromptBase takes 20%, Prompthero 30%; sellers grumbling about fees and lack of Claude Skill format support. | Mature market, unhappy sellers — wedge for a Claude-Skills-native marketplace. | Skill Pack Builder |
| [The Neuron: Claude Design launched, Reddit thoughts](https://www.theneurondaily.com/p/anthropic-s-claude-design-launched-and-reddit-has-thoughts) | Paraphrase of r/ClaudeAI reaction: "every generated app looks identical... container soup of pills and cards" — users say the built-in frontend-design skill needs alternatives. | Concrete demand for third-party Skill Packs to replace Anthropic defaults. | Skill Pack Builder |
| [Instantprompts: Best AI Prompt Marketplaces 2026](https://instantprompts.com/blog/best-ai-prompt-marketplaces-and-tools-in-2026-definitive.html) | Paraphrase: market guide notes "prices range from $1 for simple text prompts to $500+ for complex multi-step workflows" — high end is the Skill Pack opportunity. | Validates $500 price point exists for packaged AI workflows. | Skill Pack Builder |

### Pain heat map (hottest → coldest)

1. **MCP Server Builder — HOTTEST.** Every single source has a named, reproducible blocker (OAuth, multi-tenant, token recovery, discovery). HN, GitHub, and dev blogs converge on the same pain. 53% of 5,200 production servers silently shipped insecure — a quantified market.
2. **Agent Security.** Active "what tool should I use?" questions on HN about multimodal injection, MCP tool-description attacks, and Trail of Bits / Microsoft writeups generating ongoing comment threads. Pain real, defense market fragmenting fast — second only because buyers are still figuring out what to buy.
3. **AI Citation (GEO).** Buyers naming dollar prices they'll pay ($39–$79/mo) and incumbent (HubSpot) shipping a free tool — clearest commercial intent. Slightly cooler than #2 because the "tool" answer is already crowded (AIclicks, LLMrefs, Octolens, Waikay).
4. **Memory Pack.** Strong "I want X" signal (Ask HN long-term memory, Hermes cross-agent memory issue), but Mem0/Zep/Letta already absorbing demand. Hot, partially served.
5. **RAG Regression.** Devs articulate well ("guess-and-ship," "collapses in production"), but discussion is in research papers and vendor blogs — fewer raw "help me" posts. Ragas, LangSmith, Braintrust already named.
6. **Skill Pack Builder — COLDEST.** Real revenue stories exist on Gumroad/PromptBase, but few are loudly asking "where do I buy Claude Skills?" The pain is mostly seller-side (no native marketplace) rather than buyer-side demand.

---

## 5. LBC Asset Readiness

### 5a. Asset inventory

> **Hard finding:** This repo (`dirtylogic/yoyo`, branch `claude/lbc-market-research-pull-fdG3p`) contains only `README.md` (6 bytes — single line `# yoyo`). None of the named LBC assets — PAL, ARL, MCP Server Builder, Memory Pack, landing page, Stripe links, fulfillment scripts — are present in this repository. Statuses below default to **"unknown — not in this repo"** unless the user confirms otherwise from a separate workspace.

| Asset | Status (verified in this repo) | Blocker | Next action |
|---|---|---|---|
| PAL zip | Not in repo — status unknown | Need to locate authoritative copy; confirm final filename, version, license, refund policy stub | Have David point me at the source folder OR re-upload to a `/assets/pal/` path on this branch |
| ARL zip | Not in repo — status unknown | Same as PAL | Same |
| MCP Server Builder zip | Not in repo — status unknown | Same; also need to define what the zip ships (template? installable npm/pip pkg? docker?) | Decide deliverable format before packaging — see Section 7 recommendation |
| Memory Pack zip | Not in repo — status unknown | Same | Same |
| Landing page draft | Not in repo | No URL, no copy, no platform commit (Webflow / Framer / Next.js?) | Pick platform → 1-page copy + Stripe button. Recommended: Framer or single Next.js page on Vercel free tier. Same-day shippable |
| Stripe links | Not in repo | Stripe products / prices not yet created (no env vars, no markdown stubs) | Create one Stripe product per launched SKU with two prices ($X regular, $Y founder discount); generate Payment Links; no checkout integration needed for v1 |
| Fulfillment mechanism | Not in repo | No script, no signed URL setup | Pick one: (a) Stripe receipt email → manual Gumroad-style upload, (b) R2 + signed URL via webhook, (c) Lemon Squeezy as full storefront (simplest). Recommended: Lemon Squeezy for v1 — kills R2/signed-URL/webhook engineering entirely |
| Domain | Not in repo | Unknown — no DNS records committed; no purchase receipt visible | Suggest registering a single short domain (e.g. `<lbc-brand>.com`) on Cloudflare Registrar; point at Vercel/Framer landing |
| Support email | Not in repo | Need address (likely `support@<domain>`) | Configure once domain is live — Cloudflare Email Routing → `djpjronline@gmail.com` is the zero-cost path |
| Terms / refund / privacy | Not in repo | No legal copy of any kind | Use a standard generator (e.g., GetTerms, Termly) for v1; tighten for vendor-marketplace SKU per Section 5c |
| Operator packs (PAL / ARL / etc.) — source masters | Not in repo | Unknown location | Confirm — if these exist they live in a different repo or in David's local drive |

**Conclusion on readiness:** the literal "what can ship from THIS branch this week" answer is **nothing without an upload step.** David needs to either (a) add the existing zip files / landing copy to this repo as a one-shot commit, or (b) confirm they live elsewhere (Google Drive, a different repo, local disk) and reroute the publish pipeline accordingly. The fastest path is option (b) + Lemon Squeezy storefront — bypasses all packaging engineering and gets to "Stripe link goes live" in hours instead of days.

### 5b. Audience and distribution data

> No analytics, follower counts, or email-list metadata are available from inside this repo. The table below is the **schema David should populate from his own dashboards**; verified data points are noted where derivable from public sources (e.g., LinkedIn profile counts).

| Channel | Needed metric | Status | Source / action |
|---|---|---|---|
| LinkedIn | Followers, average post views, top 3 recent posts, AI/dev/RE relevant connections count | **Unknown — pull from LinkedIn analytics** | David: export "Followers" + "Analytics" tab CSV |
| X / Twitter | Followers, 30-day avg impressions, AI-adjacent overlap | **Unknown — pull from X analytics** | David: export X Premium Analytics or analytics.twitter.com |
| Email list | List size, last 30-day open rate, top source | **Unknown — depends on ESP (Mailchimp / Beehiiv / ConvertKit?)** | David: confirm ESP + share sender metrics |
| Website analytics | Monthly uniques, top 5 pages, top referrals | **No website confirmed in repo** | David: confirm whether a landing/blog exists already + what analytics is wired |
| GitHub | Stars on personal repos, profile views, recent commit activity | **Unknown — point me at GitHub handle** | David: share GitHub username — I can pull counts |
| Communities | Where David is non-spammy: Indie Hackers, AI Tinkerers, Lenny's Slack, Founder Cafe, r/Entrepreneur, MCP Discord, etc. | **Unknown** | David: list 3–5 communities where he has standing |
| Existing client network | Headcount of past consulting/agency clients reachable for warm outreach | **Unknown — likely David's CRM/Notion** | David: count or share an anonymized list |

**Distribution lever ranking for week-1 launch** (independent of David's specific numbers, based on the marketplace research above):
1. **ClaudeSkills.ai listing** — Stripe Connect, 90% to seller, zero infra (1 hour)
2. **Product Hunt launch** — best for the MCP Server Builder and GEO Audit SKUs (1 day prep)
3. **Direct LinkedIn outreach** to the 30 buyer-grade prospects in Section 6 (3 days)
4. **Twitter/X thread** showing real before/after of the MCP Builder solving the OAuth pain in Section 4 (1 day)
5. **Indie Hackers + AI Tinkerers + Hacker News Show HN** for the MCP Server Builder + Agent Security audit specifically (1 day each, staggered)
6. **Email list / newsletter swap** with one of the warm amplifiers in Section 6 (Greg Isenberg, Ben Tossell, Channing Allen, Joe Heitzeberg)

### 5c. Compliance gating (real-estate / vendor-network SKUs only)

Tagging per the active compliance memo. Apply ONLY to the proptech / Real Estate Vendor Marketplace Kit and any "MCP for Local Business Automation" SKU touching real-estate settlement services. The general AI/MCP/RAG/GEO line is **not** compliance-gated.

| SKU / direction | Tag | Notes |
|---|---|---|
| AI Citation Operator Pack / GEO audit / GEO retainer | **Clean now** | Standard marketing-services billing. No referral or steering involved. |
| MCP Server Builder / Agent Security Audit / RAG Regression Pack / Memory Pack / Production AI Shipping Bundle | **Clean now** | SaaS / template / audit / info product. No regulated industry exposure unless explicitly sold into title/escrow/lender clients — in which case re-tag the specific deal as Counsel gate. |
| Real Estate Vendor Marketplace Kit — **platform access fee model** | **Clean now** | Flat monthly platform fee charged to vendors for listing/profile/lead-routing tools. Disclose openly. |
| Vendor Marketplace Kit — **workflow coordination fee** | **Clean now** | Per-job coordination fee for actual technology work performed (scheduling, comms, doc routing). Document the work. |
| Vendor Marketplace Kit — **verified vendor marketplace fee** | **Clean now** | Subscription for vendors to appear on a vetted directory; pay-to-list is allowed when the platform performs vetting work. |
| Vendor Marketplace Kit — **bona fide service fees** | **Clean now** | Fee tied to a real, documentable service rendered. Document the deliverable per transaction. |
| Vendor Marketplace Kit — **data integration revenue** | **Clean now** | Licensing data feeds (vendor coverage, pricing, lead-time) to brokers/MLS. |
| Vendor Marketplace Kit — **licensed-service compensation** | **Counsel gate** | Only where state license permits; needs counsel sign-off per state. |
| Vendor Marketplace Kit — **disclosed transaction administration fees** | **Counsel gate** | Disclosed-to-consumer admin fees; jurisdiction-dependent; counsel review. |
| Title / escrow / insurance / lender / appraisal — anything inside RESPA Section 8 scope | **Counsel gate** | Any monetization touching settlement services must clear counsel before launch. Per-transaction or per-referral economics are the trigger. |
| Hidden per-transaction steering / unmarked kickbacks / undisclosed bundling | **AVOID** | Do not ship. Period. |
| "Referral fee" framing of any kind without RESPA counsel clearance | **AVOID** | Even informally on a sales page, social post, or pitch deck. |

**Operational rule for week-1 launches:** ship the Clean-now SKUs (everything in the general AI line + the platform-access / workflow-coordination / verified-vendor / data-integration variants of the Vendor Marketplace Kit) and **hold every Counsel-gate SKU** until counsel sign-off. This isolates compliance risk to one specific lane without blocking the cash launch.

---

## 6. Prospect List

| # | Name | Company | Role | Contact | Buyer category | Pain likely | Best-fit product | Why they might buy | Warm/cold | Outreach angle |
|---:|---|---|---|---|---|---|---|---|---|---|
| 1 | Yusuf Hashlamoun | Independent | Founder, AI Automation Agency | [LinkedIn](https://www.linkedin.com/in/yusuf-hashlamoun-394130391) | AI automation agency | Reselling generic n8n/Make builds; thin margins | MCP Builder + Security + Observability | Needs a productized differentiator beyond "we build automations" | Cold | "Most AAA founders ship n8n flows — here's how to ship MCP servers and charge 5x." |
| 2 | Sam Poutakidis | AI Automation Agency | Founder | [LinkedIn](https://www.linkedin.com/in/sampoutakidis/) | AI automation agency | Client retention; needs recurring observability story | MCP Builder + Observability | New AAA; will need a "post-build" SKU to keep retainers | Cold | "Your AAA needs a Phase 2 SKU — observability for the agents you already shipped." |
| 3 | Denis Popa | AAAgency | Founder | [LinkedIn](https://es.linkedin.com/in/denis-popa) | AI automation agency | Scaling delivery without hiring | MCP Builder, Security | EU-based AAA, target market loves "secure" framing | Cold | "EU buyers want SOC-style answers for agents — MCP security pack." |
| 4 | Sandro Kashibadze | AI automation agency | Founder | [LinkedIn](https://ge.linkedin.com/in/sandro-kashibadze-020481311) | AI automation agency | Small team, needs templated offering | MCP Builder | Early-stage agency, ideal $99–$299 entry-point | Cold | "Junior AAA founders: a $299 MCP starter kit that lets you bill $5k." |
| 5 | Alejandro Laking-Jerez | AI Automation Agency | Co-founder | [LinkedIn](https://uk.linkedin.com/in/alejandro-laking-jerez-4654441ab) | AI automation agency | UK SMB sales motion | MCP for Local Business Automation | UK SMB clients want plumbing/dental booking agents | Cold | "Local business MCP pack — drop into any UK SMB client in a day." |
| 6 | Joshua Leavitt | Omni AI | AI & Automation Agency CEO | [LinkedIn](https://www.linkedin.com/in/your-profile-joshua-leavitt-omni) | AI automation agency | Differentiation vs commoditized AAA pool | Production AI Shipping Bundle | Brands himself as CEO-tier; will buy "production" framing | Cold | "Stop selling chatbots; sell shipped production agents." |
| 7 | Wesley Gamble | AI Automation Agency | Owner | [LinkedIn](https://www.linkedin.com/in/wesley-gamble-bb37b532a) | AI automation agency | Solo-operator delivery | MCP Builder, ARL | Likely needs personal-leverage tooling | Cold | "One-person AAA stack: MCP Builder + ARL = 2 senior eng equivalents." |
| 8 | Channing Allen ⚠ | Indie Hackers / Hatch | Co-founder | [LinkedIn](https://www.linkedin.com/in/channingallen) | Indie SaaS founder | Distribution to indie audience | Skill Pack Business Builder | Operates Indie Hackers — partner / amplifier, not buyer | Warm-ish | "Could feature a Skill-Pack-Business case study on IH." |
| 9 | Gabriel Ferraz | Creem | Founder | [LinkedIn](https://www.linkedin.com/in/ferraz-gabriel/) | Indie SaaS founder | Multi-LLM cost/routing | AI Gateway Router, Memory Kit | Already writes about Claude-powered SaaS automation | Cold | "Creem is multi-LLM by nature — Gateway Router cuts your token bill 30%." |
| 10 | Samik Shrotriya | Impractical.ai (YC S22) | Co-founder | [LinkedIn](https://www.linkedin.com/in/samikshro/) | Indie SaaS founder | Memory + state in agent SaaS | Memory Kit, MCP Builder | YC AI founder needs production-grade memory plumbing | Cold | "YC AI founders: Memory Kit drop-in for stateful agents — no Letta lock-in." |
| 11 | Erol Toker | Independent | Solo Capitalist (ex-SaaS CEO) | [LinkedIn](https://www.linkedin.com/in/eroltoker/) | Technical solopreneur | Portfolio of micro-SaaS to maintain solo | PAL, ARL+, Production AI Bundle | Buys leverage tools; budget-able for $999 bundle | Cold | "Micro-SaaS portfolio = perfect ARL+ use case; ship 4 products with 1 brain." |
| 12 | Chris Closset | Giststack | Founder | [LinkedIn](https://pl.linkedin.com/in/chrisclosset) | Technical solopreneur | Operationalizing "AI systems for solopreneurs" | PAL, ARL | Publicly writes on "AI systems for solopreneur leverage" | Cold | "You write about AI leverage — PAL is the agent loop you've been describing." |
| 13 | Quentin Coudert | Limova.ai | Founder | [LinkedIn](https://www.linkedin.com/in/quentin-coudert-b26753a5/) | Technical solopreneur | Building product solo with AI | Production AI Shipping Bundle | Says solo founders need "manpower of 20-person team" | Cold | "Limova-style solo teams: bundle gives you ops, eval, deploy in one." |
| 14 | Rexon Shrestha | Independent | Solo founder / builder | [LinkedIn](https://www.linkedin.com/in/rexonms/) | Technical solopreneur | Build pipeline as solo dev | ARL, ARL+ | Already preaches "AI handles execution" | Cold | "ARL+ is the pre-built execution loop for your solo-builder thesis." |
| 15 | Bryan Wisotsky | Sky SEO Digital | Founder | [LinkedIn](https://www.linkedin.com/in/bwisotsky) | Marketing agency | AEO/GEO service productization | AI Citation Operator Pack, AI Citation Audit | Already brands as SEO + AEO agency; wants ready-made audit SKU | Cold | "Sky SEO clients want AI citation audits — here's the white-label pack." |
| 16 | Jason Barnard ⚠ | Kalicube | Founder/CEO | [LinkedIn](https://www.linkedin.com/in/jasonmbarnard/) | Marketing agency | Scaling Kalicube methodology to partners | AI Citation Audit (competitor/partner) | Coined "AEO" — competitor, but possible licensing partner | Warm-cold | "Kalicube methodology + your audit pack as a tier-1 partner SKU?" |
| 17 | Irina Shvaya | eSEOspace | Founder | [LinkedIn search](https://www.linkedin.com/search/results/people/?keywords=Irina%20Shvaya%20eSEOspace) | Marketing agency | Operationalizing GEO across client portfolio | AI Citation Operator Pack | Built agency around GEO + AEO; needs ops playbook | Cold | "GEO agency operator pack — daily citation tracking workflow built in." |
| 18 | Ben Goodey ⚠ | Spicy Margarita | Founder | [LinkedIn search](https://www.linkedin.com/search/results/people/?keywords=Ben%20Goodey%20Spicy%20Margarita) | Marketing agency | Educating thousands on GEO — needs reusable assets | AI Citation Audit | Educator + agency: partner candidate, also competitive | Warm-cold | "License the audit pack as a Spicy Margarita-branded student deliverable." |
| 19 | Abner Molina | Doc Digital SEM | Founder/CEO | [LinkedIn search](https://www.linkedin.com/search/results/people/?keywords=Abner%20Molina%20Doc%20Digital) | Marketing agency | LLM SEO delivery across 5 offices | AI Citation Operator Pack | Multi-office agency, needs standardized GEO SOP | Cold | "Five offices delivering LLM SEO — same playbook in every market." |
| 20 | Connor Kimball ⚠ | Cairrot | Founder | [LinkedIn search](https://www.linkedin.com/search/results/people/?keywords=Connor%20Kimball%20Cairrot) | Marketing agency | Builds AEO software | (Competitor / integration partner) | Cairrot IS AEO software — competitor/integration partner | Cold | "Audit pack as a Cairrot integration — your tool, our methodology." |
| 21 | Robin Rathore | Bamboo Proptech | Founder | [LinkedIn](https://www.linkedin.com/in/robinrathore/) | Proptech founder | Vendor coordination across UK SMB landlords | Real Estate Vendor Marketplace Kit | UK proptech serving SMB property mgrs; vendor pain real | Cold | "Bamboo + Vendor Marketplace Kit — bolt-on vendor module for your platform." |
| 22 | Matt Fowler | Doorify MLS | CEO | [LinkedIn](https://www.linkedin.com/in/matttriangle/) | Proptech founder | MLS-side vendor + service integration | Real Estate Vendor Marketplace Kit | 30 yrs RE; MLS exec who could license to agents | Cold | "MLS-distributed vendor marketplace — agent value-add, zero infra build." |
| 23 | Joaquin Rivera Martinez del Río | FRAXU | CEO | [LinkedIn](https://www.linkedin.com/in/joaquinriveramartinezdelrio/) | Proptech founder | LATAM RE tech needs vendor layer | Real Estate Vendor Marketplace Kit | Building RE platform in LATAM, vendor mgmt gap | Cold | "Spanish-language vendor marketplace kit — drop into FRAXU's stack." |
| 24 | Martin Byrne | sonpito | Co-founder & CEO | [LinkedIn](https://www.linkedin.com/in/martinbyrne/) | Proptech founder | Corp RE workflow, vendor scheduling | Real Estate Vendor Marketplace Kit | CRE/IoT founder; vendor coordination = adjacent value | Cold | "sonpito + vendor marketplace = full CRE operations layer." |
| 25 | Elliott Sudwarts | Scale RE | Co-founder | [LinkedIn](https://www.linkedin.com/in/elliottsudwarts/) | Proptech founder | Streamlining RE sales process | Real Estate Vendor Marketplace Kit | RE sales-tech founder; vendor side is natural extension | Cold | "Scale RE handles sale; our kit handles vendor side of close." |
| 26 | Ravi Kumar Sapata ⚠ | PropTechBuzz | Founder/CEO | [LinkedIn](https://www.linkedin.com/in/yoursproductly/) | Proptech founder | Distribution to proptech audience | Real Estate Vendor Marketplace Kit | Runs proptech media — partner/amplifier | Warm-cold | "Feature Vendor Marketplace Kit launch on PropTechBuzz." |
| 27 | Frank Fiegel (punkpeye) ⚠ | Glama | Founder; maintainer awesome-mcp-servers | [X/@punkpeye](https://x.com/punkpeye) · [GitHub](https://github.com/punkpeye) | AI dev tools / infra | Catalog of 87k+ stars; needs monetizable adjacent SKU | MCP Builder (competitor/partner) | Maintains the canonical MCP directory; partner candidate | Warm | "Listed in awesome-mcp-servers — want to co-feature a Builder edition?" |
| 28 | Joe Heitzeberg ⚠ | AI Tinkerers | Founder | [LinkedIn](https://www.linkedin.com/in/joeheitzeberg/) | AI dev tools / infra (community) | Monetizing 108k-member network | Skill Pack Business Builder | Runs largest AI builder community — partner/distribution | Warm-cold | "Sponsored Skill-Pack workshops at AI Tinkerers chapters." |
| 29 | Ankur Goyal ⚠ | Braintrust / Fibr AI | CEO | [LinkedIn](https://www.linkedin.com/in/ankurgoyal22/) | AI dev tools / infra | Competes in eval/observability | (Competitor — observability) | Direct competitor — partner only | Cold | "Skip — competitor; track for partnerships only." |
| 30 | Theo Browne | T3 Chat / Ping Labs | Founder | [LinkedIn](https://www.linkedin.com/in/t3gg/) · [X/@theo](https://x.com/theo) | AI dev tools / infra | Audience-first; needs reusable agent tooling | MCP Builder, Memory Kit | Massive dev audience; ship-fast ethos | Cold | "T3-stack MCP Builder pack — typed end to end for your audience." |
| 31 | Cole Medin ⚠ | Dynamous AI | Founder | [YouTube](https://www.youtube.com/@ColeMedin) | AI consultant | Productizing his RAG/agent IP | Production AI Shipping Bundle | Sells his own AI community/courses — competitor/partner | Warm-cold | "Bundle as a Dynamous community add-on." |
| 32 | Hamel Husain ⚠ | Independent | AI consultant | [Twitter/@HamelHusain](https://x.com/HamelHusain) | AI consultant | Independent consultant scaling deliverables | Production AI Shipping Bundle | Markets his own LLM eval course — peer, possible reseller | Warm-cold | "Production bundle as the 'do-the-work' companion to your evals course." |
| 33 | Jason Liu (jxnl) ⚠ | Independent | AI consultant; creator of Instructor | [Website](https://jxnl.co/) · [Twitter/@jxnlco](https://x.com/jxnlco) | AI consultant | Same — productizing consulting | Skill Pack Business Builder | Peer / amplifier; would license content sooner than buy | Warm-cold | "Skill Pack Business Builder = the playbook you tell every client to copy." |
| 34 | Greg Isenberg ⚠ | Late Checkout | CEO | [Twitter/@gregisenberg](https://x.com/gregisenberg) | AI consultant (idea-maven) | Always sourcing tools to feature | Skill Pack Business Builder | Posts daily AI agency content; massive amplifier | Warm-cold | "Feature: 'How to launch a $99/mo skill pack business in 7 days.'" |
| 35 | Pieter Levels (levelsio) | Nomad List / PhotoAI | Solo founder | [Twitter/@levelsio](https://x.com/levelsio) | Technical solopreneur | Multi-product solo ops | ARL+, PAL | Archetype of leverage-buyer | Cold | "ARL+ tested on 6 products in a week — your kind of ROI test." |
| 36 | Marc Lou ⚠ | ShipFast / Indie Page | Solo founder | [Twitter/@marc_louvion](https://x.com/marc_louvion) | Technical solopreneur | Boilerplate-first mindset | Production AI Shipping Bundle | Sells ShipFast — adjacent competitor | Warm-cold | "AI-shipping bundle as a ShipFast add-on SKU." |
| 37 | Tony Dinh | DevUtils / TypingMind | Solo founder | [Twitter/@tdinh_me](https://x.com/tdinh_me) | Technical solopreneur | Speed-to-launch | Production AI Bundle, MCP Builder | Built TypingMind in 5 days | Cold | "Bundle = what TypingMind v2 would have shipped with on day 1." |
| 38 | Ben Tossell ⚠ | Ben's Bites | Founder | [Twitter/@bentossell](https://x.com/bentossell) | AI consultant / educator | Audience monetization | Skill Pack Business Builder | Sells AI education; partner / amplifier | Warm-cold | "Co-launch a Skill Pack Builder cohort to Ben's Bites list." |
| 39 | Sam Bhagwat ⚠ | Mastra | Co-founder / CEO | [LinkedIn search](https://www.linkedin.com/search/results/people/?keywords=Sam%20Bhagwat%20Mastra) | AI dev tools / infra | TS agent framework adoption | (Partner) | Mastra IS the TS agent framework — integration partner | Cold | "Memory Kit packaged as a Mastra-compatible drop-in." |
| 40 | Abhi Aiyer ⚠ | Mastra | Co-founder | [LinkedIn](https://www.linkedin.com/in/abhi-aiyer-aa41bb42) | AI dev tools / infra | Same | (Partner candidate) | Co-founder Mastra | Cold | "Bundle published as a Mastra reference architecture." |
| 41 | Tyler (AI Designer MCP) ⚠ | aidesigner | Maker | [Product Hunt](https://hunted.space/product/aidesigner) | AI dev tools / infra | Productizing MCP-based UI tooling | MCP Builder (peer) | Recent PH MCP launch — peer | Cold | "Cross-promote MCP Builder + AI Designer MCP starter pack." |
| 42 | Dominik (MCP-Builder.ai) ⚠ | MCP-Builder.ai | Maker | [Product Hunt](https://www.producthunt.com/products/mcp-builder-ai) | AI dev tools / infra | Direct competitor | (Direct competitor) | Skip as buyer; competitive watch | Cold | "Track only — direct MCP Builder competitor." |
| 43 | Luis Cancilleri | Independent | Indie hacker / AI tools | [LinkedIn](https://es.linkedin.com/in/luis-cancilleri) | Indie SaaS founder | Building AI-powered tools solo | Memory Kit, MCP Builder | Active indie-hacker AI-tools brand | Cold | "Memory Kit drop-in to extend any of your AI tools to multi-session." |
| 44 | A. LDU (ledevultime) | 3 SaaS + 4 micro-SaaS | Indie hacker | [LinkedIn](https://fr.linkedin.com/in/ledevultime) | Indie SaaS founder | Maintaining 7+ products solo | ARL+, Memory Kit | Operates portfolio; leverage tools resonate | Cold | "Portfolio-first solo dev — ARL+ amortized across 7 products." |
| 45 | Bagus Ramadhan | Independent | Solopreneur | [LinkedIn](https://www.linkedin.com/in/bagusramadhan/) | Technical solopreneur | Solo SMB ops | PAL, MCP for Local Business Automation | Posts publicly on solopreneur + AI | Cold | "PAL for solopreneurs — your daily ops loop, automated." |
| 46 | Aaina Sharma | Feels Like July | Solo founder | [LinkedIn](https://www.linkedin.com/in/aaina/) | Technical solopreneur | One-woman business — leverage need | PAL, ARL | Self-describes as one-woman company | Cold | "One-person teams: PAL is the 'second brain' you've been describing." |
| 47 | Sani Varada | AI Automation Agency | Founder | [LinkedIn](https://in.linkedin.com/in/sani-varada-845869176) | AI automation agency | India SMB delivery | MCP for Local Business Automation | India-focused AAA; SMB pricing fits $99 packs | Cold | "Local-biz MCP pack at India-friendly price — resell at 10x." |
| 48 | R K Yadav | AI Automation Agency | Founder | [LinkedIn](https://in.linkedin.com/in/rahulkumaryadav) | AI automation agency | Same — India SMB delivery | MCP Builder, Local Business pack | High-volume AAA founder | Cold | "Resell the local-biz MCP pack across your client book." |
| 49 | Aryan Gorde | AI Automation Agency | Founder | [LinkedIn](https://in.linkedin.com/in/aryan-gorde-7715833a9) | AI automation agency | Young founder building delivery system | MCP Builder, Skill Pack Business Builder | Early-career AAA, education + tooling combo lands | Cold | "Skill-Pack-Business + MCP Builder = your AAA OS." |
| 50 | Bradley Leese | DirectiveGroup | Senior SEO / GEO | [LinkedIn](https://www.linkedin.com/in/seniorseoanalyst/) | Marketing agency | Modernizing a traditional SEO shop to AEO | AI Citation Audit | Inside a traditional agency adding GEO — needs reusable audit | Cold | "Inside-the-agency champion — bring the audit pack as your internal GEO playbook." |

### Coverage summary

| Category | Count | Notes |
|---|---:|---|
| AI automation agency | 11 | Strong coverage |
| Indie SaaS founder | 4 | Could add 2–3 more from IndieHackers leaderboard |
| AI consultant | 5 | All "warm-cold" — peers/partners more than buyers |
| Marketing agency (GEO/AEO) | 6 | Several competitors flagged ⚠ |
| Proptech founder | 6 | Mostly cold |
| Technical solopreneur | 8 | Best volume buyers |
| Local business automation builder | 0 standalone | Folded into AAA (#5, #47); add 3–5 dedicated from network |
| AI dev tools / infra | 7 | Mix of peers, partners, competitors |

**Gaps to fill from David's existing network:**
- 3–5 dedicated "Local business automation builder" prospects (HVAC/dental/legal verticals)
- 2 additional indie SaaS founders with confirmed MCP interest
- 2 marketing agency owners doing AEO who are not already competitors

### Top 10 highest-signal prospects (contact first)

1. **Robin Rathore (Bamboo Proptech)** — only mid-stage proptech with visible vendor-mgmt pain and recent award traction.
2. **Bryan Wisotsky (Sky SEO Digital)** — explicitly brands as SEO+AEO agency founder; ready for an audit SKU.
3. **Joshua Leavitt (Omni AI)** — uses CEO framing, will pay premium for "production" bundles.
4. **Quentin Coudert (Limova.ai)** — publicly preaches solo-leverage thesis; matches Production AI Bundle word-for-word.
5. **Theo Browne (Ping Labs / T3 Chat)** — massive dev audience, ship-fast culture; if he posts about MCP Builder it converts thousands.
6. **Matt Fowler (Doorify MLS)** — distribution into MLS agents is a force multiplier for Vendor Marketplace Kit.
7. **Sam Poutakidis** — explicit AAA founder, early-stage, needs a productized SKU now.
8. **Abner Molina (Doc Digital SEM)** — five-office LLM-SEO agency; needs standardized GEO operator pack.
9. **A. LDU (ledevultime)** — runs 7 SaaS products solo; ARL+ has obvious ROI math.
10. **Joaquin Rivera Martinez del Río (FRAXU)** — LATAM proptech with English/Spanish bridge; unowned market for Vendor Marketplace Kit.

**Buyer-vs-partner split:** ~31 likely buyers, ~14 partners/competitors (⚠), ~5 warm amplifiers. ~30 buyable from this list; supplement with 20 names from David's CRM/Twitter DMs to hit a 50-buyer target.

---

## 7. Recommendation

**Top 3 products to launch first:**

1. **MCP Server Builder Pro** — $299–$499 one-time, sold as a Claude Skill + GitHub template + Lemon Squeezy delivery.
2. **MCP / Agent Security Audit** — $499–$999 productized one-off audit; deliver as PDF report + remediation skill pack.
3. **AI Citation (GEO) Audit** — $299–$799 productized one-off audit; deliver as PDF report + Notion playbook + 30-day re-scan email.

**Why these three, in this order, based on the data:**

- **MCP Server Builder Pro is the hottest demand-side bet by every measure.** Section 1 shows the MCP cluster is at peak buyer attention (97M SDK downloads, 78% enterprise adoption); Section 3 shows ~14K MCP-server repos and Docker MCP servers passing 1M downloads each; Section 4 has the cleanest named pain in the entire dataset — OAuth-2.1 implementation, multi-tenant auth, token recovery, discovery UX — all citable from GitHub issues, HN, and dev blogs; and Section 2 confirms **white space**: every named MCP boilerplate (PaidMCP, iannuttall, f/mcp-startup-boilerplate) is free, and enterprise gateways (MintMCP, Runlayer) are sales-led with no public price. The $299–$499 paid-template tier is uncontested.

- **MCP / Agent Security Audit is the highest-margin bet.** Section 1 marks MCP security as the steepest rising curve and Section 4 quantifies it — Astrix found 53% of 5,200 production MCP servers ship without proper auth; 30+ CVEs in a single 60-day window. Buyers have CISO-level budgets (Section 1 cites 88% of orgs reporting agent incidents, 92% of security pros concerned, Gartner #1 cybersec trend). Section 2 confirms no productized audit at $499–$2,999 exists — only sales-led enterprise contracts at $3k–$15k or free OSS like RAMPART. This is the lane where the highest premium is defensible immediately.

- **AI Citation (GEO) Audit is the fastest cash bet.** Section 1 puts generative engine optimization as the steepest-rising term in the citation cluster; Section 4 has the *only* explicit "I would pay $39–$79/mo" quote in the entire dataset; Section 2 documents the white space — only one sub-$500 one-time audit exists (AI Labs Audit at $149); everything else is $189+/mo SaaS or $1.5k+ services. Marketing agencies already buy SEO tools — the muscle memory exists and HubSpot shipping a free AEO grader proves top-of-funnel demand is incumbent-validated.

**Why we deprioritize the other named LBC ideas this week:**

- **Skill Pack Business Builder** ranks coldest in the pain heat map (Section 4). Real seller revenue stories exist on Gumroad/PromptBase, but buyer-side demand isn't loud yet. Sell this *after* MCP Builder ships, as the meta-product David's first three buyers will want next.
- **Memory Pack** and **RAG Regression Pack** are warm but partially served (Mem0/Zep/Letta + Ragas/DeepEval/Braintrust already absorbing demand). Bundle them as **$99–$199 add-ons** to the MCP Builder or Production AI Shipping Bundle rather than standalone hero SKUs.
- **Real Estate Vendor Marketplace Kit** has real proptech buyers (Section 6 surfaced 6) but the Counsel-gate compliance variants in Section 5c slow it down. Ship the platform-access / verified-vendor / data-integration variants first, hold transaction-fee variants for counsel review.
- **Production AI Shipping Bundle** as named is best understood as a **positioning wrapper** around the three top SKUs above (MCP Builder + Security Audit + GEO Audit) sold at $999 with a $200 bundle discount. Launching it concurrently with the three components gives upsell math from day one.

**Operational sequence for the next 7 days (matches David's $2,000/week goal):**

| Day | Action |
|---|---|
| 1 (today) | Pick brand/domain; spin Lemon Squeezy store (kills R2/signed-URL work); confirm or upload PAL/ARL/MCP Builder source masters to this repo or to David's local. |
| 2 | Write MCP Server Builder Pro landing copy + Stripe/LS product + Claude Skills.ai listing + Gumroad mirror. Price: $299 (anchor $499). |
| 3 | Write MCP / Agent Security Audit landing copy + intake form (3-question Typeform) + delivery template (PDF + remediation skill pack). Price: $499 founder, $999 list. |
| 4 | Write AI Citation Audit landing copy + intake form (URL + 5 keywords) + delivery template. Price: $299 founder, $599 list. |
| 5 | Top-10 prospect DM/email round (Section 6) — personalized angle each. |
| 6 | Product Hunt + Show HN + r/ClaudeAI + LinkedIn launch for MCP Server Builder Pro specifically (it has the strongest "show, don't tell" demo). |
| 7 | Iterate on first-day data; if MCP Builder is converting, ship the $999 Production Bundle; if Security Audit is converting, do a paid red-team livestream as social proof. |

**Working hypothesis vs. what the data changed:**

David's hypothesis was: Production AI Shipping Bundle, MCP Server Builder Pro, Agent Security Audit, AI Citation Audit. **The data confirms 3 of 4** — Production AI Shipping Bundle should be repositioned as a *bundle of the other three* rather than a separate hero SKU. The product lane order should be MCP Builder → Security Audit → GEO Audit, with Memory + RAG as add-ons and Skill Pack Business Builder deferred to v2 once first cash lands.

**Single biggest unblocker right now:** confirm where the existing PAL / ARL / MCP Server Builder source masters live, and either commit them to this branch or wire fulfillment to wherever they are. Everything else is downstream of that one decision.
