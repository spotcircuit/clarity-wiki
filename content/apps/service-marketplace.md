# Service Marketplace

#apps #service-marketplace #directory #saas #stripe

Niche-agnostic service marketplace platform. JSON-based vertical configuration, business directory with claim flow, lead gen with quote requests, Stripe subscriptions (Free/$99/$299), multi-role auth, SEO engine.

## Architecture

- **Frontend**: Next.js 15.4 + TypeScript + Tailwind CSS + shadcn/ui + Turbopack
- **Database**: Neon PostgreSQL with Row Level Security
- **Auth**: JWT + bcrypt (Customer, Business Owner, Admin roles)
- **Payments**: Stripe (Free / Professional $99 / Premium $299)
- **Demo**: https://dumpsterdiving.netlify.app

## Key Features

Business directory with featured listings, advanced search, ratings/reviews. Quote request system with multi-business quotes. Dealer portal. SEO-optimized state/city pages with Schema.org. Fallback mode works without database.

Source: github.com/spotcircuit/service-marketplace README | Ingested: 2026-04-07

## Related

- [[atlasly]] -- similar concept (schema-driven directory) with Typesense + Mapbox
- [[site-builder-overview]] -- generates individual sites vs marketplace directory
- [[spotcircuit-services]] -- marketplace approach to service business revenue
