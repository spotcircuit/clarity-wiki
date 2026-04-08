# SEO Snap

#apps #seosnap #seo #audit #ai

AI-powered SEO audit tool. Playwright page analysis, 9 technical SEO validators, Google Lighthouse Core Web Vitals, GPT-5 Nano recommendations. Audit history, report comparison, markdown export.

## Architecture

- **Frontend**: Next.js 14 + TypeScript + Tailwind CSS
- **Database**: Neon PostgreSQL or SQLite via Prisma
- **Browser**: Playwright + @sparticuz/chromium (serverless)
- **AI**: OpenAI GPT-5 Nano (structured JSON recommendations)
- **Performance**: Google PageSpeed Insights API (Lighthouse)

## Score Calculation

Composite: SEO checks (40%) + Lighthouse metrics (60%). 9 validators: title, meta description, canonical, robots, headings, images, OG, Twitter Cards, Schema.org.

Source: github.com/spotcircuit/seosnap README | Ingested: 2026-04-07

## Related

- [[getrankedlocal]] -- complementary SEO tool (grid rankings vs page audits)
- [[site-builder-overview]] -- generated sites could be audited by SEO Snap
