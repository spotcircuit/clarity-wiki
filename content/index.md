# Clarity Wiki

The knowledge base for SpotCircuit's agentic AI engineering practice. Built on the Karpathy LLM Wiki pattern.

---

## SpotCircuit
- [[clarity-framework]] -- Open-source agentic intelligence framework. Self-learn loop, 9 commands, 3 knowledge systems.
- [[spotcircuit-services]] -- The 6 revenue streams: framework licensing, AI consulting, Claude Code, knowledge bases, pipelines, build in public.

## Patterns
- [[correlation-id]] -- Track execution across services and logs. Single most important debug tool.
- [[idempotency-guard]] -- Status gate prevents duplicate processing.
- [[error-handling]] -- Catch errors, log them, write status back to source record.
- [[config-driven-routing]] -- Routing logic in config records, not code. Zero code changes to add types.
- [[mock-data-strategy]] -- Mock toggle for external APIs without sandboxes.
- [[pre-release-checklist]] -- Every production release gate.
- [[cloudflare-pages-deploy]] -- Deploy static sites to CF Pages with auto project limit management.
- [[websocket-progress-pattern]] -- Real-time pipeline progress via WebSocket broadcast.
- [[inline-editor-pattern]] -- Post-generation editing with live iframe preview + rebuild.
- [[act-learn-reuse-testing]] -- Self-improving test loop: run, extract failures, feed knowledge back.
- [[scout-build-verify]] -- Three-agent workflow: scout analyzes, builder implements, verifier validates.

## Platform
- [[site-builder-overview]] -- Google Maps to deployed React site in 60s. Full pipeline.
- [[ai-content-pipeline]] -- Claude for copy + Gemini for images. Config-driven, model-swappable.
- [[paperclip-integration]] -- Paperclip orchestration layer for Clarity agents.
- [[orchestrator-3-stream]] -- (Reference) Pre-Paperclip multi-agent orchestrator. Superseded.
- [[lead-finder]] -- (Reference) Multi-source lead scraper + AI pitch gen.
- [[listing-launch]] -- (Reference) Real estate multi-channel content generator.
- [[getrankedlocal]] -- Google Maps 169-point grid ranking analysis + lead gen platform.

## Decisions
- [[karpathy-wiki-comparison]] -- LLM Wiki vs Clarity. Gaps, advantages, bridge plan.
- [[multi-format-ingest-strategy]] -- Config-driven + AI hybrid for normalizing data formats.
