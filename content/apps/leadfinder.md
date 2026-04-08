# LeadFinder

#apps #leadfinder #scraping #leads #python

Production lead generation system. Google Maps scraping via Playwright, AI enrichment, PostgreSQL storage, FastAPI REST API. Deployed on Render.

## What It Does

Scrapes Google Maps business profiles in parallel, enriches with AI-powered business intelligence, stores in PostgreSQL, exposes via FastAPI REST API. Batch processing via orchestrator, staggered launcher for distributed scraping, BetterContact email enrichment.

## Tech Stack

- **Backend**: FastAPI + Python 3.11-3.13 + uvicorn
- **Scraping**: Playwright (Google Maps)
- **Database**: PostgreSQL
- **Enrichment**: BetterContact (email discovery)
- **Deployment**: Render
- **Repo**: github.com/spotcircuit/leadfinder

## Status

Dormant -- last updated August 2025. Related: leadfinder_parallel (newer variant with sales funnel).

Source: GitHub README | Ingested: 2026-04-07

## Related

- [[getrankedlocal]] -- uses similar Google Maps data for ranking analysis
- [[lead-finder]] -- existing wiki reference page
- [[site-builder-overview]] -- uses similar Maps scraping pattern
