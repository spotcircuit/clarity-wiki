# Atlasly

#apps #atlasly #directory #maps #search

Schema-driven, vertical-agnostic business directory. Mapbox GL maps, Typesense geo + faceted search, Prisma + Neon Postgres, Auth.js, Stripe paid placement.

## Architecture

- **Frontend**: Next.js 14 + TypeScript + Tailwind CSS + shadcn/ui
- **Database**: Neon Postgres via Prisma
- **Search**: Typesense (geo + facets + planWeight ranking)
- **Maps**: Mapbox GL
- **Auth**: Auth.js
- **Payments**: Stripe (claim flow + placement)
- **Layout**: web/ subdirectory monorepo

## Routes

- `/directory/[city]/[category]` -- server search + map + facets
- `/listing/[slug]` -- details with claim banner

## Status

Core scaffolding done (Prisma, APIs, Mapbox, routes). Pending: Typesense provisioning, claim flow, Stripe webhooks, vertical config, tests, deploy.

Source: github.com/spotcircuit/atlasly README | Ingested: 2026-04-07

## Related

- [[service-marketplace]] -- similar concept with different search stack
- [[getrankedlocal]] -- directory features overlap
