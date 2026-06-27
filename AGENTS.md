# Agent Instructions

This repository is a technical deep-dive wiki about JPEG XL. Your job is to
maintain a durable, cited, interconnected Markdown knowledge base, not just to
answer one-off questions.

## Project Model

- `wiki/` contains synthesized pages. Agents may create and rewrite these pages.
- `sources/` contains link-only source cards. Treat these as evidence records.
- `questions/` contains durable answers or analyses produced from research
  questions.
- `notes/` contains temporary work products, triage notes, and scratch synthesis.
- `wiki/log.md` is append-only. Never rewrite past entries unless the user
  explicitly asks for history cleanup.
- `external/` contains third-party material. Do not edit it directly unless the
  task is specifically to update a submodule or external dependency.

## Default Workflow

Use one-source-at-a-time ingestion unless the user explicitly requests batch
work.

1. Read `wiki/index.md`, `sources/index.md`, and any relevant existing wiki pages.
2. Add or update the source card in `sources/` before changing synthesized pages.
3. Update every affected wiki page, including backlinks and related-page lists.
4. Update `wiki/index.md` and `sources/index.md`.
5. Append one parseable entry to `wiki/log.md`.
6. Check `git diff` and verify no unrelated files were changed.

For query-driven work, answer from the wiki first, then consult sources or the
web if the wiki is incomplete or the fact is likely to have changed. If the
answer adds durable knowledge, file it under `questions/` or integrate it into
the relevant `wiki/` pages.

## Claim Policy

- Technical claims should cite a source card or primary source link.
- Adoption, browser support, ecosystem support, release, or market claims must
  include an access date.
- Prefer primary sources: official JPEG pages, ISO metadata, libjxl docs,
  browser/platform status pages, implementation docs, and project release notes.
- If a source is secondary or advocacy-oriented, label it as such in the source
  card and avoid presenting its conclusions as neutral fact.
- If sources disagree, preserve the disagreement in the relevant page and add or
  update `wiki/Open Questions.md`.
- Keep quotations short. Prefer synthesis and citations over copied passages.

## Page Conventions

- Use Obsidian-style links for wiki pages, such as `[[libjxl]]`.
- Start each wiki page with a short summary paragraph.
- Use these sections where they fit: `## Key Points`, `## Details`,
  `## Sources`, and `## Related Pages`.
- Keep source URLs in source cards. Wiki pages may cite source card names and
  short inline links when useful.
- Favor concise, high-signal synthesis over exhaustive dumps.
- Do not leave unsupported TODO claims in wiki pages; put uncertainty in
  `wiki/Open Questions.md`.

## Source Card Template

```markdown
# Source Title

- URL:
- Publisher / author:
- Publication date:
- Accessed:
- Source type:
- Reliability tier:
- Local archive: none; link-only

## Summary

## Key Claims

## Pages Impacted
```

Reliability tiers:

- `primary`: standards bodies, official project docs, source repositories,
  vendor platform-status pages, release notes.
- `secondary`: technical articles, benchmark reports, documentation by tooling
  vendors, issue trackers with useful context.
- `tertiary`: summaries, blog commentary, social posts, or unsourced lists.

## JPEG XL Coverage Priorities

Maintain coverage across these areas:

- Standardization and specification structure.
- Codestream and container concepts.
- Coding tools and image model.
- Lossless JPEG recompression and migration.
- HDR, wide gamut, alpha, animation, layers, and progressive decoding.
- Reference implementation, CLI tools, APIs, build behavior, and licensing.
- Browser, OS, application, CDN, and tooling support.
- Comparisons with JPEG, PNG, WebP, AVIF, HEIC, JPEG 2000, and JPEG XS.
- Adoption history, controversy, and unresolved claims.
