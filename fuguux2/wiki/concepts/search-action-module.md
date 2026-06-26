---
type: concept
title: Search Action Module
tags: [search, navigation, design-pattern]
related: [web-design-patterns, action-buttons, vanduyne-2006-web-design-patterns, straightforward-search-forms, organized-search-results, vanduyne-2006-making-site-search-fast-and-relevant]
sources: [vanDuyne_02_3PP_019-038.pdf, vanDuyne_J_3PP_661-676.pdf]
created: 2026-06-23
updated: 2026-06-24
---

# Search Action Module

**Problem:** customers who know exactly what they want need a fast way to jump to it, but a full search page is often too complex to be worth using for a quick lookup.

**Solution:** put a simple search box plus an [[action-buttons|action button]] on every page, in a consistent location (above the fold — top left, middle, or right), rather than relying on a separate, more complex search page. Consistency of placement matters because customers may initiate a search from any page on the site.

For large sites with many content categories, a **search selector** (a dropdown narrowing the search to a subsection) can be added once a plain free-text search starts returning too many undifferentiated results. Two design considerations matter here: the selector needs a sensible default category (so a user who doesn't change it still gets relevant results), and a selector is not worth adding on a small site that can't produce enough results per category to justify it.

Search results returned by the module are presented on an [[organized-search-results|organized results page]]; if a query needs more precision than a simple box allows, the site can offer a more detailed [[straightforward-search-forms|search form]] as a secondary option.

This pattern is the second worked example (alongside [[action-buttons]]) used to walk through the full pattern format in [[web-design-patterns]], and was later documented in full as the opening pattern of its own group (J1).
