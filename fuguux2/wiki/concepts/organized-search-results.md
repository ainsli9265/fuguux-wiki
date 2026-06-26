---
type: concept
title: Organized Search Results
tags: [search, design-pattern, usability, accessibility]
related: [search-action-module, straightforward-search-forms, card-sorting, above-the-fold, accessibility, web-design-patterns, amazon, google, ibm, vanduyne-2006-making-site-search-fast-and-relevant, fitts-law, content-organization-schemes]
sources: [vanDuyne_J_3PP_661-676.pdf]
created: 2026-06-24
updated: 2026-06-24
---

# Organized Search Results

**Problem:** a search engine is only as good as the results page it produces — speed and recall don't matter if customers can't make sense of what comes back, whether there are too few hits or too many.

**Solution:**

- **Provide relevant, domain-specific summaries**, not bare links — a restaurant-guide site might show a review excerpt plus food/décor/service/cost ratings; an e-commerce site might show price and availability; a message-board search might show the author and posting date. What belongs in a summary depends entirely on the kind of site.
- **Clearly organize the results** — group hits by a coherent scheme ([[content-organization-schemes|category, alphabetical, chronological]]) rather than presenting a flat list, so customers aren't left sifting through hundreds of undifferentiated hits — see [[amazon]] for an example that groups hits into categories like "Books" and "zShops" rather than one flat list.
- **Give every result a real, descriptive hyperlinked title** — search engines typically just display a page's HTML title as the result's name, so a vague or duplicate title undermines the whole results page regardless of how good the underlying match was.
- **Mine search log files** to find the most common query terms and make sure those terms point to the best possible destination (including a special promoted result alongside the ordinary ones, as [[ibm|IBM]] does for "notebook" and "laptop" searches), and to find and correct the most frequent misspellings — domain-specific terms won't be in a generic dictionary, so this has to be tailored per site. When a likely misspelling is detected, silently search on the corrected term and show those results rather than a bare "no results found," which most customers won't even notice was a correction — [[amazon]] does exactly this, correcting "crossing cashm" to "crossing chasm" rather than reporting no matches.
- **Support common search tasks directly on the results page** — repeat the search box at both the top and the bottom of a long results page (so refining or restarting a search doesn't require scrolling back up), and make pagination targets (e.g., a "Next" link) large rather than a small word, which doubles as an [[accessibility]] win for customers with limited motor control (the same size/distance trade-off [[fitts-law]] formalizes) — see [[google]] for a model results page that does both.

**Forces:** putting search controls at the bottom of a results page can look like it contradicts [[above-the-fold]], but it doesn't — customers read a results page top to bottom, and the bottom controls only matter once they've already scanned everything above and not found what they wanted.

[[card-sorting]] can be used proactively, before launch, to anticipate likely search terms — catching mismatches between customer vocabulary and site terminology ahead of time rather than discovering them later through log-file analysis. This pattern is the natural destination for both [[search-action-module]] and [[straightforward-search-forms]].
