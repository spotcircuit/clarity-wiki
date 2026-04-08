# Make to n8n Converter

#apps #make-2-n8n #n8n #automation #converter

Make.com to n8n workflow converter and pricing tool. Upload Make workflow JSON, analyze complexity, categorize nodes into price tiers (Simple $25, Moderate $50, Complex $100).

## Architecture

- **Frontend**: Next.js + JavaScript
- **API**: /api/analyze-workflow (parse + categorize)
- **Deployment**: Vercel

## Node Categories

| Tier | Price | Examples |
|------|-------|---------|
| Simple | $25 | Basic triggers, simple operations |
| Moderate | $50 | API integrations, data transformation |
| Complex | $100 | Custom code, routing, media processing |

## Related Repos

- `make-to-n8n` -- earlier version (JSON-only)
- `n8n-enterprise-automations` -- portfolio of 40+ production n8n workflows

Source: github.com/spotcircuit/make-2-n8n README | Ingested: 2026-04-07

## Related

- [[spotcircuit-services]] -- automation consulting revenue stream
