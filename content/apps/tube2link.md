# Tube2Link

#apps #tube2link #youtube #linkedin #content

YouTube to LinkedIn post converter. Fetches video metadata, extracts captions via YouTube transcript API, generates AI-powered LinkedIn posts with configurable length.

## Architecture

- **Frontend**: Next.js + TypeScript + Tailwind CSS
- **Auth**: Google OAuth 2.0
- **Captions**: youtube-transcript-api (manual + auto-generated)
- **AI**: Post generation with length control (Brief/Standard/Detailed)

## Flow

Paste YouTube URL -> Fetch metadata + preview -> Extract transcript -> AI generates LinkedIn post (150-500 words) -> Copy to clipboard

Source: github.com/spotcircuit/tube2link README | Ingested: 2026-04-07

## Related

- [[ai-content-pipeline]] -- content generation pattern
- [[sopify]] -- similar pattern (video input -> structured output)
