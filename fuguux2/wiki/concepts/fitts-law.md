---
type: concept
title: "Fitts's Law"
tags: [hci-law, motor-control, accessibility, human-factors]
related: [know-your-customers, accessibility, organized-search-results, action-buttons, wikipedia-2026-fittss-law, vanduyne-2006-knowing-your-customers, vanduyne-2006-glossary, hicks-law, form-design, loading-states]
sources: [vanDuyne_03_3PP_039-068.pdf, vanDuyne_Glos_3PP_867-896.pdf, "https://en.wikipedia.org/wiki/Fitts%27s_law"]
created: 2026-06-24
updated: 2026-06-25
---

# Fitts's Law

A foundational HCI law from psychologist Paul Fitts's 1954 study (*Journal of Experimental Psychology*), proposing a metric for how hard it is to select a target by pointing at it. In plain terms: the time needed to move to and select a target depends on how far away it is and how big it is — closer, bigger targets are faster to acquire; farther, smaller ones take measurably longer. This is the underlying principle behind several patterns already in this wiki that favor large, nearby clickable targets, such as [[organized-search-results]]'s large pagination links and [[accessibility]]'s motor-control discussion, even where those pages don't name the law explicitly.

## The relationship

Formally, movement time (MT) relates to distance (D, the gap between the starting position and the target's center) and target width (W, the target's size along the direction of movement) as MT = a + b·log₂(2D/W), where *a* and *b* are empirically fitted constants. The log₂(2D/W) term is called the **index of difficulty** — practically, what matters for design is just the shape of the relationship: difficulty rises with distance and falls with size, and it does so on a logarithmic curve, so the easy early gains (going from tiny to small) taper off faster than naive intuition suggests.

## Design implications

- **Make targets bigger, not just visible** — a target's *effective* size is what's clickable, not just what's visually drawn; padding a small icon's clickable area is a direct application (already covered, without naming the law, in [[organized-search-results]] and the [[accessibility]] motor-control discussion).
- **The rule of the infinite edges** — a target placed flush against a screen edge is effectively infinite in size along that edge, since the cursor can't overshoot past it. macOS's top-of-screen menu bar relies on exactly this.
- **"Magic corners"** — a screen corner is where two infinite edges meet, making it the single easiest target on the entire screen; Windows and Microsoft Office both place high-value controls (e.g. the Start button, the Office button) in corners for this reason.
- **Touchscreens raise the stakes** — a fingertip is far less precise than a mouse cursor, so the same target-size guidance matters even more on mobile, where targets also can't rely on hover states to compensate for imprecision.
- **Radial/pie menus** put every option at the same distance from the click point, minimizing the worst-case distance rather than just the average — though handedness still matters (right-handed users select items on their left less efficiently than the right).

## Related laws

- **[[hicks-law|Hick's Law]]** — a complementary law about decision time rather than movement time: choosing among more options takes longer, roughly logarithmically in the number of choices. Where Fitts's Law governs *getting to* a target, Hick's Law governs *deciding which one* to go to; see [[hicks-law]] for its own formula and design implications.
- **The (Accot–Zhai) steering law** — extends Fitts's Law from selecting a single point target to navigating through a constrained path (e.g. a hierarchical pull-down menu, where the cursor has to stay within a corridor the whole way, not just land on an endpoint).
- **Throughput** — a related metric combining a task's index of difficulty with the time it actually took, expressed in bits per second, used to compare pointing performance across input devices or populations.

## Limitations

The model's accuracy degrades when distance and width both vary across a wide range within the same comparison, and the original one-dimensional formulation needs adjustment for real two-dimensional pointing (a target isn't just "far" or "close," it has both a width and a height relative to the movement direction). Applying it to eye-tracking/gaze-based interaction is contested, since rapid involuntary eye movements (saccades) don't behave like the deliberate, correctable hand movements the law was modeled on.

## Further reading

Victor Ponamariov's *50 Tips to Improve User Interface* (self-published ebook, no stated license — not ingested into this wiki; see `raw/copyrighted/50_ui_tips.pdf`) names this law directly in two tips: expanding a button's clickable area via padding — extending the effective target size invisibly without changing the button's visible appearance — and replacing gallery-slider dot indicators with directly clickable image areas or navigation arrows, since dots have a far smaller effective target size than the surrounding image and fail badly on touch devices.

## Notes for the wiki

Created when the dedicated Wikipedia article, plus the earlier one-sentence mentions in [[know-your-customers]] (from Ch. 3) and the book's glossary, gave the law enough substance for its own page — reversing the earlier "stays inline" call from the Ch. 3/glossary ingestion sessions, which is being logged here rather than silently overwritten.

Reclassified from `entity` to `concept` (2026-06-25) after `schema.md` was updated to classify laws as concepts rather than entities — a law is a relationship/framework, not a named thing, and the page itself draws on multiple sources, which fits the concept pattern better than the entity one.
