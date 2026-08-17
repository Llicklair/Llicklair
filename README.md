# Marcos Recio Sánchez

**AI Solutions & Automation Engineer** · Valencia, Spain

I build agentic AI systems that execute real business processes — not notebooks, not wrappers around a model API, but software that holds up under real constraints: multi-tenant isolation, Spanish tax compliance, and the rule that an autonomous system is never allowed to lie to you about its own results.

I came to engineering through the back door. My background is logistics and administration — AS400 at DB Schenker, port documentation at Cemesa, internal processes at Improving — which means I spent years on the receiving end of badly built business software before I learned to build it. **AutomatizaCore exists because I lived the problems it solves.**

I am looking for roles in **AI-driven business process automation**: consultancies, systems integrators, business software, and the wider ERP and accounting-practice ecosystem.

---

## Main project

### [AutomatizaCore](https://github.com/Llicklair/Automatiza-Core) — Spanish ERP with agentic AI, self-hosted

🔗 **[Landing page and video demo](https://llicklair.github.io/Automatiza-Core_landing)** · *early access*

A full business management platform — invoicing, accounting, banking, CRM, HR and Verifactu tax compliance — operated in natural language, where 14 domain agents carry out the actual business actions.

- **Multi-agent architecture** orchestrated with LangGraph: classify → plan → validate → dispatch, with customisable AI employees (~45 skills).
- **Custom RAG system** built on pgvector with offline embeddings (BAAI/bge-m3), answers cited back to the source.
- **Automation engine** with time- and event-based triggers, plus OAuth integrations (Gmail, Outlook, Drive, OneDrive) over APIs, JSON and webhooks.
- **Multi-tenant** with strict `tenant_id` filtering and human approval gates before any action with side effects.
- **Provider-agnostic**: Claude, Gemini and OpenAI with automatic fallback.

Designed and shipped end-to-end, solo.

`~67k lines of backend · 900+ commits · 69 API routes · 109 pages · Python · FastAPI · LangGraph · PostgreSQL/pgvector · Next.js · Electron`

---

## Tooling for AI coding agents

**[galaxy-brain](https://github.com/Llicklair/galaxy-brain)** — the deterministic harness an agent should be standing on
Facts about your Python code — where it died and in what state, what shape it has, who calls what, what a diff moved — in milliseconds, offline, and **with no model anywhere in the path**. Automatic error capture through `sys.excepthook`, so you never have to reproduce the failure; module, symbol and call graphs; and change-impact analysis. Pre-commit hook in ratchet mode: inherited debt passes, new debt does not.
`Python ≥3.9 · v0.7.0 · 445 commits · 15.6k lines of source / 11.8k of tests · 850 tests · zero runtime dependencies · Apache-2.0`

**[Forja](https://github.com/Llicklair/forja)** — autonomous code review loop
A finder→tester→fixer→evaluator pipeline that sweeps an entire project through six rotating lenses: correctness, security, concurrency, error handling, test gaps and performance. Test-first verification, an independent evaluator as the gate, cost-controlled modes, and one hard rule: it never auto-merges.
`Claude Code plugin · MIT`

**[El Consejo de los 7 Sabios](https://github.com/Llicklair/consejo-7-sabios)** — seven agents with opposing views argue about your code
Seven conflicting perspectives debate until they reach consensus, a judge synthesises the plan, and it gets executed. With pixel-art animation in the terminal, because the tools that are a pleasure to look at are the ones you actually end up using.
`Python · pytest · MIT`

**[invest-ll](https://github.com/Llicklair/invest-ll)** — an investment system built on one constraint
It proposes exact trades in equities and crypto. The principle that comes before everything else: *the system cannot lie to you about its own results.* No lookahead bias, realistic simulation, comparable strategies, capital safety on by default.
`Python · pytest · ruff · pyright`

---

## How I work

- **Facts decide, approximations inform.** Anything an agent acts on should be measured, not inferred. That is why galaxy-brain keeps every model off the hot path.
- **Tests before trust.** Close to a 1:1 test-to-source ratio in the harness; pytest, Playwright E2E, `ruff` and `pyright` gating every integration. An autonomous system without verification is just a fast way to be wrong.
- **Constraints first.** The interesting engineering starts when you write down what the system is *not* allowed to do.
- **Subtract before polishing.** Maintenance cost grows with the number of components, so the default answer to a new one is no.
- **Evidence before folklore.** Design decisions cite measured data, and negative results get written down too.

**AI and automation:** AI agents · multi-agent architectures · LangGraph · RAG and embeddings · APIs, JSON, webhooks · OAuth · Claude, Gemini, OpenAI
**Development:** Python · FastAPI · SQLAlchemy · PostgreSQL + pgvector · TypeScript · Next.js · React · Electron · Docker
**Business systems:** AS400 · IWIS · document management
**Languages:** Spanish (native) · English (C1)

---

## Contact

📧 marcosreciosanchez@gmail.com · 🌐 [Portfolio](https://llicklair.github.io/) · 🌐 [AutomatizaCore](https://llicklair.github.io/Automatiza-Core_landing) · 📍 Valencia, Spain

