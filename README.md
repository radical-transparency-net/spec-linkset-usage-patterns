# Radical Transparency — Linkset Usage Patterns Specification (`RT-P01` to `RT-P10`)

Canonical specification repository for the **Radical Transparency Linkset Usage Patterns** (`RT-P01` through `RT-P10`), rendered as a W3C-style specification via [ReSpec](https://respec.org/docs/).

- **Live ReSpec Specification (GitHub Pages):** `https://radical-transparency-net.github.io/spec-linkset-usage-patterns/`
- **Companion RDF Vocabulary (`rtwl:`):** `https://github.com/radical-transparency-net/semantic-assets`

---

## Specification Structure

- [`index.html`](index.html) — ReSpec entry point assembling the overview and all 10 patterns via `data-include` with `data-include-format="markdown"`.
- [`rt-patterns-overview.md`](rt-patterns-overview.md) — Master Overview, Problem Statement, Semantic Bridge (`rtwl:`), Resource vs. Representation Profiling, and Reading Paths.
- [`rt-p01-profile-declaration.md`](rt-p01-profile-declaration.md) – [`rt-p10-detached-local-storage.md`](rt-p10-detached-local-storage.md) — Individual pattern specifications (`RT-P01` to `RT-P10`).
- `rt-patterns-*.svg` & `rt-p01-*.svg` – `rt-p09-*.svg` — Architectural diagrams referenced in both standalone Markdown and the ReSpec document.
- [`master-links.md`](master-links.md) — Shared Markdown reference link definitions.

---

## Local Preview & PDF Export

Because ReSpec fetches external Markdown files via `fetch()` (`data-include`), browsers block `file://` URLs. Serve the repository over HTTP locally:

```bash
python3 -m http.server 8080
```

Then open `http://127.0.0.1:8080/` in your browser.

To export a static HTML snapshot or print-ready PDF, use ReSpec's built-in **ReSpec &rarr; Export &rarr; HTML** pill in the top-right corner or the browser's **Print &rarr; Save as PDF** (page breaks between patterns are preconfigured via `@media print`).
