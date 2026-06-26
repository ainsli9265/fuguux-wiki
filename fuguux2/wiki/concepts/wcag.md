---
type: concept
title: Web Content Accessibility Guidelines (WCAG)
tags: [accessibility, wcag, standards, legislation, conformance]
related: [accessibility, uswds-2025-design-principles, wikipedia-2026-web-accessibility, wikipedia-2026-web-content-accessibility-guidelines, wai]
sources: ["https://en.wikipedia.org/wiki/Web_accessibility", "https://en.wikipedia.org/wiki/Web_Content_Accessibility_Guidelines", "Design principles _ U.S. Web Design System (USWDS).pdf", "https://designsystem.digital.gov/design-principles/"]
created: 2026-06-24
updated: 2026-06-24
---

# Web Content Accessibility Guidelines (WCAG)

The W3C's formal, testable standard for [[accessibility]] — the standard [[accessibility]] itself measures conformance against, split out into its own page once the standard's internal structure and version history grew substantial enough to outgrow a single paragraph there. WCAG is produced by [[wai]], the W3C body responsible for Web accessibility standards generally; WCAG covers content specifically, while WAI's other specification families cover authoring tools, browsers, and dynamic-content markup — see [[wai]] for those.

## Structure

WCAG is organized around four top-level **POUR** principles: content must be **P**erceivable, **O**perable, **U**nderstandable, and **R**obust. Each principle breaks down into guidelines (untestable goals to aim for — 12 of them in WCAG 2.0), and each guideline breaks down into testable **success criteria** — 61 in WCAG 2.0. Every success criterion carries a conformance level: **A** (must satisfy), **AA**/Double-A (should satisfy), or **AAA**/Triple-A (may satisfy, the hardest tier). A separate, periodically-updated **techniques** document lists concrete ways to meet each criterion, kept distinct from the principles/guidelines/criteria themselves so the stable normative standard doesn't have to change every time a new technique is documented. Examples of how specific a success criterion gets: 1.4.3 Contrast (Minimum) and 2.4.7 Focus Visible are both AA-level; 2.5.7 Dragging Movements (requiring drag interactions to have a single-pointer-tap alternative) was added at AA in version 2.2.

## Version history

- **WCAG 1.0** (May 5, 1999) — built on the earlier Unified Web Site Accessibility Guidelines (1998).
- **WCAG 2.0** (W3C Recommendation, December 2008; adopted as ISO/IEC 40500:2012) — the version that introduced the POUR/guidelines/success-criteria/conformance-level structure described above; 61 success criteria total.
- **WCAG 2.1** (2018) — backward-compatible with 2.0, adding 17 more success criteria (78 total) aimed mainly at mobile, low-vision, and cognitive/learning-disability accessibility.
- **WCAG 2.2** (W3C Recommendation, October 5, 2023) — backward-compatible with 2.1, adding 9 more success criteria (87 total relative to 2.0) and deprecating one prior criterion (4.1.1 Parsing, no longer needed given how modern browsers handle malformed markup).
- **WCAG 3.0** — in draft since early 2021 (last updated September 2025 as of this wiki's ingestion), not yet an official Recommendation; expected to depart further from the 1/2.x numbering and scoring model rather than simply extending it.

## Legal adoption

WCAG conformance is a binding legal requirement in many jurisdictions, generally pegged to a specific version and level rather than "WCAG" in the abstract:

- **United States**: a U.S. Department of Justice final rule (April 24, 2024) sets WCAG 2.1 Level AA as the technical standard for state and local government Web content under Title II of the ADA — distinct from, and more specific than, [[accessibility|Section 508]], which covers federal sites.
- **European Union**: Directive 2016/2102 requires WCAG 2.1 AA for public-sector sites and apps; the European Accessibility Act extends comparable obligations into much of the private sector as of June 28, 2025.
- **United Kingdom**: public-sector bodies have been required to meet WCAG 2.1 AA since September 2018.
- **Canada, Australia**, and others reference WCAG 2.0 or 2.1 AA in their own accessibility regulations, in some cases (Canada's 2012 *Jodhan* Supreme Court decision) reinforced directly by litigation rather than statute alone.

This pattern — a single technical standard, adopted piecemeal and at different version/level combinations by different regulators — is why [[accessibility]] frames legal compliance as "near-universal but not uniform," rather than naming one law as authoritative.

## Notes for the wiki

Both Wikipedia sources used here are licensed **CC BY-SA 4.0**, not public domain — content below is paraphrased rather than quoted, consistent with the precedent set when [[wikipedia-2026-web-accessibility]] was first ingested. This page also corrects a figure introduced during that earlier ingestion: [[accessibility]] briefly stated WCAG 2.0 has 65 success criteria, sourced from an AI-summarized `WebFetch` pass over the first Wikipedia article. Reading this second article's raw text directly confirms the correct figure is **61** (verified against the literal phrase "testable success criteria (61 in all)" in the saved HTML snapshot) — the 65 figure was a small-model summarization error, not a real contradiction between sources. Corrected in both places.
