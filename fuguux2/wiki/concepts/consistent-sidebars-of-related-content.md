---
type: concept
title: Consistent Sidebars of Related Content
tags: [layout, design-pattern, navigation, content-discovery]
related: [grid-layout, web-design-patterns, homepage-portal, vanduyne-2006-designing-effective-page-layouts, multiple-ways-to-navigate]
sources: [vanDuyne_I_3PP_631-660.pdf]
created: 2026-06-24
updated: 2026-06-24
---

# Consistent Sidebars of Related Content

**Problem:** customers reading a content page (a news article, a product page) often want related material — similar products, related articles, further discussion — but presenting those links well is awkward: putting them at the bottom of the page risks visitors never scrolling far enough to see them, while overdoing it can distract from or crowd out the main content.

**Solution:** place related-content links in a sidebar near the top of the page, on the side, where they stay visually distinct from the main content without requiring a scroll. Because navigation bars conventionally run along the top and left and main content sits in the center, sidebars conventionally end up on the right. Make the sidebar's location consistent across the site by building it into the page's [[grid-layout]] and reusing that as a page template, and cap each sidebar's length (manually, or automatically if its content is pulled from a database) so a long sidebar doesn't make the page layout look lopsided next to shorter main content.

**Forces:** sidebars are one of several competing ways to surface related content — others include links embedded directly in body text, or related items placed at the bottom of the page — and the right choice depends on how much related content there is and how important it is that visitors notice it immediately versus discover it incidentally. Sidebars are also a common home for personalized or promotional content, which raises the same value-versus-infrastructure tradeoff already covered in [[homepage-portal]]'s personalization discussion.

In the vocabulary of [[multiple-ways-to-navigate]], a sidebar of related content is the canonical "relate" navigation style — content a visitor wasn't looking for but might act on anyway, which is exactly why it gets less valuable screen space than the navigation tools someone actually came for.
