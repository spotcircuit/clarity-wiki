# Orchestrator 3 Stream

#apps #reference #orchestrator #pre-paperclip

Multi-agent orchestration platform with real-time WebSocket streaming, PostgreSQL persistence, and chat autocomplete expert. **Pre-Paperclip** — built before Paperclip existed, now superseded for orchestration duties.

## What It Does

Web UI for coordinating multiple Claude Code agents. Agents stream responses in parallel, share a PostgreSQL database, and learn from chat interactions via an autocomplete expert pattern.

## Stack

FastAPI + Vue 3 + Claude SDK + PostgreSQL

## Location

`/home/spotcircuit/agentic/agent-experts/apps/orchestrator_3_stream/`

## Patterns Worth Referencing

- **Event streaming UI** — Real-time multi-agent response streaming via WebSocket
- **Autocomplete expert** — Agent learns from chat history, suggests completions
- **Shared database schema** — Single source of truth across agents (see orchestrator_db)
- **Agent wiring** — How to connect multiple Claude Code instances to a shared context

## Status

Superseded by [[paperclip-integration]] for orchestration. Code remains as pattern reference.

## Related

- [[paperclip-integration]] -- current orchestration platform
- [[websocket-progress-pattern]] -- similar real-time pattern used in site-builder
- [[site-builder-overview]] -- was previously managed by this orchestrator

---
Source: agent-experts/apps/orchestrator_3_stream/ | Ingested: 2026-04-08
