---
type: concept
title: Page Template
tags: [layout, design-pattern, information-architecture, consistency]
related: [grid-layout, above-the-fold, clear-first-reads, expanding-and-fixed-screen-width, consistent-sidebars-of-related-content, multiple-ways-to-navigate, category-pages, clean-product-details, responsive-web-design, web-site-development-process, vanduyne-2006-designing-effective-page-layouts, vanduyne-2006-developing-customer-centered-sites]
sources: [vanDuyne_05_3PP_097-116.pdf, vanDuyne_I_3PP_631-660.pdf]
created: 2026-06-26
---

# Page Template

A page template is a reusable structural layout applied consistently to all pages of the same type on a site. Where a [[grid-layout|grid]] defines the underlying column-and-row system, a page template fills that grid with fixed-position regions — header, navigation, main content area, sidebar, footer — whose positions stay stable across every page in the same class. A customer who has seen one product page on a site has implicitly learned the template; the second product page requires no reorientation.

## Why templates matter

Consistency is one of the seven principles in [[interface-design-principles]]: when the same element appears in the same place every time, customers build expectations that let them navigate faster on repeat visits. Page templates operationalize consistency at the structural level — they make it impossible (or at least inconvenient) for individual pages to drift away from the site's established layout.

Templates also separate concerns: the template determines where things appear; content determines what appears. A well-designed template can absorb a wide range of content without breaking — short or long articles, dense or sparse product pages, narrow or wide images — because the structural regions are built to flex while maintaining their relative positions.

## Template classes

A site typically has a small set of distinct templates corresponding to its page types, not a single universal template for all pages:

- **Homepage** — highest-stakes first impression; often the most bespoke layout, though still built on the site grid
- **Category / section pages** — consistent navigation entry points into a product or content area; see [[category-pages]]
- **Detail pages** — the canonical leaf page type: an article, a product, a profile; often the most standardized template on the site since the content structure is predictable (see [[clean-product-details]] for the e-commerce variant)
- **Search results** — a distinct template optimized for scanning a list rather than reading a single item
- **Checkout / form pages** — often stripped-down templates that suppress non-essential navigation to focus the user on a single task (see [[quick-flow-checkout]])

## Templates in the development process

Per [[web-site-development-process]], page templates emerge during the Refinement phase — the site is broken into template classes (homepage, second-level, leaf page) rather than designing every page individually. In the Production phase, each template class is refined into an interactive prototype and eventually into a reusable HTML skeleton that forms the technical basis for implementation. Defining templates early reduces both design and development effort: decisions made once in the template propagate to every page in that class.

## Relationship to layout patterns

The six layout patterns documented in Pattern Group I of *The Design of Sites* ([[grid-layout]], [[above-the-fold]], [[clear-first-reads]], [[expanding-and-fixed-screen-width]], [[consistent-sidebars-of-related-content]]) are each described in the source as contributions to the page template — each governs one dimension of the template's structure. The dedicated PAGE TEMPLATE pattern (D1) is in Pattern Group D, not yet ingested into this wiki; when Group D is ingested, expand this page with that material.

[[responsive-web-design]] adds a temporal dimension to the template: the same structural template reflows at defined breakpoints for different viewport sizes, so a single template definition covers the full range of screen widths rather than requiring separate mobile and desktop versions.
