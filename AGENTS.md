# AI Agent Guidelines & Repository Directives (`AGENTS.md`)

This repository (`radical-transparency-net/spec-linkset-usage-patterns`) holds the canonical specification for the **Radical Transparency Linkset Usage Patterns (RT-P01 to RT-P10)**, assembled using [ReSpec](https://respec.org/docs/).

---

## 1. Authoritative Directives

- **Strictly English Repository Artifacts:** All specification text, diagrams, documentation, HTML wrapper code, and commit-ready notes must be written in clear, factual English.
- **Canonical Markdown + SVG Sources:** Keep `rt-patterns-overview.md`, `rt-p01-*.md` through `rt-p10-*.md`, and `rt-*.svg` diagrams in the root alongside `index.html` so relative links (`./rt-p01-profile-declaration.svg`) resolve identically on GitHub and inside ReSpec.
- **Dual-Mode Link Hygiene:** Keep standalone Markdown relative links valid (e.g., `./rt-p01-profile-declaration.md`) and update `PATTERN_ID_MAP` in `index.html` if pattern filenames or section IDs change.
- **Zero Secrets:** Never commit credentials, tokens, or local IDE overrides (`.agents/local/**` and `.agents/rules/local-*` are git-ignored).

---

## 2. Verification Before Completion

Before declaring specification or ReSpec edits complete:

1. Verify all `data-include` Markdown files and referenced SVG images exist locally with zero broken relative paths.
2. Serve over local HTTP (`python3 -m http.server 8080`) and inspect `index.html` in a browser (checking ReSpec rendering, TOC generation, SVG diagrams, and zero console errors).
