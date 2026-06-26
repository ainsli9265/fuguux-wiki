---
type: concept
title: Web Design Patterns
tags: [design-patterns, pattern-language, web-design]
related: [customer-centered-design, action-buttons, search-action-module, process-funnel, homepage-portal, up-front-value-proposition, ebay, amazon, google, yahoo, ibm, vanduyne-2006-web-design-patterns, grid-layout, above-the-fold, clear-first-reads, expanding-and-fixed-screen-width, consistent-sidebars-of-related-content, vanduyne-2006-designing-effective-page-layouts, straightforward-search-forms, organized-search-results, vanduyne-2006-making-site-search-fast-and-relevant, multiple-ways-to-navigate, browsable-content, content-organization-schemes, category-pages, vanduyne-2006-creating-navigation-framework]
sources: [vanDuyne_02_3PP_019-038.pdf]
created: 2026-06-23
updated: 2026-06-24
---

# Web Design Patterns

A design pattern captures a recurring UX problem and its solution in a compact, reusable form: the problem itself, the rationale for a solution, how to apply it, and the trade-offs involved. The idea originates with architect Christopher Alexander, whose 1977 book *A Pattern Language* proposed a shared vocabulary non-experts could use to participate in designing buildings and towns. Web design patterns adapt this to digital interfaces, with a deliberate focus on the customer's experience rather than on whatever conventions a team happens to fall into (see [[customer-centered-design]]).

Alexander argued that isolated patterns have limited value — the power comes from a *language* of interconnected patterns that complete and constrain one another. Web design patterns work the same way: a given pattern typically references higher-level patterns it helps complete and lower-level patterns that complete it. For example, [[action-buttons]] helps complete a [[process-funnel]] (by giving each step a clear call to action) and is itself completed by patterns for fast-loading images.

## Pattern format

Each pattern is documented in six parts, always in the same order:

1. **Name** — a short phrase usable in a sentence, conventionally written in small capitals.
2. **Background** — context: which other patterns lead into this one, and the pattern's scope.
3. **Problem** — a concise statement of the specific design problem.
4. **Forces** — the competing concerns (user behavior, task requirements, technology constraints, social context) that make the problem non-trivial and that any solution must balance. For instance, bigger buttons are easier to click but consume more space, and image-based links load slower than text links.
5. **Solution** — a succinct statement of how to resolve the problem, generally accompanied by a sketch.
6. **Other patterns to consider** — related patterns that can complete or extend the solution.

## Pattern groups

Patterns are organized into thirteen lettered groups (A–M), roughly ordered by where they fit in the design process — from high-level site genres and navigation frameworks (A, B) through content, trust, and e-commerce concerns (D–H), to page layout, search, navigation mechanics, performance, and mobile concerns (I–M):

Site Genres (A) · Creating a Navigation Framework (B) · Creating a Powerful Homepage (C) · Writing and Managing Content (D) · Building Trust and Credibility (E) · Basic E-Commerce (F) · Advanced E-Commerce (G) · Helping Customers Complete Tasks (H) · Designing Effective Page Layouts (I) · Making Site Search Fast and Relevant (J) · Making Navigation Easy (K) · Speeding Up Your Site (L) · The Mobile Web (M)

## Patterns documented in full on this wiki

Most of the ~100+ named patterns in the book are only named in passing wherever they're cited (per the page-creation threshold); a pattern only gets its own page once a source explains it in full. So far: [[action-buttons]] (K4) and [[search-action-module]] (J1, originally a worked example here, later expanded to full pattern depth by its own group) from the worked examples in this chapter; [[process-funnel]] (H1); [[homepage-portal]] (C1) and [[up-front-value-proposition]] (C2) from Pattern Group C; [[multiple-ways-to-navigate]] (B1), [[browsable-content]] (B2), [[content-organization-schemes]] (B3–B7, combined — the book presents them as a menu of interchangeable/combinable schemes for one decision, not five separate problems), and [[category-pages]] (B8) from Pattern Group B (B9, SITE ACCESSIBILITY, was folded into the existing [[accessibility]] page instead, given how much it already overlapped); [[grid-layout]] (I1), [[above-the-fold]] (I2), [[clear-first-reads]] (I3), [[expanding-and-fixed-screen-width]] (I4 + I5), and [[consistent-sidebars-of-related-content]] (I6) from Pattern Group I; and [[straightforward-search-forms]] (J2) and [[organized-search-results]] (J3) from Pattern Group J. Keep this list current as more pattern-group chapters are ingested.

## Durability

Comparing screenshots of major sites ([[ebay]], [[amazon]], [[google]], [[yahoo]], CNN, MSN) from 2001 to 2006, the underlying structural patterns (navigation bars, search modules, checkout flows) stay essentially constant even as visual styling becomes more polished and information-dense. The argument is that surface visual trends change quickly, but the underlying interaction patterns are comparatively stable — what the authors call the "common Web look and feel" (e.g., two- or three-column grid layout, navigation bar/tab row along the top, search box at top right or middle-left, a clickable logo, privacy/about-us links in the footer).
