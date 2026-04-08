# WeatherProof

#apps #weatherproof #construction #weather #insurance

Automated weather delay tracking and insurance claim generation for construction companies. NOAA weather monitoring, photo documentation, PDF reports, cost calculations, analytics.

## Architecture

- **Frontend**: Next.js 15 + React 18 + TypeScript + shadcn/ui
- **Backend**: Supabase (PostgreSQL, Auth, Storage)
- **Weather**: NOAA Weather Service API
- **PDF**: jsPDF + html2canvas
- **Deployment**: Vercel

## Key Features

Real-time NOAA weather collection. Delay documentation with photos. Professional insurance PDFs with weather verification. Auto cost calculations (labor, equipment, overhead). Bulk CSV import/export.

## Variants

- `weatherproof` -- full version with Supabase
- `weatherproof-lite` -- lightweight with Drizzle ORM, in-memory mode, Chrome extension architecture
- n8n workflow -- WeatherProof Alert System (16 nodes, active 24/7)

Source: github.com/spotcircuit/weatherproof README | Ingested: 2026-04-07

## Related

- [[spotcircuit-services]] -- SaaS for construction vertical
