# LeadFinder

#apps #leadfinder #scraping #leads #python

Production lead generation system. Google Maps scraping via Playwright, AI business intelligence enrichment, PostgreSQL storage, FastAPI REST API. Batch orchestrator, staggered launcher, BetterContact email enrichment.

## Architecture

- **Backend**: FastAPI + Python 3.11+ + uvicorn
- **Scraping**: Playwright (Google Maps profiles)
- **Database**: PostgreSQL
- **Deployment**: Render
- **Enrichment**: BetterContact (email discovery)

## Pipeline

Orchestrator (batch) -> Staggered Launcher (distributed) -> Google Business Profile Parallel (core scraper) -> AI Enrichment -> Database Insert -> Deduplication

## Variants

- `leadfinder` -- this repo, production API on Render
- `leadfinder_parallel` -- newer variant with sales funnel system, 70+ cities scraped, 3,748+ businesses

Source: github.com/spotcircuit/leadfinder README | Ingested: 2026-04-07

## Related

- [[lead-finder]] -- existing wiki reference page
- [[getrankedlocal]] -- complementary (grid rankings + lead collection)
- [[site-builder-overview]] -- leads from finder could feed site generation
