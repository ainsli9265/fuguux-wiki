---
type: source
title: "Fitts's Law (Wikipedia)"
tags: [hci-law, motor-control, accessibility, human-factors]
related: [fitts-law, know-your-customers, accessibility]
created: 2026-06-24
updated: 2026-06-24
authors: [Wikipedia contributors]
year: 2026
url: "https://en.wikipedia.org/wiki/Fitts%27s_law"
venue: "Wikipedia"
---

# Fitts's Law (Wikipedia)

A dedicated encyclopedia article on Fitts's Law — previously only a one-sentence, below-threshold mention in this wiki (from [[vanduyne-2006-knowing-your-customers]] and the book's glossary), now substantial enough to justify its own concept page, [[fitts-law]]. Wikipedia articles are continuously edited, so `year` above reflects the access date (2026-06-24), not a fixed publication year.

## Key points

- Paul Fitts published the original 1954 study in the *Journal of Experimental Psychology*, proposing a way to quantify how hard a target-selection task is.
- Movement time depends on distance to the target and the target's width, following MT = a + b·log₂(2D/W) — the log₂(2D/W) term is the **index of difficulty**.
- Design implications well beyond "make buttons bigger": the rule of the infinite edges (a target flush against a screen edge is effectively infinite in size along that edge — why macOS puts its menu bar at the very top), "magic corners" (where two infinite edges meet, exploited by Windows/Office for high-value controls), touchscreen target sizing, and handedness effects in radial/pie menus.
- Related laws: Hick's Law (decision time vs. number of choices), the Accot–Zhai steering law (extending Fitts's Law to constrained-path navigation like hierarchical menus), and throughput (bits/second, combining difficulty and time).
- Documented limitations: predictive accuracy degrades when distance and width both vary widely in the same comparison; the 1D formulation needs adjustment for real 2D pointing; applying it to eye-tracking/gaze interaction is contested, since saccadic eye movement isn't the same kind of motor act as a deliberate hand movement.

## Notes for the wiki

A local snapshot is saved at `raw/safe/wikipedia-fittss-law.html` alongside the live URL. Licensed CC BY-SA 4.0, same treatment as this wiki's other Wikipedia sources — content folded in is paraphrased, not quoted.

**What was left out, and why** (per `schema.md`'s ingestion-report requirement): the full mathematical derivation and the Shannon-formulation history behind the index-of-difficulty formula were excluded as more information-theory than UX design — [[fitts-law]] keeps the formula but not its derivation. Specific numeric studies/citations validating or critiquing the law in particular populations (cited in the article's body but not summarized above) were also left out as academic-literature detail rather than a design-relevant fact. Everything else from the `WebFetch` summary was used; nothing was excluded for being out of `purpose.md`'s scope outright, since this entire article is squarely a design heuristic.

This is another case of a "mentioned but below threshold" topic getting reconsidered once a dedicated source appeared — same pattern as the [[wcag]]/[[wai-aria]] splits. Updated [[know-your-customers]], [[accessibility]], [[organized-search-results]], and [[action-buttons]] to link the new page where each already discussed the underlying idea without naming it.

Reclassified [[fitts-law]] from `entity` to `concept` (2026-06-25) after `schema.md` was updated to classify laws as concepts rather than entities.
