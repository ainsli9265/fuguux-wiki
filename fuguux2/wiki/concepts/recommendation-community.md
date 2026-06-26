---
type: concept
title: Recommendation Community
tags: [e-commerce, recommendations, design-pattern, user-generated-content, trust]
related: [featured-products, cross-selling-and-up-selling, personalized-recommendations, process-funnel, action-buttons, trust-and-credibility, amazon, ebay, yahoo, vanduyne-2006-advanced-e-commerce]
sources: [vanDuyne_G_3PP_491-544.pdf]
created: 2026-06-25
updated: 2026-06-25
---

# Recommendation Community

**Problem:** customer reviews are valuable enough that people will leave a site to find them elsewhere if they're missing — a 2000 Pew Internet & American Life Project survey found 73% of people research a product or service before buying it — but running a review system well means managing genuine abuse risk (obscenity, libel, copyrighted material, fake or commercially-motivated reviews) without that moderation burden becoming unmanageable.

**Solution:**

- **Scaffold the writing process as a two-step [[process-funnel|process funnel]]**: first, a title, free-text body, and numerical rating, with concrete writing guidelines (what to cover, what to avoid — e.g. don't spoil endings, don't attack the author personally); second, a review of what was written, exactly as it will appear, before it posts. Both [[amazon]] and Yahoo! Video follow this shape.

![Amazon.com lets customers write a review, then check it before submitting](../../raw/media/vanduyne-2006-advanced-e-commerce/G4.3a.png)

- **Publish use policies and filter automatically** for profanity and outbound links before anything posts, and keep a human editor in the loop afterward — exhaustive pre-screening isn't realistic at volume, so spot-checking plus a "report this" path covers what filters miss. These policies sit alongside a site's broader fair-information and privacy practices (e.g. handling reviews from minors), which is worth involving legal counsel on given the liability exposure.
- **Add meta-ratings.** A "was this review helpful?" vote (Amazon's approach) or a simple +1/0/−1 reputation score (eBay's buyer/seller feedback system) lets the community itself separate trustworthy reviews and reviewers from noise, without the site having to adjudicate quality directly. Implement the vote itself with an [[action-buttons|action button]].
- **Prime the pump.** A new recommendation community needs enough reviews to look credible before it can grow further — surface reviews prominently next to the product they're about, make adding one easy, and consider a direct incentive (a contest, a small reward) for a site's very first reviewers.

**Forces:** the same openness that makes a recommendation community valuable (real, unfiltered customer voices) is what creates its moderation burden — tightening review rules to reduce risk also reduces how authentic reviews feel, so the two pull against each other and the right balance is a legal and editorial judgment call, not a fixed rule. This trade-off is part of why a site's reliability and honesty about its own practices ([[trust-and-credibility]]) matters here as much as the recommendation features themselves.
