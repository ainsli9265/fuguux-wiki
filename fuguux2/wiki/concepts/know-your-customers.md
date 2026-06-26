---
type: concept
title: Know Your Customers
tags: [customer-research, ux-principles, human-factors]
related: [customer-centered-design, accessibility, task-analysis, personas-and-scenarios, customer-research-methods, iterative-design, web-site-development-process, vanduyne-2006-knowing-your-customers, fitts-law]
sources: [vanDuyne_03_3PP_039-068.pdf]
created: 2026-06-23
updated: 2026-06-24
---

# Know Your Customers

The first of two pillars of [[customer-centered-design]] (the second being [[iterative-design]], keeping customers involved iteratively). Its starting premise: *you are not your customers* — design teams don't share their customers' experience, vocabulary, or working habits, so intuition alone can't substitute for actually understanding them.

## The four elements

Every design balances four competing elements, each exerting its own forces on the outcome: **people**, **tasks**, **technology**, and **social/organizational context**. None should dominate; the job is to balance them.

- **People** — two layers: individual differences (demographics, vocabulary, domain expertise — a site for medical professionals can assume jargon a site for pre-med students can't) and general human abilities (perception, memory, motor control), drawn from cognitive psychology, ergonomics, and HCI. One concrete law: [[fitts-law|Fitts's Law]] — the time to move a pointer to a target depends on distance and target size — meaning small or distant links and buttons are measurably harder to click, which is why patterns favor larger, nearer calls to action. A related perceptual constraint is covered in its own page: [[accessibility]].
- **Tasks** — see [[task-analysis]] for the technique. One useful design move is to reduce the work customers have to do by reusing a metaphor they already know (a spreadsheet program borrowing the paper spreadsheet; e-commerce borrowing the shopping cart) — but a metaphor should improve on, not just imitate, the original (a Web "page-turning" telephone directory that ignores the Web's search capability is the cautionary counter-example). There's also a real difference between *ease of learning* and *ease of use*: not everything must be usable on first try (Douglas Engelbart: "If ease of use was the only valid criterion, people would stick to tricycles and never try bicycles"). But customers have little patience for training on a Web site specifically, compared to desktop software they've already paid for and installed — futurist Paul Saffo describes a "threshold of indignation," the point past which people simply abandon a tool that asks too much of them for too little payoff.
- **Technology** — capabilities and limits of what customers actually have (browsers, plug-ins, connection speed, screen size). Two failure modes: ignoring technology entirely (sites that silently fail for anyone without the latest plug-in) and over-indexing on a favored technology ("technology for technology's sake," prioritizing a tool over customer needs). A concrete constraint: response times around 100ms are needed for direct-manipulation actions (dragging, typing), and around 1 second to preserve an uninterrupted flow of thought for routine actions like clicking a button — real but not absolute constraints, since current Web/network conditions make sub-second loads everywhere unrealistic. Rule of thumb: people and tasks first, technology second.
- **Social/organizational issues** — how a Web site fits into existing organizational culture and workflow, not just individual behavior. Leysia Palen's 1999 study of group calendaring software at two large tech companies found that **default settings** mattered more than configurability: over 80% of users kept whatever default was set, and the "right" default (e.g., whether a shared calendar shows full event detail or just "busy") differed sharply between the two organizations' cultures around privacy and control. The lesson generalizes: adding a customization option doesn't solve a bad default, because most people never change it. It's also worth distinguishing the *customer's* organizational goals from the *client's* — they can diverge, and reconciling that early avoids late-stage conflict.

## A bias to watch for: customers who don't return

Borrowed from a WWII anecdote about reinforcing aircraft armor: researchers nearly recommended adding armor wherever returning planes showed bullet damage, until someone pointed out they should study the planes that *didn't* return — the ones hit in the locations that actually mattered. Applied to Web analytics: studying only customers who keep coming back overlooks the people who hit a barrier and left for good, who are arguably more informative about what's broken.

This four-element analysis is the substance behind the customer analysis document produced in [[web-site-development-process]]'s Discovery phase, and the same questions get revisited when evaluating competitor sites in that phase's research step.
