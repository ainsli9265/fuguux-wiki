---
type: source
title: "WAI-ARIA (Wikipedia)"
tags: [accessibility, wcag, standards, assistive-technology]
related: [wai-aria, wai, accessibility]
created: 2026-06-24
updated: 2026-06-24
authors: [Wikipedia contributors]
year: 2026
url: "https://en.wikipedia.org/wiki/WAI-ARIA"
venue: "Wikipedia"
---

# WAI-ARIA (Wikipedia)

An encyclopedia article on WAI-ARIA, one of the five specification families produced by [[wai]] (already covered for [[wcag]] specifically via two earlier Wikipedia sources). Wikipedia articles are continuously edited, so `year` above reflects the access date (2026-06-24), not a fixed publication year.

## Key points

- Solves a real gap: custom JavaScript-driven controls and partial-page content updates ("rich Internet applications") have no native HTML vocabulary, so screen readers and other assistive technology can't tell what a custom widget is or how its state just changed without extra metadata.
- Adds that metadata as **roles**, **properties**, and **states**, which feed the **accessibility tree** assistive technology actually reads.
- **The Five Rules of ARIA**: prefer native HTML semantics over ARIA when possible; don't override native semantics without good reason; keep all interactive ARIA controls keyboard-usable; don't strip semantics or hide focusable elements; give every interactive element an accessible name.
- Version history confirmed directly against the raw HTML (not just an AI-summarized pass, after the lesson learned from the WCAG 65-vs-61 correction): work began 2006 (first published September 26, 2006); WAI-ARIA 1.0 became a W3C Recommendation March 20, 2014; 1.1 followed December 14, 2017; 1.2 reached Recommendation status June 6, 2023.

## Notes for the wiki

A local snapshot is saved at `raw/safe/wikipedia-wai-aria.html` alongside the live URL. Licensed CC BY-SA 4.0, same treatment as this wiki's other Wikipedia sources — content folded in is paraphrased, not quoted.

Created a new concept page, [[wai-aria]], rather than folding this into [[wai]] or [[accessibility]] — the five-rules hierarchy and the accessibility-tree/roles-states-properties model are substantial enough to warrant their own page, the same judgment call already made for [[wcag]]. Deliberately excluded specific `aria-*` attribute syntax beyond the two named as rule examples, since that crosses into "specific code implementation," out of `purpose.md`'s scope — kept the page at the level of *why* the rules exist and what they're for, not *how* to write the markup.
