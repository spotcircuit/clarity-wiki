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

| Project | Purpose |
|---|---|
| Site Builder | FastAPI backend for site generation pipeline |
| getrankedlocal | Python/Flask scraper for grid search Playwright automation |
| Agent Experts - Orchestrator | Pre-Paperclip orchestrator (likely deprecated) |
| Digitize-Invoices | Invoice processing |
| valiant-creation | Unknown |
| dependable-expression | Unknown |
| tac | Unknown |

Railway auto-deploys from standalone GitHub repos on push to main.

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
