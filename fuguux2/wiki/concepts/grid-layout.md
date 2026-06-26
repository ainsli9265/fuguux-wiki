---
type: concept
title: Grid Layout
tags: [layout, design-pattern, page-template, visual-design]
related: [above-the-fold, clear-first-reads, expanding-and-fixed-screen-width, consistent-sidebars-of-related-content, web-design-patterns, homepage-portal, vanduyne-2006-designing-effective-page-layouts, gestalt-psychology, browsable-content, category-pages, multiple-ways-to-navigate]
sources: [vanDuyne_I_3PP_631-660.pdf]
created: 2026-06-24
updated: 2026-06-24
---

# Grid Layout

**Problem:** the many competing elements of a Web page (titles, logos, navigation, search, content modules) are hard to organize cohesively without creating clutter that overwhelms the visitor.

**Solution:** borrow grid layout from graphic design — divide the page into rows and columns and make every element fit within that grid, with constant elements (logo, navigation) always appearing in the same place. Three payoffs: customers can predict where things live; clutter drops and strong visual cues make content easier to find and faster to read; and once a grid is built, the design team can reuse it instead of re-deciding layout for every new page.

To build one: identify the elements common across most pages (logo, navigation bars, a search box, a privacy-policy link, content modules) and use them to anchor the grid; sketch several candidate grids and group related elements visually (proximity, shared size/color/font, separating lines — see [[gestalt-psychology]] for the perceptual principles this relies on) while keeping unrelated elements apart; lean on known placement expectations (an instance of [[gestalt-psychology|the Gestalt law of past experience]]: people interpret a layout according to what they've already seen, not in a vacuum) — research at Wichita State University found people expect shopping-cart, account-management, and help links at the top right, a sign-in link near the top left, and a clickable logo back to the homepage in the very top-left corner; and test sketches with real customers by **"greeking"** the text (replacing it with nonsense placeholder text — classically a corrupted Latin passage starting "Lorem ipsum dolor sit amet") to see whether people can still identify the page's basic elements from position and layout alone.

**Forces:** a grid has to accommodate variable-length, often dynamically-retrieved content (news items, stock quotes, and similar modules vary in length), which makes precise control over the final layout harder than the grid metaphor alone suggests.

Grid layout is the structural backbone of a Web site's page template (the higher-level pattern it serves is not yet documented in this wiki); the three elements most central to it are navigation bars, a search box, and content modules. It's typically combined with [[above-the-fold]] (deciding what must be visible without scrolling), [[clear-first-reads]] (giving the page a single dominant focal point), [[expanding-and-fixed-screen-width]] (deciding how the grid responds to different browser widths), and [[consistent-sidebars-of-related-content]] (reserving part of the grid for related-content links). The same grid is also what makes [[browsable-content|browsable content]] scannable rather than overwhelming, what keeps [[category-pages|category pages]] feeling like one consistent site, and what gives every tool in [[multiple-ways-to-navigate]] a stable, predictable place to live. Older sites often built grids out of HTML tables; current practice favors style sheets instead — an implementation detail outside this wiki's scope, beyond noting that the underlying design discipline (rows, columns, consistent placement) is unchanged either way.
