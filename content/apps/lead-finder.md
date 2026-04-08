# Lead Finder

#apps #reference #scraping #lead-gen

Multi-source real estate lead prospecting tool. Scrapes Zillow FSBO, Craigslist, Redfin with Playwright + generates AI outreach pitches with Claude Haiku.

## What It Does

1. Parallel scraping across multiple lead sources with stealth anti-detection
2. Unified lead normalization into common schema
3. AI-powered outreach pitch generation (Claude Haiku for speed/cost)
4. Vue 3 UI with WebSocket progress tracking

## Stack

FastAPI + Vue 3 + Playwright + Claude Haiku

## Location

`/home/spotcircuit/agentic/agent-experts/apps/lead_finder/`

## Patterns Worth Referencing

- **Stealth scraping** — Anti-detection tactics for Playwright automation
- **Parallel source scraping** — Multiple sources normalized into one schema
- **AI pitch generation** — Fast, cheap content gen with Haiku

## Related

- [[site-builder-overview]] -- similar scrape-to-AI pipeline
- [[ai-content-pipeline]] -- content generation patterns

---
Source: agent-experts/apps/lead_finder/ | Ingested: 2026-04-08
