---
type: source
title: "Card Sorting (Wikipedia)"
tags: [information-architecture, customer-research, methodology]
related: [card-sorting, customer-research-methods]
created: 2026-06-24
updated: 2026-06-24
authors: [Wikipedia contributors]
year: 2026
url: "https://en.wikipedia.org/wiki/Card_sorting"
venue: "Wikipedia"
---

# Card Sorting (Wikipedia)

Wikipedia's article on card sorting, a knowledge-elicitation method for understanding how people mentally categorize information, used to design information architecture, navigation, and menu structure.

## Key points

- **Basic method.** A representative participant receives index cards bearing item names, groups them in whatever way seems logical, and names each group; this repeats across several participants, and the results are analyzed afterward for patterns (a category tree, or "dendrogram").
- **Open card sorting** (generative): participants invent their own category names — reveals both how people classify items and what words they use for the categories, useful for discovering a new organizational scheme.
- **Closed card sorting** (evaluative): participants sort into a fixed, predetermined set of category names — reveals how much agreement there is on what belongs where, useful for judging an existing or proposed scheme rather than generating one.
- **Reverse card sorting**, more commonly called **tree testing**: tests an existing category hierarchy in isolation. Participants are given a task and have to find the right place for it by navigating the card-based hierarchy from the top down, with none of a real site's navigational aids (search, breadcrumbs) — isolates whether the structure itself, not the UI around it, supports the task.
- **Modified-Delphi card sorting** (created by Celeste Paul): only the first participant does a full independent sort; each subsequent participant iterates on the previous participant's result rather than starting over. Builds consensus with fewer participants than independent sorting.
- **Analysis** falls into two families: **semantic** methods examine the labels/descriptions participants gave (e.g. *gist analysis*, grouping differently-worded labels that mean the same thing — "Difficult to understand" and "Confusing"); **syntactic** methods examine the structure of the sorts themselves — card-based analysis builds similarity/dissimilarity matrices of which cards landed together, feeding cluster analysis and dendrograms; sort-based analysis measures the "edit distance" (card moves needed to turn one participant's sort into another's, calculable via the Hungarian algorithm) between whole sorts.
- **Online/remote card sorting**: web-based tools reach more participants at lower cost and can automate analysis, but lose the moderator's ability to ask a participant *why* they grouped something a certain way.

## Notes for the wiki

A local snapshot is saved at `raw/safe/wikipedia-card-sorting.html` alongside the live URL. Licensed CC BY-SA 4.0, same treatment as this wiki's other Wikipedia sources — content folded in is paraphrased, not quoted.

This wiki already has a concept page for this exact topic, [[card-sorting]] (paired with affinity diagramming), so rather than create a duplicate, folded this article's new material directly into it: the open/closed distinction, reverse card sorting (tree testing), Modified-Delphi card sorting, a brief note on semantic vs. syntactic analysis, and the remote/online tradeoff.

**Excluded:** the deeper statistical mechanics of syntactic analysis (the Hungarian algorithm's actual computation, orthogonality's minimum-spanning-tree formula, multidimensional scaling) — named so a reader recognizes the terms, but not derived, since the math itself is outside `purpose.md`'s design-practice scope; the "See also" pointers to cluster analysis, group concept mapping, and Q methodology as general statistical/research techniques rather than card-sorting-specific content; and citation-level bibliographic detail (e.g. the specific Nielsen and Maurer/Warfel references), beyond crediting Celeste Paul by name for the one technique she's specifically credited with originating.
