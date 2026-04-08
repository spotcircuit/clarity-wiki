# Infrastructure

#platform #infrastructure #deployment #railway #vercel #cloudflare #neon

Shared deployment infrastructure across all SpotCircuit apps.

## Deployment Matrix

| App | Frontend | Backend | Database | Generated Sites |
|---|---|---|---|---|
| **SpotCircuit Website** | Vercel | - | - | - |
| **Site Builder** | Vercel | Railway | - | Cloudflare Pages (or Vercel) |
| **GetRankedLocal** | Vercel | Railway | Neon PostgreSQL | - |
| **Clarity Wiki** | GitHub Pages (Quartz) | - | - | - |

## Railway Projects

Railway hosts Python/Flask backends. CLI installed (`railway 4.8.0`).

| Project | Repo | Language | Purpose |
|---|---|---|---|
| Site Builder | spotcircuit/site-builder | Python | FastAPI backend for site generation pipeline |
| getrankedlocal | spotcircuit/getrankedlocal | Python | Flask scraper for grid search Playwright |
| Agent Experts - Orchestrator | spotcircuit/agent-experts | Python | Pre-Paperclip orchestrator (deprecated) |
| Digitize-Invoices | spotcircuit/invoicedb | Python | Invoice database with agentic AI workflows |
| tac | spotcircuit/tac-8 (latest) | Python | TAC project (5 iterations: tac-4 through tac-8) |
| valiant-creation | ? | ? | Unknown Railway project |
| dependable-expression | ? | ? | Unknown Railway project |

Railway auto-deploys from standalone GitHub repos on push to main.

## Full GitHub Repo Inventory (Docker-ready)

All of these have Dockerfiles and are Railway-deployable:

| Repo | Language | Description |
|---|---|---|
| spotcircuit/site-builder | Python | Google Maps to React site in 60s |
| spotcircuit/getrankedlocal | TypeScript | Local SEO grid ranking + lead gen |
| spotcircuit/seosnap | TypeScript | AI-powered SEO audit with Lighthouse + GPT-5 |
| spotcircuit/TextPRO | Python | Backend services with AI Developer Workflow |
| spotcircuit/prior-auth-fastlane | Python | Healthcare prior-auth SaaS MVP |
| spotcircuit/invoicedb | Python | Invoice database with agentic AI |
| spotcircuit/service-marketplace | TypeScript | Next.js service marketplace platform |
| spotcircuit/leadfinder | Python | Lead finder (original) |
| spotcircuit/leadfinder_parallel | Python | Lead finder (parallel version) |
| spotcircuit/chopshop | TypeScript | TBD |
| spotcircuit/parcelaudit | TypeScript | TBD |
| spotcircuit/velocityelectric | TypeScript | TBD |
| spotcircuit/drcoins | TypeScript | TBD |
| spotcircuit/roofmaster | TypeScript | TBD |
| spotcircuit/TruckingAIO | TypeScript | TBD |
| spotcircuit/tac-4 through tac-8 | Python | TAC iterations |

## Vercel

Vercel hosts all Next.js/Vue frontends. Auto-deploys from GitHub.

| Project | Repo |
|---|---|
| spotcircuit.com | spotcircuit/spotcircuit |
| Site Builder frontend | spotcircuit/site-builder |
| getrankedlocal.com | spotcircuit/getrankedlocal |

## Cloudflare Pages

Used by Site Builder to deploy generated React sites. Each generated site gets its own Cloudflare Pages project (auto-named `site-{slug}-{jobid}`).

Account-level project limit exists. The deployer auto-deletes the oldest project when limit is hit.

Requires: `CLOUDFLARE_API_TOKEN`, `CLOUDFLARE_ACCOUNT_ID`

## Neon PostgreSQL

Serverless PostgreSQL used by GetRankedLocal.

| Table | Purpose |
|---|---|
| grid_searches | Main search records |
| grid_competitors | Discovered businesses |
| grid_point_results | Rankings at each grid coordinate |
| competitor_summaries | Aggregated statistics |
| grid_cells | Cell metadata with competition density |
| lead_collections | Many-to-many lead organization |
| prospects | Detailed lead information |

## GitHub Pages

Hosts the Clarity Wiki via Quartz static site generator.
- Repo: spotcircuit/clarity-wiki-site
- URL: https://spotcircuit.github.io/clarity-wiki-site/
- Deploy: GitHub Actions on push to main

## Paperclip

Local orchestration platform at `localhost:3100`. Manages 5 Claude Code agents.
- Install: `~/.paperclip/`
- Start: `npx paperclipai run`
- Embedded PostgreSQL on port 54329

See [[paperclip-integration]] for agent details.

## Related

- [[paperclip-integration]] -- agent orchestration
- [[cloudflare-pages-deploy]] -- deployment pattern details
- [[site-builder-overview]] -- uses Railway + Cloudflare
- [[getrankedlocal]] -- uses Railway + Neon + Vercel

---
Source: railway list, app expertise files | Filed: 2026-04-08
