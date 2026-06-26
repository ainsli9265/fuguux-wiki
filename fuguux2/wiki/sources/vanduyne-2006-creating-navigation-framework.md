---
type: source
title: "Creating a Navigation Framework (Pattern Group B, The Design of Sites)"
tags: [design-patterns, navigation, information-architecture, accessibility]
related: [multiple-ways-to-navigate, browsable-content, content-organization-schemes, category-pages, accessibility, web-design-patterns, card-sorting]
created: 2026-06-24
updated: 2026-06-24
authors: [van Duyne, Landay, Hong]
year: 2006
url: ""
venue: "The Design of Sites (2nd ed.), Pattern Group B, pp. 215-266"
---

# Creating a Navigation Framework

Pattern Group B of *The Design of Sites* — nine patterns (B1-B9) for letting customers move through a site in whatever way suits how they arrived and what they're after, since customers rarely all enter at the homepage or want the same thing.

## Key points

- [[multiple-ways-to-navigate]] (B1) — the intention/impulse motivator framework and the five navigation styles (search, browse, next-step, relate, promote) that serve them, plus where each belongs on the page.
- [[browsable-content]] (B2) — organizing content for browsing rather than searching, the information-scent concept (coined at Xerox PARC), and finding-your-way-back cues.
- [[content-organization-schemes]] (B3-B7, combined into one page) — hierarchical, task-based, alphabetical, chronological, and popularity-based organization, presented in the book as a menu of interchangeable/combinable answers to one question rather than five separate problems.
- [[category-pages]] (B8) — keeping a site's distinct sections recognizably part of one whole, via consistent layout and a clear "you've arrived" signal.
- SITE ACCESSIBILITY (B9) — folded into the existing [[accessibility]] page rather than given its own (see Notes below).

## Notes for the wiki

This chapter resolves two long-flagged documentation gaps: MULTIPLE WAYS TO NAVIGATE (B1) and BROWSABLE CONTENT (B2) had been referenced, unlinked, from several earlier-ingested chapters and concept pages without ever being explained — both now have full pages.

B9 (SITE ACCESSIBILITY) was **not** given its own page, unlike the other eight patterns in this chapter. By the time this chapter was ingested, [[accessibility]] already covered POUR, WCAG, WAI-ARIA, color-vision deficiency, motor control, and screen-reader/assistive-technology support in depth from four prior Wikipedia/USWDS ingestions — most of B9's content (Section 508, alt text, color contrast, keyboard navigation) simply re-confirmed what was already there. The genuinely new material was folded into [[accessibility]] instead: the curb-cut-effect framing for the business case, a concrete green-unvisited/red-visited link-color example, a 2005 study (Mankoff, Fait, and Tran) on the relative effectiveness of different accessibility-testing methods, and a brief note connecting style-sheet-based content/presentation separation to accessibility specifically.

Card sorting's role in [[content-organization-schemes|hierarchical organization]] (B3) is paired here with two testing techniques not previously in this wiki — category identification and category description — both folded into [[card-sorting]] rather than left only on the organization-schemes page, since they're squarely card-sorting-adjacent testing methods. Both are described more fully in a pattern this chapter references but doesn't itself contain, FAMILIAR LANGUAGE (K11), not yet ingested.

**Excluded:** the chapter's specific accessibility-tool recommendations (WebXACT/Bobby, the Colorblind Web Page Filter, Vischeck, Fangs) as named, mostly-defunct circa-2001-2006 software products — implementation tooling, not design principle, consistent with how other defunct named tools (the Web Metrics Tool Suite, UsableNet Liftmachine) were excluded from the usability-engineering ingestion; the W3C's older "ten quick tips" checklist, since it's a simplified precursor to the POUR/WCAG framework already documented in depth via [[wcag]]; HTML/CSS specifics (`<alt>`, `<title>`, `<longdesc>` attribute syntax) per `purpose.md`'s implementation-code exclusion; and the mobile-device-specific accessibility tips (MOBILE SCREEN SIZING, MOBILE INPUT CONTROLS), since Pattern Group M (the Mobile Web) hasn't been ingested yet and these patterns aren't explained anywhere else in this wiki to link against.

No new entities. Wal-Mart, Sun.com, Salesforce.com, FindLaw, Billboard, Flickr, the "Lycos 50 Daily Report," Martha Stewart's site, REI.com, and the Weather Channel are single-source incidental examples; Yahoo! and Amazon each get another incidental confirming example here (hierarchical directory, intention/impulse navigation respectively) but no new substance beyond what their existing entity pages already say.
