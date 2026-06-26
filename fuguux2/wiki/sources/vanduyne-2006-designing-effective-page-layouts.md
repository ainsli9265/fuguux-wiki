---
type: source
title: "Designing Effective Page Layouts (Pattern Group I, The Design of Sites)"
tags: [design-patterns, layout, page-structure]
related: [grid-layout, above-the-fold, clear-first-reads, expanding-and-fixed-screen-width, consistent-sidebars-of-related-content, web-design-patterns, homepage-portal]
created: 2026-06-24
updated: 2026-06-24
authors: [van Duyne, Landay, Hong]
year: 2006
url: ""
venue: "The Design of Sites (2nd ed.), Pattern Group I, pp. 631-660"
---

# Designing Effective Page Layouts

Pattern Group I of *The Design of Sites* — six patterns (I1-I6) for giving a Web page a clear, predictable structure. Documents all six in full six-part format, per [[web-design-patterns]].

## Key points

- [[grid-layout]] (I1) — organizing a page's competing elements into a consistent row/column structure that customers can learn to predict.
- [[above-the-fold]] (I2) — what must be visible without scrolling, and why the Web's variable screen sizes make this a harder problem than it was in print.
- [[clear-first-reads]] (I3) — finally gives full-pattern depth to "first read," a term this wiki had previously only referenced in passing (in [[homepage-portal]]) and explicitly flagged as a documentation gap in the 2026-06-24 lint pass.
- [[expanding-and-fixed-screen-width]] (I4 + I5) — combined into one page since the book always presents these two as a direct contrast with each other.
- [[consistent-sidebars-of-related-content]] (I6) — where and how to place links to related content so visitors actually notice them.

## Notes for the wiki

PAGE TEMPLATE (D1) is referenced by every single pattern in this chapter — it's described as the umbrella pattern all six of I1-I6 contribute to — but it's never itself explained here; it lives in the not-yet-ingested Pattern Group D. This is now a stronger documentation gap than SITE BRANDING (E1) / PRIVACY POLICY (E4), flagged in earlier sessions, given how central it evidently is; prioritize Pattern Group D next if a choice has to be made.

No new entities. CNN.com appears here as a screenshot example (I6, sidebars) — its third incidental mention across ingested sources (after the Ch. 1/Ch. 2 "durability" lists) — but it's still just a name-drop or screenshot each time, never a substantive paragraph the way Yahoo! got in Chapter 1, so it stays below the entity threshold for now; worth reconsidering if a future source adds real depth. Lands' End, Williams-Sonoma, Outpost.com, iWon, CNET News.com, IFILM, Beliefnet, the EPA, and Wichita State University (the placement-expectation research cited in both [[grid-layout]] and [[above-the-fold]]) are all single-source incidental examples.

Heavy implementation content — HTML table-width syntax and style-sheet code for I4/I5, and a table-border debugging trick for I1 — was excluded per `purpose.md`'s "specific code implementation" rule; only the underlying design rationale was kept.
