# Listing Launch

#apps #reference #real-estate #content-gen

Real estate marketing content generator. 4-step wizard: address autocomplete → scrape property → generate multi-channel content (MLS, Instagram, Facebook, Email, Flyer) with HUD Fair Housing compliance.

## What It Does

1. Address autocomplete via Google Places
2. Property data scraping
3. Multi-channel marketing content generation via Claude
4. Fair housing compliance validation (regex-based)

## Stack

FastAPI + Vue 3 + WebSocket

## Location

`/home/spotcircuit/agentic/agent-experts/apps/listing_launch/`

## Patterns Worth Referencing

- **Multi-channel content gen** — One source, multiple output formats
- **Compliance validation** — Regex-based content filtering for legal requirements
- **Wizard UI pattern** — Step-by-step Vue 3 workflow

## Related

- [[site-builder-overview]] -- similar scrape-to-content pipeline
- [[ai-content-pipeline]] -- content generation patterns

---
Source: agent-experts/apps/listing_launch/ | Ingested: 2026-04-08
