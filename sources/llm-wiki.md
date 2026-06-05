---
title: LLM Wiki
type: source
created: 2026-05-20
updated: 2026-05-20
sources:
  - raw/llm-wiki.md
tags:
  - knowledge-base
  - llm-agent
  - wiki
---

# LLM Wiki

## Summary

The source proposes a pattern for using an LLM agent to maintain a persistent markdown wiki from raw documents. Instead of relying only on retrieval at question time, the agent reads sources once, extracts durable knowledge, updates interlinked pages, flags contradictions, and keeps a compounding knowledge base current over time.

## Key Claims

- A persistent wiki gives the LLM accumulated context that does not need to be rediscovered on every query.
- Raw sources should remain immutable and serve as the source of truth.
- The LLM should own the generated wiki layer: summaries, entity pages, concept pages, cross-references, and syntheses.
- `AGENTS.md` or an equivalent schema file is the key configuration that turns a generic LLM into a disciplined wiki maintainer.
- Useful operations include ingesting sources, querying the wiki, and linting the knowledge base for health issues.

## Connections

- [[persistent-llm-wiki]]

## Open Questions

- What domain should this wiki specialize in first?
- Should the workflow prefer one-source-at-a-time ingest or batch ingest?
- Should this workspace add search tooling later, such as a markdown search CLI or MCP server?

