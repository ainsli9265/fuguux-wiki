---
type: source
title: "Hick's Law (Wikipedia)"
tags: [hci-law, decision-time, navigation, information-architecture]
related: [hicks-law, fitts-law]
created: 2026-06-24
updated: 2026-06-24
authors: [Wikipedia contributors]
year: 2026
url: "https://en.wikipedia.org/wiki/Hick%27s_law"
venue: "Wikipedia"
---

# Hick's Law (Wikipedia)

A dedicated encyclopedia article on Hick's Law — previously only a one-sentence mention on [[fitts-law]] ("Related laws"), now substantial enough to justify its own concept page, [[hicks-law]]. Wikipedia articles are continuously edited, so `year` above reflects the access date (2026-06-24), not a fixed publication year.

## Key points

- William Edmund Hick published the original 1952 study; Ray Hyman's 1953 work is closely related, so the law is sometimes called the Hick–Hyman law.
- Decision time grows logarithmically with the number of choices: T = b·log₂(n+1) for equally-probable choices. Doubling the options does not double the time.
- The logarithmic benefit depends on the choice set being *organized* — an alphabetized or categorized menu lets people subdivide it efficiently; an unstructured list of the same length forces linear scanning, and the article states plainly that the law "does not apply" in that case.
- Documented limitations: doesn't hold for verbal responses to very familiar stimuli, can show no effect or a reversed effect for reflexive eye-movement (saccade) responses, and unequal-probability choice sets need an information-theoretic (entropy-based) adjustment to the formula.
- E. Roth (1964) found a correlation between an individual's Hick's-Law processing-speed slope and IQ.

## Notes for the wiki

A local snapshot is saved at `raw/safe/wikipedia-hicks-law.html` alongside the live URL. Licensed CC BY-SA 4.0, same treatment as this wiki's other Wikipedia sources — content folded in is paraphrased, not quoted.

**What was left out, and why** (per `schema.md`'s ingestion-report requirement): the entropy-based formula for unequal-probability choice sets is named but not derived in [[hicks-law]] — the derivation is more information theory than UX design. Nothing was excluded for being outside `purpose.md`'s scope outright; like [[wikipedia-2026-fittss-law]], this entire article is a design-relevant heuristic.

Linked the new page from [[homepage-portal]] (the 95%/5% above-the-fold rule is a concrete instance of progressive disclosure reducing decision load) and from [[fitts-law]] (upgraded the existing one-line "related law" mention to a full cross-reference now that both have their own pages).

Reclassified [[hicks-law]] from `entity` to `concept` (2026-06-25) after `schema.md` was updated to classify laws as concepts rather than entities.
