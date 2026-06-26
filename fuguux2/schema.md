# Wiki Schema

## Page Types

| Type       | Directory         | Purpose                                               |
| ---------- | ----------------- | ----------------------------------------------------- |
| entity     | wiki/entities/    | Named things (people, tools, organizations, datasets) |
| concept    | wiki/concepts/    | Ideas, techniques, frameworks, laws                   |
| source     | wiki/sources/     | Papers, articles, talks, books, blog posts            |
| query      | wiki/queries/     | Open questions under active investigation             |
| comparison | wiki/comparisons/ | Side-by-side analysis of related entities             |
| synthesis  | wiki/synthesis/   | Cross-cutting summaries and conclusions               |
| overview   | wiki/             | High-level project summary (one per project)          |

## Naming Conventions

- Files: `kebab-case.md`
- Entities: match official name where possible (e.g., `openai.md`, `gpt-4.md`)
- Concepts: descriptive noun phrases (e.g., `chain-of-thought.md`)
- Sources: `author-year-slug.md` (e.g., `wei-2022-cot.md`)
- Queries: question as slug (e.g., `does-scale-improve-reasoning.md`)

## Frontmatter

All pages must include YAML frontmatter:

```yaml
---
type: entity | concept | source | query | comparison | synthesis | overview
title: Human-readable title
tags: []
related: []
created: YYYY-MM-DD
updated: YYYY-MM-DD
---
```

Source pages also include:
```yaml
authors: []
year: YYYY
url: ""
venue: ""
```

Concept, query, comparison, and synthesis pages that draw on one or more sources also include:
```yaml
sources: []
```
- `sources:` lists the actual raw file name(s) (pdf/html, matching files in `raw/safe/`) that a page draws on — not source-page slugs. Exception: for sources with a live URL (e.g. Wikipedia articles), cite the URL itself rather than the local snapshot's filename, even though a snapshot is still kept in `raw/safe/` for reference.
- `related:` lists other concept/query/comparison/synthesis pages the page is conceptually related to, **and** the slug(s) of any `wiki/sources/` page(s) it draws on.
- This keeps `sources:` pointing at the underlying raw document (useful for re-checking a claim against the original file) while `related:` remains the single place to look for every page-to-page link, including citations.

## Index Format

`wiki/index.md` lists all pages grouped by type. Each entry:
```
- [[page-slug]] — one-line description
```

## Log Format

`wiki/log.md` records activity in reverse chronological order:
```
## YYYY-MM-DD

- Action taken / finding noted
```

When the action is a source ingestion, the entry must summarize **both sides** of the scope decision, not just what got added:
- What was extracted/folded in, and into which pages.
- What was deliberately left out, grouped by why — e.g. "specific code implementation" or another named exclusion from `purpose.md`'s scope, "below the page-creation threshold" (named but only a sentence deep), "legal/litigation reference rather than design guidance," or "no new substance over an existing mention." Naming a concrete reason, not just "left out," is what lets a later session judge whether that call still holds without re-reading the source.

This applies to every ingestion, including ones where everything fit `purpose.md`'s scope — in that case, say so explicitly (e.g. "nothing excluded; all of it was in scope") rather than leaving the omission silent and ambiguous.

## Source Triage (`raw/`)

New source files land in `raw/` and must be sorted before any extraction work begins.

1. **Determine copyright status**, then **confirm with the user** which bucket it belongs in before moving the file:
   - **Safe**: public domain (e.g. expired copyright, U.S. federal government works under 17 U.S.C. § 105) or covered by an explicit open license (CC0, CC-BY, MIT, etc. — cite which one).
   - **Copyrighted**: everything else, including material that's free to read/download but carries no stated license. Free of charge does not imply public domain — require an actual license or public-domain basis, not just the absence of a paywall.
