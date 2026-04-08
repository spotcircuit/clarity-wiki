# GetRankedLocal

#platform #product #local-seo #grid-search #playwright #lead-gen

Google Maps ranking analysis and lead generation platform. 169-point grid searches show exactly where a business ranks across their entire service area.

## What It Does

1. User enters a business name and keyword (e.g. "medical spa near me")
2. System generates a 13x13 grid (169 points) across a 5-mile radius
3. Playwright runs 169 parallel Google Maps searches at each coordinate
4. Results mapped to an interactive heat map showing ranking positions
5. AI extracts business intelligence and competitor analysis
6. Personalized landing page shows revenue impact of poor rankings

## Stack

| Layer | Technology |
|---|---|
| Frontend | Next.js 15.5 + React 19 + TypeScript + Tailwind |
| Database | Neon PostgreSQL (serverless) |
| Scraping | Playwright (169 concurrent browser tabs) |
| Visualization | Recharts + Google Maps API + custom heat maps |
| Backend | Railway (Python/Flask scraper) |
| Deploy | Vercel (frontend) + Railway (scraper) |

## Key Numbers

- 169 grid points per search (13x13)
- 6,511+ leads across 9 business categories
- 5 specialized database tables for grid data
- 21+ Playwright e2e tests

## Revenue Potential

Targets local businesses who don't know they're invisible on Google Maps. Three pricing models under consideration:
- SaaS: $99-499/mo
- Agency reseller: $500-1000/mo (white-label)
- Lead marketplace: per-qualified-lead pricing

## Patterns Worth Noting

- **Parallel Playwright scraping** at scale (169 concurrent searches)
- **Bulk database inserts** with deduplication via Place IDs
- **Geographic grid math** for coordinate calculations
- **Progressive disclosure UI** (simple vs detailed view toggle)

## Location

GitHub: `github.com/spotcircuit/getrankedlocal`
Live: `https://getrankedlocal.com`

## Related

- [[site-builder-overview]] -- similar scrape-to-deploy pipeline
- [[lead-finder]] -- lead prospecting from different sources
- [[cloudflare-pages-deploy]] -- similar deployment patterns

---
Source: raw/getrankedlocal-README.md, raw/getrankedlocal-ARCHITECTURE.md | Ingested: 2026-04-08
