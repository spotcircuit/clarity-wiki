# LinkedIn Post: 2026-04-08 — clarity

#linkedin #content #clarity #spotcircuit

Posted to LinkedIn on 2026-04-08. Topic: clarity.

## Post Content

Three weeks. That's how long most engineers burn just figuring out what a client's stack actually looks like before they write a single useful line of code.

I got tired of that tax. So I built Clarity and open-sourced it.

The seed was Andrej Karpathy's LLM Wiki pattern, structured knowledge that an AI reads before it answers anything. Good idea. But a static wiki only gets you so far.

Clarity layers three things on top. First, operational data in a structured YAML file that captures project state right now, not last quarter. Second, behavioral memory so the system knows how your team actually works (preferences, guardrails, the stuff that lives in someone's head). And third, a self-learn loop where raw observations validate against live state and auto-promote into real knowledge. No manual curation.

The result? Full project context on day one. And it compounds. Every session makes the system smarter.

It's 9 slash commands. An Obsidian-compatible wiki. Runs with Claude Code out of the box. Nothing fancy to set up.

I built this because I kept solving the same onboarding problem over and over. Now I don't.

GitHub: https://github.com/spotcircuit/clarity-framework

#OpenSource #AgenticAI #KnowledgeManagement #ClaudeCode #LLM

## Related

- [[site-builder-overview]]
- [[ai-content-pipeline]]

---
Source: system/drafts/linkedin-2026-04-08-clarity.md | Filed: 2026-04-08
