---
type: source
title: "Web Accessibility (Wikipedia)"
tags: [accessibility, wcag, assistive-technology, standards, legislation]
related: [accessibility, wcag, wikipedia-2026-web-content-accessibility-guidelines]
created: 2026-06-24
updated: 2026-06-24
authors: [Wikipedia contributors]
year: 2026
url: "https://en.wikipedia.org/wiki/Web_accessibility"
venue: "Wikipedia"
---

# Web Accessibility (Wikipedia)

A general-encyclopedia overview of Web accessibility: assistive technologies, the WCAG/ATAG/UAAG guideline family, WAI-ARIA, country-by-country legislation, and auditing methods. Wikipedia articles are continuously edited, so `year` above reflects the access date (2026-06-24), not a fixed publication year — re-check the live page if a claim here needs revalidating against the current text.

## Key points

- **POUR principles**: WCAG organizes its guidelines under four top-level principles — content must be **P**erceivable, **O**perable, **U**nderstandable, and **R**obust.
- **WCAG 2.0's structure**: 4 principles → 12 untestable guidelines (goals) → 61 testable success criteria, each rated conformance level A, AA, or AAA. *(Corrected from an initial "65" — see Notes below.)*
- **History**: WCAG 1.0 (1999, W3C Web Accessibility Initiative) → WCAG 2.0 (December 2008) → adopted as ISO/IEC 40500:2012 → WCAG 2.1 (2018).
- **Assistive technologies named**: screen readers with synthesized speech, refreshable braille displays, screen magnification software, speech-recognition software, keyboard overlays, and closed captioning/sign-language access for video.
- **Legal landscape is global, not just U.S.**: beyond Section 508/ADA, the article documents accessibility laws or standards in the EU (European Accessibility Act, applicable since June 2025), UK (Equality Act 2010, BS 8878), Canada, Australia, Japan, Israel, and many other countries — accessibility compliance is now a near-universal legal requirement, not a U.S.-specific one.
- **A 2018 WebAIM survey** found about 93% of respondents had received no formal training in Web accessibility — cited as context for why automated scanners alone (which catch only a fraction of real issues) remain so common despite their limits.

## Notes for the wiki

A local snapshot is saved at `raw/safe/wikipedia-web-accessibility.html` alongside the live URL. Wikipedia text is licensed **CC BY-SA 4.0** (Creative Commons Attribution-ShareAlike), not public domain — an explicit open license under this wiki's `## Source Triage` rule in `schema.md`, so it belongs in `raw/safe/`, but unlike the U.S.-government sources already in this wiki, reusing its wording verbatim would carry an attribution/share-alike obligation. Everything folded into [[accessibility]] below is paraphrased rather than quoted for this reason.

Folded the POUR framework, the WCAG 2.0 quantified structure, conformance levels (A/AA/AAA), a brief standards history, and concrete assistive-technology examples into [[accessibility]]. Did not fold in the country-by-country legislation list or the U.S. litigation statistics — useful context but more legal reference than UX design principle, and `purpose.md` scopes this wiki to design/accessibility *guidelines* rather than litigation tracking; mentioned only in summary (laws exist well beyond the U.S.) rather than enumerated.

**Correction (2026-06-24):** the "65 testable success criteria" figure above was wrong — an artifact of the original `WebFetch` AI-summarized pass over this article rather than a misstatement by Wikipedia itself. Ingesting [[wikipedia-2026-web-content-accessibility-guidelines]] and reading its raw HTML directly confirmed the correct figure is 61. That source's added depth on WCAG's own structure, version history (2.1, 2.2, the 3.0 draft), and jurisdiction-specific legal mandates also justified moving all of this article's WCAG-structure content out of [[accessibility]] and into a new dedicated page, [[wcag]], rather than continuing to grow a single paragraph there.
