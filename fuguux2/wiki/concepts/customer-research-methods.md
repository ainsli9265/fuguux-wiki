---
type: concept
title: Customer Research Methods
tags: [customer-research, usability-testing, interviews, surveys, focus-groups, ethnography]
related: [know-your-customers, task-analysis, card-sorting, usability-evaluation-methods, vanduyne-2006-knowing-your-customers, digitalgov-2026-interviews]
sources: [vanDuyne_03_3PP_039-068.pdf, digitalgov-interviews.html]
created: 2026-06-23
updated: 2026-06-24
---

# Customer Research Methods

A family of techniques for filling in a [[task-analysis]] and validating the elements described in [[know-your-customers]] with real customer data. No single method is sufficient — qualitative methods (observation, interviews, focus groups) and quantitative ones (surveys) each cover different gaps, and the results feed into [[card-sorting]] once enough raw data has been gathered.

**Ethnographic observation** — watching customers in their normal environment (home, work) rather than only asking them about it. Its core advantage over self-report is that it captures what people actually *do*, not just what they *say* they do, and surfaces context (tools, people they interact with, artifacts they create) that's hard to recall accurately out of context. A rigorous ethnographic study is slow; an informal "ethnographically inspired" version — following someone for a day, photographing their workspace — is much faster and still useful.

**Interviews** — best conducted in the customer's own environment so they can show, not just describe. Practical guidance: avoid interruptions; start with easy questions before harder ones; ask open-ended questions rather than yes/no ones (avoid "Would you like this feature?" — almost everyone says yes; instead show two alternatives and ask which is better, or have people rate a list of features 1–7 on importance); be nonjudgmental; and listen more than you talk. Recording and transcribing interviews catches subtleties that note-taking alone misses.

Run interviews with at least two people on the team — an interviewer and a dedicated notetaker — and prepare a guide of key topics to cover rather than a fixed question script, so the session plays out as a guided conversation rather than a formal Q&A (having a short "elevator pitch" ready helps if a participant asks what the project is about). Two techniques sharpen what you get out of it: the **5 Whys**, repeatedly asking "why" about a vague word or phrase the participant used to draw out the concrete detail behind it; and mirroring the participant's own words back to them in question form rather than leading with your own paraphrase, which avoids cueing them toward the answer you expect. Interviewer bias is treated as unavoidable rather than something to eliminate outright — the practical fix is staying aware of it, not pretending it's absent.

**Surveys** — good for breadth: gathering structured (multiple-choice) and open-ended (free-form) data from many people at once, via mail, phone, in-person intercept, or the Web. Response requires incentive (a T-shirt up to cash, scaled to how long the survey takes and how senior the respondent is) and surveys longer than ~15 minutes see steep drop-off, especially online. The catch: drawing valid quantitative conclusions requires **reliable data** (consistent results if repeated) and **statistical validity** (enough responses, from a representative-enough sample) — a lot of informal Web surveys fail on one or both. Like interviews, surveys report what people *say*, which doesn't always match what they *do*.

**Focus groups** — 6–12 representative customers discussing a site or its competitors together, useful especially early in design for gauging attitudes and reactions to sketches or scenarios. Risks: an overly controlling moderator steering toward a preferred conclusion, a dominant participant triggering groupthink in the rest of the group, and "professional respondents" who join groups for the incentive rather than because they represent real customers. Group chemistry alone can swing results from positive to very negative on the same questions, so running a focus group more than once, with different people in different locations, is safer than trusting a single session. Like surveys, focus groups reveal attitudes, not necessarily behavior.

**Analyzing existing sites** — recruiting representative customers to use and critique an existing or competitor site. Starting from people who already emailed in feedback is convenient but biased — they've self-selected as unusually vocal or expert — so this should be supplemented with a deliberately broader sample.

The unifying caveat across surveys and focus groups: both tell you what people *say*; if you need to know what people will actually *do*, you have to watch them do it.

These methods are about understanding customers *before* a design exists; the analogous toolkit for testing customers against an actual prototype or finished design is [[usability-evaluation-methods]] — observation and interviews here correspond to informal evaluation there, and surveys correspond to formal usability studies.
