---
type: concept
title: Above the Fold
tags: [layout, design-pattern, navigation, screen-resolution]
related: [grid-layout, clear-first-reads, expanding-and-fixed-screen-width, web-design-patterns, homepage-portal, organized-search-results, vanduyne-2006-designing-effective-page-layouts]
sources: [vanDuyne_I_3PP_631-660.pdf]
created: 2026-06-24
updated: 2026-06-24
---

# Above the Fold

**Problem:** visitors often miss content and navigation elements that require scrolling — many never realize there's more below, so anything that matters has to be visible without scrolling.

**Background:** the term comes from newspaper layout, where editors put the day's most important story above the literal fold of a physical paper. On the Web, "the fold" isn't a fixed line — it's wherever a given visitor's screen and browser window happen to cut the page off — so unlike print, a designer can never be certain exactly where it falls for any one visitor.

**Solution:** decide on a minimum screen resolution to support (survey customers' actual resolutions rather than guessing), then deliberately place the most important material within that minimum visible area: the page title, a [[clear-first-reads|clear first read]], navigation bars, and key content modules. The same placement-expectation research used in [[grid-layout]] (the Wichita State University study) found people expect the shopping cart, account management, and help links at the top right, a sign-in link near the top left, and a clickable logo back to the homepage in the very top-left corner. Test candidate layouts across a range of screen sizes rather than just the designer's own monitor — see [[expanding-and-fixed-screen-width]] for the layout strategies that determine what those sizes actually look like.

**Forces:** above-the-fold space is a page's most contested real estate — marketing wants ads there, engineers want to show off the feature they just built, designers want to show off visual work — and reconciling those pulls with what customers actually need to see first is the core tension this pattern manages. It also competes directly with [[clear-first-reads]]: a first read needs to be large enough to dominate the page, but that size eats into the limited space available above the fold, so the two have to be balanced against each other rather than both maximized independently. A search-results page is the one place this pattern's logic runs in reverse: [[organized-search-results|putting search refinement controls below the fold]] only looks like a violation — by the time a customer reaches the bottom of a results page they've already scanned everything above it, so those controls matter most exactly where they sit.