2. **Move the file** into the matching folder — `raw/safe/` or `raw/copyrighted/` — before doing any further work.
3. **Then treat it per its folder:**
   - **`raw/safe/`** → ingest normally: extract entities/concepts per `purpose.md`'s scope and the Page Creation Thresholds below, create a source page, and update `index.md`, `overview.md`, and `log.md`.
   - **`raw/copyrighted/`** → do **not** create a source page; do **not** add it to any page's `sources:` frontmatter. You **may** create new concept/entity pages (and add them to `index.md`) if the copyrighted source introduces a concept or entity that meets the Page Creation Thresholds — but the copyrighted source's specific content must not appear in the page body. Instead, place a `## Further reading` section at the bottom of the page (new or existing) with a plain-text pointer to the source: raw file path under `raw/copyrighted/`, a URL, or both, plus author/title, license status, and a one-to-two sentence summary of what the source adds beyond what the page body already says. The body itself should draw only on common knowledge or other safe sources already in the wiki; it is acceptable for the body to be empty (title + `## Further reading` only) if all substantive content belongs to the copyrighted source. Do not reproduce or closely paraphrase the copyrighted source's text anywhere on the page. Skip the further-reading note where the connection is tenuous; a missing note is better than a forced one. Still record the triage decision and any pages created or updated in `log.md`.

     **What counts as common knowledge:** A claim passes the bar if it can be independently sourced — to a Wikipedia article, published design guidelines (e.g. Nielsen Norman Group, WCAG, Material Design documentation), an established UX textbook, or another safe source already in this wiki — without citing the copyrighted source. If the only path to the claim runs through the copyrighted source, it belongs in `## Further reading`, not the body.

     **Specific red flags** — move these to `## Further reading` even if individual sentences might seem defensible:
     - Numeric thresholds, timing values, or counts the source introduced or popularized (e.g. "≤7 options," "500ms delay")
     - Named psychological effects or principles applied to a design pattern *in a way the source itself draws the connection* — even if the effect is independently known
     - Step-by-step implementation techniques the source describes (techniques belong in Further reading; the underlying principle may stay in the body)
     - Numbered lists of problems or failure modes whose structure mirrors the source's own structure

     **Self-check:** after writing any body paragraph, ask "how would I source this without the copyrighted material?" If the honest answer is "I can't — I know it from the source," move it to `## Further reading`. The test is not "is this true in general?" but "did I learn it from this source specifically?"

4. **Media** (images, screenshots, diagrams, etc.) extracted from a source while ingesting it go in `raw/media/<source-page-slug>/` — a subfolder named for the matching `wiki/sources/` page slug (e.g. `raw/media/wikipedia-2026-affordance/`), create this folder at ingestion time. This applies regardless of which bucket the source itself landed in (`raw/safe/` or `raw/copyrighted/`); the copyrighted-source restrictions above (no source page, no `sources:` frontmatter entries) still apply to copyrighted media.

## Page Creation Thresholds

* **Entities**: only create a dedicated page and list it in index.md if the entity appears in 2+ sources.
  Incidental mentions should be inline text, not pages.

* **Concepts**: only create a page if the concept requires explanation beyond
  a sentence.

* **Prefer updating existing pages** over creating new ones. Before creating any
  page, check index.md for a closely related existing page and expand it instead.

## Cross-referencing Rules

- Use `[[page-slug]]` syntax to link between wiki pages, only link a page if it actually exists in the wiki, do not link a page within itself
- Every entity and concept page should appear in `wiki/index.md`
- Queries link to the sources and concepts they draw on
- Synthesis pages cite all contributing source pages via `related:`, and list the underlying raw file names in `sources:`

* The text inside `[[...]]` must exactly match the filename without the `.md`
  extension, including hyphens, capitalization, and any year/author prefix.

* When in doubt, prefer plain text over a wikilink. A missing link is less
  harmful than a broken one.

* Never paraphrase or abbreviate a slug when linking
  (e.g. use `[[wei-2022-cot]]` not `[[wei-2022]]` or `[[cot-paper]]`).

## Contradiction Handling

When sources contradict each other:
1. Note the contradiction in the relevant concept or entity page
2. Create or update a query page to track the open question
3. Link both sources from the query page
4. Resolve in a synthesis page once sufficient evidence exists
