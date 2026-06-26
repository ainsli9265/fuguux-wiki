---
type: concept
title: Personas and Scenarios
tags: [customer-research, design-artifacts, ux-process]
related: [task-analysis, know-your-customers, card-sorting, web-site-development-process, vanduyne-2006-knowing-your-customers, vanduyne-2006-glossary]
sources: [vanDuyne_03_3PP_039-068.pdf, vanDuyne_Glos_3PP_867-896.pdf]
created: 2026-06-23
updated: 2026-06-24
---

# Personas and Scenarios

Tools built on top of [[task-analysis]] for trying out design ideas before any software exists, often seeded by [[card-sorting|card sorting and affinity diagramming]].

A **scenario** is a context-rich story focused on *what* a customer will do, not *how* (close to a software-engineering *use case*). Example, for a hypothetical gift-shopping site:

> Victoria is a bright, young college student looking for a gift for her younger sister, who is turning 16 in two weeks... She's heard some of her friends talk about ebirthdayz.com, so she decides to check it out... Victoria finds the recommendations screen and views gifts based on her sister's age and general interests, as well as her own limited finances... Total time spent: 20 minutes.

Note what the scenario deliberately leaves out: it never says where the recommendation feature lives on the page or how recommendations are computed — at this stage the point is to test whether the *idea* is compelling, not to lock in an interface.

A **persona** is a detailed, recurring fictional customer (name, background, what they do, where they live) used across multiple scenarios so design questions can be checked against a consistent, specific person rather than an abstract "user." E.g., "Would Victoria use a feature for sending business gifts to colleagues? No — she's a college student, that's irrelevant to her." Reusing the same personas throughout a project lets the team sanity-check whether decisions still make sense as the design evolves. The book also uses the lighter-weight term **profile** for a shorter, less-detailed customer description assembled directly from research findings — useful early in Discovery, before a full persona has been fleshed out.

A **storyboard** is a rough, sketched sequence of pages showing how a persona would carry out one task — deliberately kept low-fidelity rather than polished, so the team isn't tempted to treat early ideas as final.

Scenarios and personas also point toward which design patterns are likely relevant before any pattern is chosen: a gift-shopping scenario like Victoria's implies looking at personalization and gift-giving patterns in addition to the basic e-commerce patterns every shopping site needs. They're also useful for communicating intent to clients and stakeholders who haven't been in the research itself — the customer analysis document in [[web-site-development-process]]'s Discovery phase is typically built around exactly this kind of persona work.
