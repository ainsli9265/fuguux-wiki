---
type: concept
title: Expanding and Fixed Screen Width
tags: [layout, design-pattern, responsive-layout, readability]
related: [grid-layout, above-the-fold, web-design-patterns, vanduyne-2006-designing-effective-page-layouts, responsive-web-design]
sources: [vanDuyne_I_3PP_631-660.pdf]
created: 2026-06-24
updated: 2026-06-24
---

# Expanding and Fixed Screen Width

Two contrasting strategies for handling the fact that a Web designer never knows exactly how wide a visitor's browser window will be — covered together here because the book always presents them as a direct contrast with each other.

**Expanding screen width**: let the page's layout stretch to fill whatever width the browser window happens to be, typically by keeping navigation and side content at a fixed width while letting the central content column grow or shrink to absorb the difference. The payoff is not wasting space that a larger-than-expected window would otherwise leave empty — useful for pages with lots of navigation elements and varied content, such as a portal homepage. The tradeoff is reduced control over the page's exact appearance, and there's still a practical minimum width below which the layout breaks down, so designers still need to survey customers' actual screen resolutions and decide on a floor to support (see [[above-the-fold]]).

**Fixed screen width**: keep the page at exactly the same width regardless of browser size, usually by giving the column holding the main content (centered or left-aligned — a stylistic choice with no real functional difference) a fixed width. This is the better choice for articles, essays, and other long passages of text, because text allowed to stretch across an overly wide browser window becomes hard to skim and easy to lose your place in — readability, not screen real estate, is what drives the choice here.

**Forces:** the choice between the two comes down to content type more than aesthetics — pages dominated by navigation and varied content modules lean toward expanding width; pages dominated by a single long passage of reading lean toward fixed width. Both are normally combined with [[grid-layout]] and built into a reusable page template; the actual mechanics (HTML table widths vs. style-sheet-based layout) are an implementation detail outside this wiki's scope.

The fixed-vs.-expanding binary is the older framing of a question that [[responsive-web-design]] now answers more generally: proportion-based fluid grids that reflow at defined breakpoints, so the same page serves both a narrow smartphone and a wide desktop without choosing one or the other.
