---
type: concept
title: Iterative Design
tags: [ux-process, iterative-design, design-methodology]
related: [customer-centered-design, know-your-customers, rapid-prototyping, usability-evaluation-methods, interface-design-principles, process-funnel, web-site-development-process, vanduyne-2006-involving-customers, usability-engineering]
sources: [vanDuyne_04_3PP_069-096.pdf]
created: 2026-06-24
updated: 2026-06-24
---

# Iterative Design

The second pillar of [[customer-centered-design]] (the first being [[know-your-customers]]): repeatedly cycling through **design → prototype → evaluate** with measurable goals, refining a Web site until it meets or surpasses them, rather than designing once and shipping. The premise is that no design team has complete information about customer needs, so the process is built to compensate for that gap rather than assume it away. This three-step cycle traces to 1988, when John Whiteside and John Bennett isolated early goal-setting, iterative evaluation, and prototyping as the key activities of [[usability-engineering]] — the discipline this cycle is the central technique of.

## The three-step cycle

1. **Design** — consider business goals and customer needs, set measurable goals, develop design concepts.
2. **Prototype** — build artifacts ranging from scenarios and storyboards to running sites (see [[rapid-prototyping]]).
3. **Evaluate** — assess whether the prototype meets the goals set in step 1 (see [[usability-evaluation-methods]]).

The results feed the next iteration. Design patterns help move quickly through each step: high-level patterns rough out early features, low-level patterns help storyboard specific scenarios, and patterns are consulted again to fix problems evaluation turns up.

## Why iterate: the cost of late fixes

Architect Frank Lloyd Wright's line — "an architect's most useful tools are an eraser at the drafting board, and a wrecking bar at the site" — captures the core argument: errors are roughly **10x** more expensive to fix late in a project than if caught early, and **100–1000x** more expensive once the site has shipped (a figure attributed to software-engineering research, e.g. Watts Humphrey). Downstream changes are expensive for three reasons: every later deliverable has to be made consistent with the change, one change often forces others, and anything touching source code/HTML is costly to redo. Studies cited from the Standish Group International attribute many IT project failures specifically to a lack of end-customer input — the problem iterative design is meant to solve.

## The right-feature / right-implementation framework

Design mistakes fall into a 2×2 grid crossing **feature** (right vs. wrong) with **implementation** (right vs. wrong):

- Right feature, wrong implementation — e.g. a shopping cart that's the correct feature for an e-commerce site but is hard to actually check out with. Iterative testing surfaces these.
- Wrong feature, right implementation — e.g. a beautifully-built advanced search that most customers don't understand or need.
- Wrong feature, wrong implementation — neither useful nor functional.

The goal is the fourth quadrant: right feature, right implementation. Iterative design pushes a project toward it by continually feeding customer feedback about both dimensions back into the next design pass.

## Goals and principles

Design **goals** (faster task completion, fewer errors, higher conversion, more repeat visits, etc.) come from analyzing business and customer needs — see [[know-your-customers]]. Design **principles** — seven of them, adapted from Shneiderman, Nielsen, and Tufte — guide *how* patterns get applied to reach those goals; they're substantial enough to warrant their own page, [[interface-design-principles]]. The two are complementary: goals are the destination, principles are the route.

Achieving goals requires testing and measuring. Useful metrics include task completion time, task success rate, ease-of-learning (time or attempts needed to reach proficiency), error rate (with errors explicitly defined in advance, since something as simple as clicking the browser Back button is ambiguous), shopping-cart abandonment rate, and subjective measures like satisfaction or "fun," gathered via surveys. A metric like cart abandonment can have multiple root causes beyond interface design — pricing, missing inventory, surprise shipping costs — so a single number rarely diagnoses the actual problem on its own. Getting statistically meaningful numbers typically requires 20–50 research participants. These site-level metrics are themselves only proxies for higher-level business goals (e.g. revenue), which prototypes generally can't measure directly.

Information architecture (structuring content), navigation design (helping customers move through that structure), and graphic design (visual communication via color, type, layout) are the three design activities iterative design is applied to; they overlap, and traditional "user interface design" sits mostly at the intersection of navigation design and usability evaluation. None can compensate for failure in another — rich graphic design can't fix a poor information architecture, and vice versa.

This cycle scales up beyond a single prototype: the [[web-site-development-process]] applies design→prototype→evaluate both across an entire project's seven phases and within each individual phase.
