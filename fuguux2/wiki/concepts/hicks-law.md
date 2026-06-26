---
type: concept
title: "Hick's Law"
tags: [hci-law, decision-time, navigation, information-architecture]
related: [fitts-law, homepage-portal, grid-layout, wikipedia-2026-hicks-law, form-design]
sources: ["https://en.wikipedia.org/wiki/Hick%27s_law"]
created: 2026-06-24
updated: 2026-06-25
---

# Hick's Law

A foundational HCI law from psychologist William Edmund Hick's 1952 study ("On the rate of gain of information"), with related work by Ray Hyman in 1953 — sometimes called the **Hick–Hyman law**. It describes how decision time grows as the number of choices grows: more options take longer to choose among, but not in direct proportion. Doubling the number of choices does not double decision time; the relationship is logarithmic, so each additional option adds progressively less delay than the one before it.

## The relationship

For equally probable choices, reaction time (T) relates to the number of choices (n) as T = b·log₂(n+1), where *b* is an empirically fitted constant. The log₂ base reflects a binary-search-like process: people narrow down a large option set efficiently, the same way a search algorithm halves a sorted list at each step — *if* the set is organized in a way that supports that narrowing. Unequal-probability choices (some options picked far more often than others) need an adjusted, information-theoretic version of the formula.

## Design implications

- **Structure beats raw count.** A long alphabetized or categorized menu lets people subdivide it logarithmically (the same way they'd find a name in a phone book); an unstructured list of the same length forces linear, one-by-one scanning, where the logarithmic benefit disappears entirely — "Hick's law does not apply" to an unordered list, in the article's own words. The practical lesson is about organization, not just trimming options.
- **Progressive disclosure** — showing fewer choices at once, with a path to reveal more — reduces the immediate decision load even when the total option count doesn't shrink. [[homepage-portal]]'s 95%/5% rule (dedicating most above-the-fold space to the dominant audience's needs and pushing rarer needs to a subsidiary page) is a concrete instance of this, arrived at independently of this law in the book it comes from.
- **Search vs. browsing** trade off differently against this law: a well-organized navigation hierarchy benefits from the logarithmic curve, while an unstructured set of links does not — which is itself an argument for the kind of deliberate grouping [[grid-layout]] already recommends, even though that page doesn't name this law.

## Relationship to Fitts's Law

[[fitts-law|Fitts's Law]] and Hick's Law are often discussed together because both describe logarithmic relationships in human-computer interaction, but they govern different things: Fitts's Law is about *physically reaching* a target once you've picked it (movement time as a function of distance and size), while Hick's Law is about *deciding which one* to pick in the first place (decision time as a function of how many options there are, and how they're organized).

## Limitations

The law doesn't hold universally: verbal responses to highly familiar stimuli show little reaction-time increase regardless of choice count, and reflexive eye-movement (saccade) responses can show no relationship to choice count or even the opposite effect. Predictability within a sequence of repeated choices also doesn't follow the same curve. A frequently cited extension (E. Roth, 1964) found that the rate of information processing implied by an individual's Hick's-Law curve correlates with IQ, framing the law as a rough measure of cognitive processing capacity rather than only a UI design rule of thumb.

## Further reading

Victor Ponamariov's *50 Tips to Improve User Interface* (self-published ebook, no stated license — not ingested into this wiki; see `raw/copyrighted/50_ui_tips.pdf`) applies this law directly to option-selector choice: for five to seven or fewer options, replace a dropdown (whose choices are hidden until opened) with radio buttons, clickable card selectors, or tag-style toggles — all of which reveal choices immediately, reducing the decision cost this law describes. See also [[form-design]].

## Notes for the wiki

Created when the dedicated Wikipedia article gave the law enough independent substance — its own formula, its own design implications, and its own documented limitations distinct from Fitts's Law's — to warrant a page rather than staying folded into [[fitts-law]]'s "Related laws" section as a one-sentence, parenthetical mention.

Reclassified from `entity` to `concept` (2026-06-25) after `schema.md` was updated to classify laws as concepts rather than entities — a law is a relationship/framework, not a named thing.
