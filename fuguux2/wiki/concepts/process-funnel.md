---
type: concept
title: Process Funnel
tags: [task-flow, e-commerce, checkout, design-pattern]
related: [web-design-patterns, action-buttons, customer-centered-design, iterative-design, interface-design-principles, vanduyne-2006-web-design-patterns, vanduyne-2006-involving-customers, content-organization-schemes, multiple-ways-to-navigate, form-design, quick-flow-checkout, shopping-cart, easy-returns]
sources: [vanDuyne_02_3PP_019-038.pdf, vanDuyne_04_3PP_069-096.pdf, vanDuyne_F_3PP_431-490.pdf]
created: 2026-06-23
updated: 2026-06-24
---

# Process Funnel

A sequence of pages designed to walk a customer through one specific, well-defined task (e.g., a purchase checkout), step by step, completing one of the higher-level patterns described in [[web-design-patterns]]. Effective process funnels keep instructions concise, minimize links that could lead someone out of the sequence, and minimize the total number of steps required to finish.

An e-commerce checkout is the running example of a process funnel: it fails when it has hidden charges, tedious text entry, confusing link labels, extraneous buttons, or overly complex instructions — any of which can cause cart abandonment before a sale completes. The e-commerce checkout pattern is fully documented in [[quick-flow-checkout]], which covers the four-step structure, checkout step design (address, shipping, payment, order summary, confirmation), and relationship to [[shopping-cart]] and [[easy-returns]].

A specific, observed failure mode: if a customer accidentally clicks a link that exits the funnel, browser back-navigation often does not restore the data they had already entered, forcing them to redo the step — a critical error that compounds whatever caused the accidental exit in the first place (e.g., a call-to-action button positioned below the fold, easily missed on smaller screens). This failure was caught through direct observation of real customers — see [[customer-centered-design]]. Each step of a process funnel benefits from a clearly distinguished [[action-buttons|action button]] to reduce the chance of a customer clicking the wrong thing and falling out of the funnel.

A related, more abstract pattern noted in the source is **shopping cart** persistence: how long unpurchased items should remain in a cart before being cleared. Clearing too aggressively can lose a sale when a customer returns expecting their selections to still be there.

Distinct from [[content-organization-schemes|task-based organization]], a looser sibling pattern: a process funnel forces one narrow, specific task through a fixed sequence with few choices at each step, while task-based organization *offers* a relevant next step among several rather than mandating one. In the vocabulary of [[multiple-ways-to-navigate]], a process funnel is the canonical "next-step" navigation style — intentional, sequential, and narrow by design.

A process funnel is also the canonical example, in [[iterative-design]] and [[interface-design-principles]], of deliberately restricting customer control and freedom in order to help them complete a task — e.g. applying one after server logs and a usability study show customers abandoning a multi-step community-posting flow partway through.

## Further reading

Victor Ponamariov's *50 Tips to Improve User Interface* (self-published ebook, no stated license — not ingested into this wiki; see `raw/copyrighted/50_ui_tips.pdf`) addresses multi-step forms from two angles: progress elements in complex forms leverage the goal gradient effect (people accelerate toward a visible finish), restating the progress-indicator rationale in [[interface-design-principles]] from the user-motivation side. The same source argues against placing complex forms inside modal overlays — modals lack a stable URL, can scroll-collide with background content, risk accidental dismissal, and reduce mobile screen space — which reinforces this pattern's core requirement that each funnel step have a reliable, dedicated page. See [[form-design]] for the full forms treatment.
