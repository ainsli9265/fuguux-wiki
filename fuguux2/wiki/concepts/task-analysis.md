---
type: concept
title: Task Analysis
tags: [customer-research, ux-process, requirements]
related: [know-your-customers, personas-and-scenarios, customer-research-methods, vanduyne-2006-knowing-your-customers]
sources: [vanDuyne_03_3PP_039-068.pdf]
created: 2026-06-23
updated: 2026-06-23
---

# Task Analysis

A structured way of cataloging what customers currently do and what they want to do, before any design or implementation work starts. A **task** (used interchangeably with *goal*) describes *what* a customer wants to accomplish — "find the best digital camera under $500 and buy it" — deliberately without saying *how* it should be done; the *how* is exactly what the design process is supposed to figure out.

**Process:** identify the target customer population, find people representative of that population, then find out what they actually do. Early on this can be informed guesswork plus informal interviews with task experts; later it gets refined with the methods covered in [[customer-research-methods]] — observation, surveys, and evaluation of competitors' (or your own existing) site. The two should run in tandem — an initial task analysis focuses field investigation, while field evidence should be allowed to overturn the initial analysis, not the other way around.

Sample question categories used to drive a task analysis mirror the four elements in [[know-your-customers]]: **people** (who they are, vocabulary, skills, physical constraints), **tasks** (current behavior, frequency, time constraints, recovery from failure), **technology** (browsers, plug-ins, connection speed, screen size), and **social issues** (work environment, noise/stress level, data sensitivity, who else the data is shared with).

**Two cautionary examples** for why this matters before implementation, not after:
- A company's refund form was effectively undiscoverable through its own site search; the only fallback was a fax number. A task analysis would have surfaced "find and submit a refund form" as a real, common task and led to a downloadable (or directly submittable) online form.
- A dentist's office paid to digitize paper billing forms, only to have staff reject the new system almost outright — the paper forms had carried informal handwritten margin notes (e.g., "this patient's insurance takes longer than most") that the new system had no way to capture. A closer look at how the *existing* artifact was actually used would have caught this before money was spent building the wrong thing.

**Reducing work:** reusing a metaphor customers already know (a paper spreadsheet, a physical shopping cart) lowers the learning burden — but copying an old medium's interface wholesale isn't always right. Recreating a paper telephone directory as flippable page-images on the Web preserves its weaknesses (slow lookup, no partial-match search) instead of using the computer's actual strengths.

## Choosing good tasks

For tasks used in scenarios (see [[personas-and-scenarios]]) or later customer testing, a task should be:

- **Detailed** — specific to the customer and situation, still without specifying *how*.
- **Representative** — a real task customers actually want, even for a genuinely novel site. (Sites like evite.com didn't invent "inviting people to a party and tracking RSVPs" — they moved an existing task online.)
- **Common or important** — either done frequently, or carrying real consequences if done wrong (e.g., getting your registered name/email wrong on an invitation site undermines the whole site).
- **Complete** — a whole activity, not an isolated subtask. A banking site that's only ever tested on "check savings balance," "check checking balance," and "transfer funds" as three separate tasks can still end up clumsy at the realistic combined task — "make sure I have enough in checking to cover this check" — which chains all three and benefits from being explicitly designed as one flow.
