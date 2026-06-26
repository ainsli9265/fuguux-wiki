---
type: concept
title: Multiple Ways to Navigate
tags: [navigation, design-pattern, information-architecture]
related: [browsable-content, search-action-module, straightforward-search-forms, action-buttons, process-funnel, consistent-sidebars-of-related-content, grid-layout, web-design-patterns, vanduyne-2006-creating-navigation-framework, homepage-portal]
sources: [vanDuyne_B_3PP_215-266.pdf]
created: 2026-06-24
updated: 2026-06-24
---

# Multiple Ways to Navigate

**Problem:** customers reach a goal on a Web site in different ways depending on what brought them there in the first place; a site that only supports one of those ways will feel tedious or shallow to everyone else.

**Background:** customers are driven to act by two distinct motivators — **intention** (a goal or task they arrived with, from very specific to vaguely "looking around") and **impulse** (something that grabs their attention once they're already on the site, like a promotion or a related item). Neither is inherently better; a site that omits intention-based navigation feels shallow, and one that omits impulse-based navigation feels boring.

**Solution:** support both motivators with distinct navigation styles, each suited to a different one:

- **Search** and **browse** (intention) — the familiar styles for someone who already knows, or roughly knows, what they want. See [[search-action-module]] and [[straightforward-search-forms]] for search; [[browsable-content]] for browse.
- **Next-step** ("wizard") (intention) — guiding someone step by step toward a goal that requires more than one decision; see [[process-funnel]] for the canonical strict version of this.
- **Relate** and **promote** (impulse) — surfacing related items or promotions that someone wasn't looking for but might act on anyway; see [[consistent-sidebars-of-related-content]].

**Placement follows the same logic as the motivator itself.** Intention-driven tools (search, browse) need to be near where customers start reading, since these are the tools that get a visit started — losing them to obscurity loses the visit. Next-step tools that *continue* a goal already in motion belong near the top but on the opposite side from where reading starts (conventionally top right), so they're visible without scrolling but don't compete with the starting point; they're often repeated at the bottom too, since that's where attention naturally ends up after scanning the whole page. Impulse-driven tools (relate, promote) get the least valuable screen space — lower on the page, or opposite the starting point — precisely because you can't guarantee a customer will act on them the way you can expect them to use an intention-driven tool they came looking for.

**Forces:** every navigation tool needs a single, consistent place to live across the whole site, or customers can't build the expectation that lets them find it quickly a second time — this pattern depends on a strong [[grid-layout]] inside a consistent page template to hold all of these tools in place page after page. Once a customer commits to a next-step path, clearly distinguished [[action-buttons]] help them complete it without falling out partway through.

The [[homepage-portal|homepage]] is where this pattern is under the most pressure: it has to make every one of these styles findable at once, in the page with the least room to spare.
