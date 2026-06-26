---
type: source
title: "Usability Testing (Wikipedia)"
tags: [usability-testing, evaluation, ux-research, methodology]
related: [usability-evaluation-methods, usability-engineering, customer-research-methods, accessibility]
created: 2026-06-24
updated: 2026-06-24
authors: [Wikipedia contributors]
year: 2026
url: "https://en.wikipedia.org/wiki/Usability_testing"
venue: "Wikipedia"
---

# Usability Testing (Wikipedia)

Wikipedia's article on usability testing, the practice of evaluating a product by testing it directly on real users, contrasted with expert/inspection-based methods.

## Key points

- **Definition.** Usability testing evaluates a product by observing real, previously-unexposed users attempting tasks with it under controlled conditions — distinct from usability *inspection* methods (expert review), where specialists evaluate an interface without users present.
- **Guerrilla testing** (also hallway testing or pop-up research): short, informal interviews in public spaces frequented by likely users — cheap, fast, used early in a design process, but a form of convenience sampling whose results can be biased and need pairing with other methods.
- **Remote testing**: testing with the evaluator and participant separated in space and/or time. Synchronous (moderated) testing uses real-time video/screen-sharing tools; asynchronous (unmoderated) testing has the participant work alone, auto-logged. Improves access for participants with limited mobility, illness, disability, or transportation constraints.
- **A/B testing** (split testing): in Web design/marketing, comparing two page versions identical except for one variable, to see which improves an outcome of interest (e.g. click-through or conversion rate). **Multivariate/bucket testing** extends this to more than two versions at once. This is the same technique this wiki's [[web-site-development-process]] already describes as "virtual testing," credited there to [[amazon]] and [[google]] — Wikipedia supplies the standard name.
- **The "five users" claim.** Jakob Nielsen (Sun Microsystems, early 1990s) popularized testing with as few as five participants per round, formalized by the Nielsen-Landauer formula U = 1 − (1 − p)ⁿ (proportion of problems found, given *p* = per-user detection probability and *n* = number of users) — an asymptotic curve where each additional user finds proportionally fewer new problems.
- **Critiques of the five-user claim.** A small sample isn't representative of the full user population; problems vary in how easy they are to detect, so the formula's constant-probability assumption breaks down for subtle, severe problems requiring larger samples. Empirically, groups of five found 85% of problems on average but with wide variance (as low as 55% in some runs), while no group of twenty found fewer than 95%. Modern practice typically runs 5–10 participants per round, repeated across multiple rounds (Nielsen suggests 50–100 testers cumulatively across a project).
- **Sampling-bias limitations.** Two systemic gaps: (1) underrepresentation of users with disabilities — the WHO estimates 1.3 billion people (16% of the global population) experience significant disability, yet this group is routinely excluded from testing due to recruitment and stakeholder-culture barriers; (2) **WEIRD sampling bias** — Western, Educated, Industrialized, Rich, Democratic populations are ~12% of the world but ~96% of published behavioral-science research participants, and cognitive/perceptual processes (e.g. susceptibility to certain optical illusions) are shown to vary by culture, so usability findings from WEIRD samples may not generalize.
- **Roles**: facilitator (runs the session), note-taker, observers (kept unobtrusive), and participants drawn from the target population.

## Notes for the wiki

A local snapshot is saved at `raw/safe/wikipedia-usability-testing.html` alongside the live URL. Licensed CC BY-SA 4.0, same treatment as this wiki's other Wikipedia sources — content folded in is paraphrased, not quoted.

This wiki already has a concept page covering this exact topic, [[usability-evaluation-methods]] (expert review, informal/think-aloud evaluation, formal studies) — rather than create a duplicate page under a different name, folded this article's genuinely new content into it: a new "Guerrilla testing" note, a "Remote testing" note, a "A/B testing" tie-in linking to the wiki's existing "virtual testing" terminology (in [[web-site-development-process]], [[amazon]], [[google]]), a "How many participants" section (the five-users claim, the Nielsen-Landauer formula, and its empirical critique), and a "Sampling limitations" section (disability underrepresentation, WEIRD bias).

**Excluded:** the article's two worked "Examples" (a 2015 medical-device usability test, the 1982 Apple IIe design guidelines) as one-off case studies rather than generalizable design guidance; the "Education" and "Survey research" sections, which discuss usability testing as a pedagogical/survey-methodology topic rather than UI/UX design practice; and citation-level bibliographic detail.
