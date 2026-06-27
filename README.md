# JPEG XL LLM Wiki

This repository is a persistent, LLM-maintained knowledge base about JPEG XL.
It is organized as a technical deep dive for engineers, codec researchers, and
readers who want durable context on the format, reference implementation,
standardization, adoption, and tradeoffs.

The repository follows the pattern described in
`external/llm-wiki.md/llm-wiki.md`: raw source metadata is kept separately from
synthesized wiki pages, and future agents maintain the wiki by ingesting one
source at a time.

## Start Here

- `AGENTS.md`: operating instructions for future agents.
- `wiki/index.md`: map of synthesized wiki pages.
- `sources/index.md`: catalog of source cards.
- `wiki/log.md`: append-only activity log.

## Repository Layout

- `wiki/`: synthesized JPEG XL pages maintained by agents.
- `sources/`: link-only source cards with metadata and key claims.
- `questions/`: durable answers to research questions worth preserving.
- `notes/`: temporary working notes and triage lists.
- `external/`: third-party references, including the LLM wiki pattern submodule.

This repo intentionally stores source cards rather than full source archives.
If a source later needs to be preserved locally, document that exception in the
source card and in `wiki/log.md`.
