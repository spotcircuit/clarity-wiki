# Site Builder

#platform #site-builder #tool #revenue

Google Maps business listing to deployed React website in 60 seconds. Scrape, generate AI content, build, deploy, edit inline.

## Architecture

- **Frontend**: Vue 3 + TypeScript + Pinia + Tailwind (port 5177)
- **Backend**: FastAPI + Python 3.13 + asyncio (port 9405)
- **Generated sites**: React 18 + Tailwind CSS (Vite build)
- **AI Content**: Claude Sonnet for copy, Gemini 2.5 Flash for images
- **Deploy**: Cloudflare Pages (primary), Vercel (fallback)
- **Real-time**: WebSocket for pipeline progress

## Pipeline

| Step | Module | Output |
|------|--------|--------|
| 1. Parse Google Maps URL | `maps_url_parser.py` | ParsedMapsUrl |
| 2. Scrape business profile | `maps_scraper.py` (Playwright) | BusinessData |
| 3. Scrape business website | `website_scraper.py` (optional) | WebsiteData |
| 4. Generate AI content | `site_generator.py` (Claude) | SiteContent |
| 5. Generate AI images | `image_generator.py` (Gemini) | ImageGenerationResult |
| 6. Build React site | `react_builder.py` (npm build) | dist/ |
| 7. Deploy | `cloudflare_deployer.py` / `vercel_deployer.py` | Live URL |

## Location

`/home/spotcircuit/agentic/agent-experts/apps/site_builder/`

Standalone repo: `spotcircuit/site-builder` (auto-synced via GitHub Actions)

## Revenue Connection

This is a demonstration tool for the **AI Integration Consulting** and **Knowledge Base Builder** revenue streams. Shows end-to-end AI pipeline from scrape to deploy.

## Related

- [[cloudflare-pages-deploy]] -- deployment pattern with project limit management
- [[websocket-progress-pattern]] -- real-time pipeline progress via WebSocket
- [[inline-editor-pattern]] -- post-generation editing with live preview
- [[ai-content-pipeline]] -- Claude + Gemini hybrid content generation
- [[act-learn-reuse-testing]] -- self-improving test pattern

---
Source: raw/site-builder-readme.md, raw/site-builder-architecture.md | Ingested: 2026-04-08
