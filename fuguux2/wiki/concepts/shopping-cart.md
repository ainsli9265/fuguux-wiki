---
type: concept
title: Shopping Cart
tags: [e-commerce, cart, process-funnel, conversion, persistence]
related: [process-funnel, quick-flow-checkout, clean-product-details, cross-selling-and-up-selling, action-buttons, multiple-destinations, gift-giving, order-tracking-and-history, barnes-and-noble, vanduyne-2006-basic-e-commerce]
sources: [vanDuyne_F_3PP_431-490.pdf]
created: 2026-06-25
---

# Shopping Cart

The shopping cart is the holding area between browsing and buying. Its design has to serve two distinct customer states simultaneously: a customer who is ready to purchase right now, and a customer who is collecting items to evaluate later or return to on a subsequent visit.

## Accessibility from every page

The cart should be reachable from every page of the site — typically via a persistent icon (shopping bag, cart) in the header that shows the current item count. This serves as both a navigation target and a visual confirmation that adding an item succeeded. A customer should never have to wonder "did that add?" — the cart indicator updates immediately.

## Clear add-to-cart interaction

The Add to Cart button on a [[clean-product-details|product page]] should be unambiguous in both label and placement. After adding an item, the customer should receive a clear confirmation — an updated cart count, a brief confirmation message, or a mini-cart dropdown — and a clear path to either continue browsing or proceed to checkout. Forcing a redirect to the cart page on every add-to-cart interrupts browsing for customers who want to accumulate multiple items.

## Allow browsing without an account

Do not require login or account creation before adding items to the cart. Customers should be able to browse and accumulate selections before committing to a purchase or an account. The checkout flow handles account identification — the cart is not the right moment to demand it.

## Cart content display

Each item in the cart needs enough detail to be recognizable without returning to the product page:

- Product name and a brief description or variant (size, color, edition)
- Availability status — confirm the item is in stock or flag if stock is uncertain
- Price per unit
- Quantity selector with an easy way to change quantity or remove the item
- Item subtotal

The cart should also show a running order subtotal, and a shipping estimate if it can be calculated at this stage. Surprises at the payment step — unexpected shipping costs, unavailable stock — are among the most common causes of checkout abandonment.

## Navigation balance

The cart page must present two paths without favoring one over the other inappropriately: continue shopping (to add more items) and proceed to checkout (to complete the purchase). The balance point depends on the site: a high-consideration purchase site (furniture, electronics) may want to make "continue browsing" easy; a consumables site may benefit from emphasizing "check out." Both links should be clearly visible. Hiding or obscuring "continue shopping" frustrates customers who wanted to add one more item.

## Persistence

Carts should persist for returning customers — at minimum 24 hours, ideally for the customer's full consideration period (which for high-cost purchases may be days or weeks). A customer who spends time building a cart, leaves, and returns to find it empty has lost real effort and is unlikely to rebuild it. Persistent carts also function as a form of wish list for customers who are not yet ready to buy.

## Wish lists

A wish list is a second holding area, distinct from the cart, for items a customer wants to save for later without yet intending to purchase. It serves customers who are in a research or gift-planning mode. The key design decisions: make it easy to move items from the cart to a wish list and back; make wish lists persistent across sessions; allow sharing a wish list (supporting [[gift-giving|gift purchase]] by others). [[barnes-and-noble|Barnes & Noble]]'s site is a cited example: items move directly from the wish list to the cart, and lists can be shared with others for gift planning. The cart and wish list serve different intentions — the cart implies near-term purchase intent, the wish list implies deferred or potential purchase intent — and conflating them removes a useful signal.

## Cross-selling and localization

[[Cross-selling-and-up-selling|Cross-sells]] in the cart are appropriate but should be visually secondary to the cart contents and checkout action. Prominence that rivals the checkout path turns a cross-sell into a distraction.

Terminology for the cart itself varies by market: "shopping cart," "shopping basket," and "shopping bag" each carry associations. The dominant usage in a given market or locale is worth observing — presenting what customers already expect removes one unnecessary source of confusion.
