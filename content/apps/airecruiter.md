# AI Recruiter

#apps #airecruiter #recruiting #ai #saas

Comprehensive AI recruiting platform. Company intelligence, candidate ATS pipeline (Kanban), resume parsing, AI matching with explainable scoring, automated outreach, analytics.

## Architecture

- **Frontend**: Next.js 14 + TypeScript + Tailwind CSS
- **Auth**: NextAuth.js (email, Google, LinkedIn SSO)
- **Database**: Supabase (PostgreSQL)
- **AI**: OpenAI GPT-3.5/4 (parsing, matching, semantic search)
- **Payments**: Stripe
- **State**: Zustand

## Key Modules

- **Company Intelligence**: Discovery, BD pipeline Kanban, ICP builder, CSV import
- **Candidate Management**: ATS pipeline (7 stages), smart matcher, resume parser (PDF + Word)
- **Jobs**: AI-generated descriptions, application tracking, candidate-job matching
- **Analytics**: Pipeline metrics, recruiting KPIs

Source: github.com/spotcircuit/airecruiter README | Ingested: 2026-04-07

## Related

- [[spotcircuit-services]] -- potential SaaS product line
