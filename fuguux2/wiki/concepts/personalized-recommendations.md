---
type: concept
title: Personalized Recommendations
tags: [e-commerce, recommendations, design-pattern, personalization, privacy]
related: [featured-products, cross-selling-and-up-selling, recommendation-community, process-funnel, trust-and-credibility, lands-end, vanduyne-2006-advanced-e-commerce]
sources: [vanDuyne_G_3PP_491-544.pdf]
created: 2026-06-25
updated: 2026-06-25
---

# Personalized Recommendations

**Problem:** personalized recommendations make shopping easier when they're good, but generating them well requires real customer data — and the easiest data to collect (where someone clicked, what they searched for) is also the least reliable.

**Solution:** prefer recommendations grounded in deliberate customer behavior over data inferred from incidental browsing:

- **Avoid purely inferred data.** A page visit alone doesn't mean a customer wanted what's on that page — they might have clicked the wrong link or mistyped a search term. Recommendations built only on referrer logs or path data can ring hollow because the underlying signal is noisy.
- **Make rating easy and immediate.** Letting customers rate products they've bought (or are just familiar with) gives a much more reliable signal than inference, but only if the friction is low — e.g. a rating control that updates the page instantly rather than requiring a form submission and reload.

![Lands' End asks customers a short series of preference questions, then offers customized recommendations](../../raw/media/vanduyne-2006-advanced-e-commerce/G3.4a.png)

- **Offer a short preference interview as an alternative to ratings**, especially for complex or unfamiliar product categories — a brief [[process-funnel|process funnel]] (Lands' End's clothing-preference questionnaire is the worked example) that ends in tailored suggestions. Keep it short and tell customers up front how long it'll take, since a long interview with unclear payoff invites abandonment.
- **Explain *why* a recommendation was made**, in plain terms ("customers who liked X also liked these") rather than describing the algorithm — customers who don't understand or trust a recommendation's basis tend to ignore it.
- **Show several recommendations at once, including ones the customer is known to already like.** This lets customers sanity-check the system themselves: if it's surfacing things they already know they like, they're more likely to trust the new suggestions mixed in alongside them.
- **Address privacy directly.** Personalization runs on the same customer data that [[trust-and-credibility]] says has to be handled visibly and honestly — disclose what's collected and how it's used, and use explicit opt-in for anything beyond the recommendation itself (e.g. using the data for outside marketing).

**Forces:** the more deliberate and specific the data a recommendation is based on (an explicit rating, an interview answer), the more reliable it is — but also the more effort it asks of the customer, so each technique trades signal quality against participation.
