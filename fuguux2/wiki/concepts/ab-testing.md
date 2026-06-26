---
type: concept
title: A/B Testing
tags: [usability-testing, evaluation, ux-research, quantitative]
related: [usability-evaluation-methods, iterative-design, web-site-development-process, customer-centered-design, amazon, google]
sources: [vanDuyne_05_3PP_097-116.pdf, vanDuyne_04_3PP_069-096.pdf, "https://en.wikipedia.org/wiki/Usability_testing"]
created: 2026-06-26
---

# A/B Testing

A/B testing (also called split testing) is a controlled experiment comparing two versions of a page or interface element that are identical except for one variable, run simultaneously on real users. The two versions (A and B) are served randomly to different segments of the live user population; behavioral outcome metrics (click-through rate, conversion rate, task completion, time on page) are measured and compared. Whichever version produces the better outcome on the target metric is the winner.

The technique is sometimes called **virtual testing** in the context of full-page redesigns — a new site design is shown to a small subset of customers while the rest continue to see the current version, letting the team compare behavior across the two groups before committing to a complete switch. This is the form credited in [[web-site-development-process]] to [[amazon]] and [[google]], who used it to validate site redesigns rather than launching blindly to all users. **Multivariate testing** (or bucket testing) extends the approach to more than two versions simultaneously, allowing multiple variables to be tested in a single experiment.

## What A/B testing answers

A/B testing answers *which* version performs better on a specific metric — it does not answer *why*. It is a quantitative complement to qualitative methods. Where an informal [[usability-evaluation-methods|think-aloud usability test]] reveals why users struggle (what confused them, what they expected instead), an A/B test measures the magnitude of a behavioral difference under real-world conditions with a statistically representative sample.

The appropriate question for A/B testing is narrow and measurable: "Does version B produce more clicks on the primary action?" rather than "Is version B better overall?" Broader questions require qualitative evaluation and design judgment, not an A/B test.

## Requirements

A/B tests need enough traffic to reach statistical significance — a difference that's real rather than noise. Low-traffic sites and early-stage designs rarely generate enough events to detect small differences meaningfully. Running an A/B test on a low-traffic page and reading a trend as conclusive before significance is reached is a common misuse of the method.

Tests should change only one variable at a time, so results are attributable to that variable. A test that simultaneously changes button color, copy, and page layout cannot tell which change drove the outcome. Multivariate tests can handle multiple variables, but require proportionally more traffic to maintain significance per variant.

## Placement in the design process

A/B testing fits later in the design lifecycle than informal usability testing — it is most useful once a design is live or nearly live and the goal is to optimize an already-functional flow, not to discover fundamental usability problems. Per [[iterative-design]], finding problems early (through expert review and informal testing) is always cheaper than measuring them after launch. A/B testing is appropriate for fine-tuning decisions that depend on behavioral scale and cannot be predicted from observation alone: headline copy, CTA placement, pricing display, form field ordering.

See [[usability-evaluation-methods]] for the full treatment of formal usability studies, of which A/B testing is one specialized form.
