---
type: source
title: "Speeding Up Your Site (Pattern Group L, The Design of Sites)"
tags: [design-patterns, performance, implementation]
related: [interface-design-principles, homepage-portal, web-design-patterns]
created: 2026-06-24
updated: 2026-06-24
authors: [van Duyne, Landay, Hong]
year: 2006
url: ""
venue: "The Design of Sites (2nd ed.), Pattern Group L, pp. 759-792"
---

# Speeding Up Your Site

Pattern Group L of *The Design of Sites* — six patterns (L1-L6) for making a site download, and feel, fast: LOW NUMBER OF FILES, FAST-LOADING IMAGES, SEPARATE TABLES, HTML POWER, REUSABLE IMAGES, and FAST-LOADING CONTENT.

## Key points

- L1-L5 are almost entirely implementation technique: removing unnecessary files, image file-format trade-offs (GIF vs. JPEG vs. PNG, cropping/shrinking/compression ratios, progressive-scan vs. interlaced loading), splitting large HTML tables so the top of a page renders before the rest, using native HTML markup instead of images, and relying on browser image caching. Per `purpose.md`'s "specific code implementation" exclusion, none of this was extracted into wiki pages — it sits below the UX/design-principle level this wiki tracks, regardless of how many sources might eventually repeat it.
- L6 (FAST-LOADING CONTENT) is the one pattern in this group with real UX substance: the distinction between actual speed and *perceived* speed, and a taxonomy of progress indicators — a static text message, an animated "marching ants" indicator, a thermometer, and progressively displaying content as it arrives — each with a real trade-off (a thermometer is the most reassuring when accurate, but worse than no indicator at all when it isn't). This is a direct, concrete elaboration of the "offer informative feedback" principle already documented in [[interface-design-principles]], so it was folded into that page's existing feedback principle rather than split into a new one.
- [[homepage-portal]] already noted that "fast downloads matter as much as content" — added a forward link there to [[interface-design-principles]]'s feedback principle, for the case where a homepage genuinely can't be made fast enough and the next-best thing is managing the wait itself.

## Notes for the wiki

No new concept or entity pages. All of this chapter's screenshot examples (Yahoo!, Geocaching.com, Craigslist, Napster, Lowestfare.com, PETA, BabyCenter, the Lincoln Highway site, SideStep, A9.com, Yahoo! Mail, Expedia, Zazzle, Kayak.com, Google Maps) are single-source and illustrate implementation techniques rather than UX substance — and for several (image formats, HTML attributes, AJAX), the subject itself is out of scope regardless of source count, so they wouldn't earn a page even with repetition elsewhere. Yahoo!'s minimalist-homepage example here simply reconfirms what [[yahoo]] already says about its fast, sparse-graphics interface — no new substance was added to that page.
