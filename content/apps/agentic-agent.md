# Agentic Agent

#apps #agentic-agent #orchestration #multi-agent #claude

Production-ready web-based multi-agent orchestration. Manages multiple Claude Code agents at scale with real-time WebSocket streaming, PostgreSQL persistence, event logging, and automatic cost tracking.

## Architecture

- **Backend**: Python 3.12+ (uv package manager)
- **Frontend**: Bun runtime (Node.js 18+)
- **Database**: PostgreSQL (NeonDB or Docker)
- **AI**: Claude Code ecosystem
- **Real-time**: WebSocket streaming
- **Observability**: Full event + cost tracking

## Key Features

Natural language control of multiple agents. Orchestrator agent manages specialized agents. Every event, cost, and interaction tracked. Per-agent token usage and USD totals.

Source: github.com/spotcircuit/agentic_agent README | Ingested: 2026-04-07

## Related

- [[paperclip-integration]] -- Paperclip agent orchestration (5 agents)
- [[orchestrator-3-stream]] -- earlier pre-Paperclip orchestrator
- [[clarity-framework]] -- could become Clarity's orchestration layer
