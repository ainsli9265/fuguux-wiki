---
type: source
title: "Advanced E-Commerce (Pattern Group G, The Design of Sites)"
tags: [design-patterns, e-commerce, recommendations, checkout]
related: [featured-products, cross-selling-and-up-selling, personalized-recommendations, recommendation-community, multiple-destinations, gift-giving, order-tracking-and-history, walmart, lands-end, amazon, ebay, yahoo, trust-and-credibility, process-funnel, web-design-patterns, vanduyne-2006-basic-e-commerce, barnes-and-noble]
created: 2026-06-25
updated: 2026-06-25
authors: [van Duyne, Landay, Hong]
year: 2006
url: ""
venue: "The Design of Sites (2nd ed.), Pattern Group G, pp. 491-544"
---

# Advanced E-Commerce

Pattern Group G of *The Design of Sites* — seven patterns (G1-G7) building on the basic e-commerce checkout flow ([[vanduyne-2006-basic-e-commerce|Pattern Group F]]) with optional features for promoting products, personalizing the shopping experience, and supporting customers after the sale. Documents all seven in full six-part format, per [[web-design-patterns]].

## Key points

- [[featured-products]] (G1) — curated, editorialized product lists (Best-Sellers, Editors' Picks, On Sale) for browsing-minded customers who don't arrive with a specific product in mind.
- [[cross-selling-and-up-selling]] (G2) — recommending accessories or upgrades related to a customer's current choice, kept visually secondary to the main product and repeated at checkout in case it was missed.
- [[personalized-recommendations]] (G3) — recommendations built on deliberate signals (ratings, a short preference interview) rather than noisy inferred browsing data, with explicit attention to privacy disclosure.
- [[recommendation-community]] (G4) — customer-written reviews: a two-step write/preview funnel, use policies and filtering, and meta-ratings (Amazon's "helpful?" votes, eBay's buyer/seller feedback score) to surface trustworthy reviews.
- [[multiple-destinations]] (G5) — shipping different items in one order to different addresses, with a destination-grouped order summary.
- [[gift-giving]] (G6) — price-hiding packing slips, per-item gift notes and wrap pricing, and a gift-finder recommendation flow.
- [[order-tracking-and-history]] (G7) — self-service order history, modification, and shipment tracking, replacing phone-based customer service for routine status questions.

## Notes for the wiki

Four of the seven patterns (G1-G4) are explicitly described as alternative, *non-exclusive* ways to provide product recommendations — a site can use any or all simultaneously — so each got its own page rather than being merged, unlike e.g. [[content-organization-schemes]] (B3-B7), which the book presents as five mutually-exclusive answers to one decision.

**Entities:** [[walmart]] and [[lands-end|Lands' End]] both cross the 2+-source entity threshold here — each had previously appeared only as a bare, unexplained name (Walmart in Pattern Group B's list of examples; Lands' End as an uncaptioned screenshot in Pattern Group I) and this chapter gives each real depth (Walmart: [[multiple-destinations]] and [[gift-giving]]; Lands' End: the preference-interview technique in [[personalized-recommendations]]). [[amazon]], [[ebay]], and [[yahoo|Yahoo!]] all gained substantial new material, folded into their existing pages rather than duplicated.

Stayed below the entity threshold despite a second mention: **Martha Stewart's site** and **Barnes & Noble** — both now appear in two sources, but neither mention (here or previously) goes beyond a single bare or lightly-captioned screenshot, the same standard that's kept CNN and Epicurious below threshold in earlier sessions. **Netflix** appears twice in this chapter alone (cross-sell floating window in G2, a star-rating system in G3) but that's still one source no matter how many times it's used within it, so it stays inline regardless of depth. 1-800-Flowers, Brooks Brothers, Ann Taylor, The Knot, CD Universe, RedEnvelope, TiVo, Nordstrom, and Shutterfly are single-source incidental examples.

**Media:** 40 screenshots/figures extracted from the PDF (via `pypdf`, since no PDF-render tool like `pdftoppm`/`pdfimages` is available in this environment) and saved to `raw/media/vanduyne-2006-advanced-e-commerce/`, named by figure number (e.g. `G1.1.png`, `G3.4a.png`). A few pages yielded more raster chunks than the text's figure count implied (G6.2/G6.2-Continued, G7.2) — inspected each one directly and confirmed they're genuinely separate screenshots from the same multi-step flow, not duplicate tiles, and named them with sequential letter suffixes (`G6.2a`-`G6.2d`, `G7.2a`-`G7.2b`) accordingly. The chapter's purely schematic "Solution" diagrams (G1.5, G2.7, G3.5, G4.6, G5.5, G6.4, G7.4) didn't extract as raster images — likely vector graphics in the original PDF — so no files exist for those.

**Excluded** (per `schema.md`'s ingestion-report requirement): Table G1.1/G1.2's specific commonly-asked-question/pattern-cross-reference grids and Table G7.1/G7.2's order-status/modification-routing grids — summarized in prose in the relevant concept pages rather than reproduced as tables, consistent with this wiki's general preference for prose over reproduced book tables; G4's footnoted Pew Internet & American Life Project citation detail beyond the one statistic actually used; AJAX as an implementation detail (G3's ratings-without-reload mention) per the code-implementation exclusion. Cross-references to patterns in not-yet-ingested groups (A, D, E, H, K) were kept as plain text rather than forced links — Group F has since been ingested as [[vanduyne-2006-basic-e-commerce]] (pages: [[quick-flow-checkout]], [[shopping-cart]], [[clean-product-details]], [[easy-returns]]). This chapter leaned especially heavily on Group F and Group H (PROCESS FUNNEL — already covered by [[process-funnel]] from Ch. 2 — plus SIGN-IN/NEW ACCOUNT, GUEST ACCOUNT, FLOATING WINDOW, PREDICTIVE INPUT, DRILL-DOWN OPTIONS), reinforcing both as priorities for future ingestion.
