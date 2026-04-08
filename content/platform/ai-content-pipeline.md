# AI Content Pipeline

#platform #site-builder #ai #claude #gemini

Hybrid AI approach: Claude Sonnet generates website copy, Gemini 2.5 Flash generates hero/about images. Config-driven, model-swappable.

## Content Generation (Claude)

Module: `site_generator.py` (1039 lines)

- Input: BusinessData (scraped from Google Maps) + optional WebsiteData
- Output: SiteContent — structured JSON with all section content
- Prompt includes business name, category, rating, reviews, hours, services
- Generates: hero headline/sub, about text, services list, FAQ, testimonials, CTAs, SEO metadata
- Section-level regeneration via `/api/generate-section` endpoint

## Image Generation (Gemini)

Module: `image_generator.py` (302 lines)

- Uses Gemini 2.5 Flash Image model
- Generates hero background and about section image
- Prompt derived from business category and generated content
- Falls back gracefully if GEMINI_API_KEY not set

## Pattern: Config-Driven Provider

The pipeline doesn't hardcode Claude or Gemini. The model is selected via env vars and could be swapped. This matches the [[config-driven-routing]] pattern from Clarity.

## Related

- [[site-builder-overview]] -- full pipeline context
- [[config-driven-routing]] -- routing logic in config, not code

---
Source: raw/site-builder-architecture.md, raw/site-builder-readme.md | Ingested: 2026-04-08
