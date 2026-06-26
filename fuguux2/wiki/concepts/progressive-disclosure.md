---
type: concept
title: Progressive Disclosure
tags: [information-architecture, cognitive-load, navigation, ux-principles]
related: [hicks-law, above-the-fold, loading-states, homepage-portal, form-design, multiple-ways-to-navigate, interface-design-principles, wikipedia-2026-progressive-disclosure]
sources: ["https://en.wikipedia.org/wiki/Hick%27s_law", "https://en.wikipedia.org/wiki/Progressive_disclosure"]
created: 2026-06-26
---

# Progressive Disclosure

Progressive disclosure is the practice of presenting only the information or choices necessary for the current step, revealing additional detail when it becomes relevant to the task at hand. The goal is to reduce cognitive load at each decision point without removing options — the full capability remains available, deferred until the user actually needs it.

The macOS print dialog is the canonical example: the default view shows only the most commonly needed controls; clicking "Show Details" expands the panel to reveal a full set of advanced options. The simpler state is not a limitation — it is the default deliberately chosen for the common case.

## Rationale

Two mechanisms explain why progressive disclosure works. First, [[hicks-law|Hick's Law]]: decision time grows logarithmically with the number of choices presented simultaneously. Showing fewer choices at once reduces the immediate decision load even when the total number of options is unchanged. Second, working memory: people can hold roughly four to seven items in active attention at once; an interface that presents more than that simultaneously forces users to mentally track things rather than decide among them.

Progressive disclosure doesn't solve these problems by removing content — it solves them by *timing* content appropriately. A secondary option that never shows until it's needed is both less cognitively expensive and easier to find when it is needed, because it has no other options to compete with.

The principle extends beyond digital interfaces. Theme park queue designers use it physically: rather than making the full length of a long ride queue visible at once (which would discourage visitors from joining), only a short segment is visible from any vantage point. As visitors advance, the next segment reveals itself. The same underlying logic applies — the total length hasn't changed, but exposure is metered to reduce the perceived burden at each moment.

## Common applications

- **Navigation menus** — a top-level navigation shows categories; subcategories appear on hover, click, or drill-down rather than all at once. The hierarchical structure is itself a progressive-disclosure arrangement: each level is revealed only after the level above has been traversed.
- **Above-the-fold / below-the-fold layout** — [[above-the-fold]] content presents the essential decision elements first; detail is disclosed below as the user scrolls. A [[clean-product-details|product details page]] is a canonical instance: purchase-critical information above the fold, full specifications and reviews below it.
- **Multi-step forms and funnels** — a [[process-funnel]] reveals each step in sequence rather than presenting the entire form at once. A [[quick-flow-checkout|checkout flow]] breaks the overall task into four steps (account, shipping, payment, confirmation), each presenting only what's needed for that stage.
- **"Show more" and "Advanced options"** — interfaces that hide secondary or expert-level controls behind an expandable section present a simpler default state without removing capability for users who need it.
- **Progressive loading** — content rendered incrementally as it arrives, rather than blocking until everything is ready, is a temporal form of progressive disclosure (see [[loading-states]]).

## Relationship to the 95/5 rule

[[homepage-portal]]'s 95%/5% rule — dedicating most [[above-the-fold|above-the-fold]] space to the dominant audience's needs and surfacing rarer needs on a subsidiary page — is a concrete instance of progressive disclosure applied to homepage design. The principle is the same: present the common case prominently; disclose the uncommon case on demand rather than cluttering the primary view with it.

## Limits

Progressive disclosure shifts cognitive cost rather than eliminating it. Content hidden behind a "show more" link is less findable for users who don't know to look for it. Applied carelessly, it can frustrate expert users who already know what they need and have to take extra steps to reveal it. The tradeoff is between a cleaner default state (benefiting novices and occasional users) and a more efficient expert experience (which may benefit from having more exposed at once). Interfaces that serve a wide ability range often need both paths.
