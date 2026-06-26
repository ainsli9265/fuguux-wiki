---
type: concept
title: Multiple Destinations
tags: [e-commerce, checkout, design-pattern, shipping]
related: [gift-giving, process-funnel, quick-flow-checkout, action-buttons, grid-layout, walmart, amazon, vanduyne-2006-advanced-e-commerce]
sources: [vanDuyne_G_3PP_491-544.pdf]
created: 2026-06-25
updated: 2026-06-25
---

# Multiple Destinations

**Problem:** customers buying gifts for several people in one order need to ship different items to different addresses, but a standard single-address checkout has no way to express that.

**Solution:**

![Walmart.com offers a "Ship to Multiple Addresses" option during checkout](../../raw/media/vanduyne-2006-advanced-e-commerce/G5.1.png)

- **Offer the option explicitly during checkout**, via a "Ship to Multiple Addresses" [[action-buttons|action button]] at the point where the customer would otherwise enter one shipping address (Walmart's worked example).
- **Reuse the existing address book.** For returning customers, show a pick list of previously-used addresses next to each product in the order, rather than asking them to re-enter destinations from scratch; first-time customers (with an empty address book) go straight to an address-entry form instead.
- **Group the order summary by destination**, not just by product, so customers can verify each address's contents are correct before confirming — with an Edit [[action-buttons|action button]] on each address group, so a mistake doesn't require restarting the whole order. Carry the same per-destination grouping into the printable confirmation page.

**Forces:** none specific to this pattern beyond what [[process-funnel|process funnels]] generally face — every extra address a customer assigns multiplies the number of things that can be wrong in the final review step, which is why a clear, destination-grouped summary matters more here than in a single-address checkout.

This pattern depends on a working single-address checkout already being in place — see [[quick-flow-checkout]] for the full basic checkout flow — it only adds the *branching* needed when one order has to split across recipients, not the checkout flow itself.
