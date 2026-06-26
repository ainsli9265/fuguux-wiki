---
type: concept
title: Usability Engineering
tags: [usability-testing, evaluation, ux-research, history]
related: [iterative-design, usability-evaluation-methods, interface-design-principles, customer-research-methods, wikipedia-2026-usability-engineering]
sources: ["https://en.wikipedia.org/wiki/Usability_engineering"]
created: 2026-06-24
updated: 2026-06-24
---

# Usability Engineering

**Definition:** the professional discipline that studies and tests the usability of interactive systems, drawing on computer science and psychology to identify *why* something is hard to use. It's distinct from UX or interaction design in where it focuses effort: a usability engineer concentrates on the research and testing phase — surfacing problems — while a UX or interaction designer focuses on solving them. In practice the two roles work together throughout [[iterative-design]]'s design→prototype→evaluate cycle.

## Origins

The field traces to 1988, when John Whiteside (Digital Equipment Corporation) and John Bennett (IBM) identified three activities as central to building usable systems: setting goals early, evaluating iteratively, and prototyping — the same three-step cycle this wiki documents as [[iterative-design]], named here for the first time. Jakob Nielsen's 1993 book *Usability Engineering* became the field's defining text, describing how to test a product throughout development — checking for barriers to five qualities — rather than discovering problems only after launch.

## The five usability attributes

Nielsen's framework names five qualities a usability evaluation should check a design against:

- **Learnability** — how quickly a new user can become proficient
- **Efficiency** — how quickly an experienced user can complete tasks
- **Memorability** — how well infrequent users retain proficiency between visits
- **Errors** — how often errors occur, how severe they are, and how easily they're recovered from
- **Satisfaction** — how pleasant the system is to use, subjectively

These give concrete substance to *what* [[usability-evaluation-methods]]'s expert reviews, informal evaluations, and formal studies are actually testing for.

## ISO 9241's definition

The ISO 9241 standard (part 11) operationalizes usability as the **context, efficiency, and satisfaction** with which specified users can achieve specified goals — a more formal, standards-body counterpart to Nielsen's five attributes, used by usability engineers to ground interface requirements in an accepted definition rather than an informal one.

## Errors: slips vs. mistakes

A two-part taxonomy of human error, useful for diagnosing *why* an error happened rather than just that it did:

- A **slip** is the right goal, executed via the wrong action — typos, clicking the wrong menu item — typically a failure of automatic behavior rather than judgment.
- A **mistake** is a consciously deliberated but wrong goal in the first place — the user's plan itself was flawed.

A **mode error** is a particularly dangerous slip subtype: the user acts correctly for the mode they *believe* they're in, but the system is actually in a different one (e.g. a car in reverse instead of drive). Designers mitigate mode errors either by avoiding modes altogether (modeless interfaces) or by requiring a continuous action to remain in a special mode, so leaving the mode is automatic the moment the action stops (e.g. holding a key to keep Photoshop's lasso tool active). This sharpens [[interface-design-principles]]'s fourth principle (helping customers avoid and recover from errors): preventing slips and preventing mistakes call for different design responses, since one is about reducing accidental wrong actions and the other is about catching a wrong plan before it's acted on.

One technique named in this source but documented in full on [[usability-evaluation-methods]] rather than here: the **RITE method** (Rapid Iterative Testing and Evaluation), a faster variant of the evaluation methods in [[usability-evaluation-methods]] and [[customer-research-methods]].
