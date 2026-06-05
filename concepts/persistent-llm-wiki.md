---
title: Persistent LLM Wiki
type: concept
created: 2026-05-20
updated: 2026-05-20
sources:
  - wiki/sources/llm-wiki.md
tags:
  - knowledge-base
  - agent-workflow
---

# Persistent LLM Wiki

## Summary

A persistent LLM wiki is a markdown knowledge base maintained by an LLM agent. It sits between raw sources and user questions, turning documents into durable, linked, updated pages rather than treating every question as a fresh retrieval task.

## Key Ideas

- The wiki compounds: source summaries, entity pages, concept pages, and syntheses become reusable context.
- The agent updates existing pages when new sources arrive, rather than creating isolated summaries.
- Contradictions and uncertainty should be documented explicitly.
- Strong index and log files let the wiki remain navigable without requiring heavy retrieval infrastructure at small or medium scale.

## Workflow

1. Put immutable sources in `raw/`.
2. Ingest sources into `wiki/sources/`.
3. Update relevant `wiki/entities/` and `wiki/concepts/` pages.
4. File substantial analyses in `wiki/syntheses/`.
5. Keep `wiki/index.md` and `wiki/log.md` current.

## Related Pages

- [[llm-wiki]]

