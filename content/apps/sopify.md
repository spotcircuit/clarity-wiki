# SOPify

#apps #sopify #loom #notion #sop #n8n

Converts Loom videos into structured Notion SOPs. Direct URL conversion, keyword search, folder navigation. Uses n8n webhooks for processing with Google CSE fallback.

## Architecture

- **Frontend**: Next.js 14 + TypeScript + Tailwind CSS + Heroicons
- **Processing**: n8n webhooks at n8n.spotcircuit.com
- **Fallback**: Google Custom Search Engine
- **Parsing**: Cheerio (HTML extraction)
- **Output**: Notion API (SOP creation)

## Flow

Paste Loom URL or search by keyword -> n8n webhook extracts transcript -> Converts to structured SOP -> Creates Notion page

Source: github.com/spotcircuit/SOPify README | Ingested: 2026-04-07

## Related

- [[spotcircuit-services]] -- knowledge base builder revenue stream
- [[ai-content-pipeline]] -- content transformation pattern
