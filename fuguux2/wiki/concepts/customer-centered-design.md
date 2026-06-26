---
type: concept
title: Customer-Centered Design
tags: [ux-process, usability-testing, design-philosophy]
related: [web-design-patterns, process-funnel, action-buttons, know-your-customers, iterative-design, web-site-development-process, design-centering-styles, myths-of-customer-centered-design, yahoo, vanduyne-2006-web-design-patterns, vanduyne-2006-knowing-your-customers, vanduyne-2006-involving-customers, vanduyne-2006-customer-centered-web-design, wikipedia-2026-design-of-everyday-things]
sources: [vanDuyne_01_3PP_001-018.pdf, vanDuyne_02_3PP_019-038.pdf, vanDuyne_03_3PP_039-068.pdf, vanDuyne_04_3PP_069-096.pdf, "https://en.wikipedia.org/wiki/The_Design_of_Everyday_Things"]
created: 2026-06-23
updated: 2026-06-25
---

# Customer-Centered Design

A design approach that builds decisions around the customer's existing knowledge, expectations, and goals rather than around internal conventions or guesswork. A site is **customer-centered** when it scores well on five factors: content, ease of use, performance, brand value/trustworthiness, and satisfaction. The term *customer* is used deliberately instead of *user*: it covers anyone who uses or depends on the site (administrators, partners, managers, producers — not just end-customers), and signals that the design has to account for more than usability alone (trustworthiness, brand value, how well the company's other customer-facing channels work).

The "customer" substitution is a deliberate variant of an older term: Donald Norman popularized **user-centered design** (in his 1986 *User-Centered System Design*, then *The Design of Everyday Things*) to mean designing around user needs ahead of secondary concerns like aesthetics — operationalized as simplifying task structure, visibility, getting mapping right, exploiting constraints, designing for error, and explaining affordances (see [[seven-stages-of-action]] and [[affordance]]). This book's authors keep that same priority but widen the term itself to cover everyone a site has to serve, not just its end users.

It rests on two pillars: [[know-your-customers]] — understanding people, their tasks, their technology, and their social context before designing anything — and [[iterative-design]] — keeping customers involved throughout the design and implementation process via repeated prototyping and evaluation, illustrated below. These two pillars are the book's **principles**; **processes** ([[web-site-development-process]]) describe how to put them into practice across a project, and **patterns** (the lettered pattern groups, A–M) are the reusable, tailorable solutions principles and processes are applied through. Principles arbitrate between process activities (e.g. whether to do one more paper-prototype iteration or move to a high-fidelity build) and between competing pattern-based solutions to the same problem.

## Why it matters: the business case

Customer-centered design isn't purely a quality nicety — it's argued to directly affect revenue. One cited case: an unnamed IBM site redesign that simplified and made navigation more consistent (after IBM noticed customers leaned heavily on search and help because they couldn't otherwise find things) led to a sharp drop in search/help reliance and a 400% jump in online sales within a week of launch. More generally, the source's own research found that a 5% increase in customer satisfaction was associated with a 25%-or-greater increase in revenue — driven by easier-to-find products (more repeat visits) and fewer support contacts/returns (lower cost). [[yahoo]] is offered as a standing example: its popularity is attributed less to visual design than to a fast, text-heavy, easy-to-use interface shaped by ongoing field studies, interviews, and usability evaluations baked into its development process.

It's also explicitly contrasted with three design styles it argues against — company-centered, technology-centered, and designer-centered design — covered in [[design-centering-styles]] — and defended against nine common objections to investing in it, covered in [[myths-of-customer-centered-design]].

## In practice: keeping customers involved

People arriving at a Web site bring prior experience with the Web and with physical-world objects (e.g., recognizing shaded buttons as clickable, see [[action-buttons]]); a customer-centered design deliberately reuses those expectations instead of inventing unfamiliar interactions.

In practice, this means keeping customers in the loop throughout the design process rather than only at the end. A worked example in the source: a designer noticing checkout abandonment in server logs, consulting relevant design patterns (e.g., [[process-funnel]]) to generate candidate fixes, sketching alternatives, then validating them by recruiting a small number of representative customers (five, in the example) to walk through both the existing and the redesigned flow. Observing real customers surfaced problems the design team had not anticipated — e.g., a key button positioned below the fold was invisible on smaller/older monitors, causing users to click the wrong link and lose entered form data when they fell out of the flow.

This also points to a methodological caveat: when the observer is present during testing (as in informal in-home sessions), participants may complete a task despite real usability problems, an effect attributed to testing bias — task completion alone shouldn't be read as evidence that a flow is easy to use.
