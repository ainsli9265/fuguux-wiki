---
type: concept
title: Seven Stages of Action
tags: [cognition, design-principles, mental-models, history]
related: [affordance, interface-design-principles, accessibility, wikipedia-2026-design-of-everyday-things]
sources: ["https://en.wikipedia.org/wiki/The_Design_of_Everyday_Things"]
created: 2026-06-25
updated: 2026-06-25
---

# Seven Stages of Action

Donald Norman's model of how a person actually carries out and checks any action, from "I want more light" to threading a film projector — split into four **execution** stages and three **evaluation** stages:

**Execution** (doing something to the world):
1. Forming the **goal** — the state to be achieved (e.g., "I need more light to keep reading").
2. Forming the **intention** to act on that goal.
3. **Specifying an action** — translating the intention into a concrete sequence (reach toward the lamp, extend a finger toward the switch).
4. **Executing** the action — actually performing it.

**Evaluation** (checking whether it worked):
5. **Perceiving** the state of the world after acting.
6. **Interpreting** that perception.
7. **Evaluating** the interpretation against the original intention and goal.

Norman built this model after watching, at an Italian conference, several people in succession fail to thread a film projector none of them had used before — confusion compounding as more people tried to help, until a technician fixed it in seconds. The puzzle wasn't that the task was hard in the abstract; it was that nothing about the projector communicated what to do, at any of these seven points.

## The two gulfs

Splitting the cycle in half exposes two distinct kinds of failure (both terms actually predate this book, first appearing in Norman's 1986 *User-Centered System Design*):

- **Gulf of execution** — the gap between what someone intends and what the system's actual, allowable actions are. The book's VCR example: a customer wants to "record this show," which feels like it should be one action, but actually requires pressing record, setting a time, selecting a channel, and confirming — each an extra, separately-learned step the customer's mental model of "just record it" didn't anticipate. [[affordance|Affordances and signifiers]] exist specifically to narrow this gulf, by making the allowable actions visible and obvious rather than hidden behind unmarked menus or modes.
- **Gulf of evaluation** — the effort needed to figure out, after acting, whether it worked: interface → perception → interpretation → evaluation. This gulf is small when a system's state is easy to perceive, easy to interpret, and matches how the person already thinks about it — and large when, as in the projector example, there's no way to tell from looking whether the film was even threaded correctly until it's run.

## Design implications

The seven stages double as a checklist for design review — at each stage, ask whether the gulf of execution or evaluation is being widened — and the book distills this checklist into four principles:

- **Visibility** — a customer can tell, just by looking, what state the system is in and what actions are available.
- **A good conceptual model** — the system presents itself consistently enough that a customer can build an accurate mental picture of how it works, rather than a wrong one that leads to confident mistakes.
- **Good mappings** — the relationship between a control and its effect (and between system state and what's visible) is intuitive rather than arbitrary.
- **Feedback** — the customer gets continuous, legible information about what just happened. This is the same principle [[interface-design-principles]] already documents in depth (its second principle, "offer informative feedback") — see that page for the loading-indicator and progress-display detail this article doesn't go into.

A small gulf of evaluation is also why [[accessibility]] concerns (e.g., a status that's only ever communicated by a color change) compound for some customers: if a system's state isn't perceivable through more than one channel, the gulf of evaluation widens specifically for whoever can't use that one channel.
