---
type: concept
title: Action Buttons
tags: [affordance, visual-design, navigation, design-pattern]
related: [web-design-patterns, process-funnel, ebay, amazon, vanduyne-2006-web-design-patterns, fitts-law, affordance, form-design, loading-states]
sources: [vanDuyne_02_3PP_019-038.pdf]
created: 2026-06-23
updated: 2026-06-25
---

# Action Buttons

**Problem:** customers can't tell what is and isn't clickable on a page.

**Solution:** give an otherwise flat button a shaded, three-dimensional appearance. This works as a perceivable [[affordance]] because it borrows two sources of prior knowledge: familiarity with physical three-dimensional buttons (keyboards, remote controls), and the learned behavior, from graphical user interfaces generally, that raised-looking elements can be pressed with a mouse. Both [[ebay]] and [[amazon]] use this technique for key calls to action on their homepages (e.g., eBay's "Register Now," Amazon's "Find Gifts").

There are two implementations: **HTML buttons**, rendered by the browser with limited control over appearance, and **graphical buttons**, implemented as one or more images, which give full design control at the cost of slower downloads.

**Forces:** larger buttons are easier to see and click (per [[fitts-law]]) but consume more page space; an image-based button may warrant a redundant text link for the same destination; image-heavy buttons slow page load.

Action buttons help complete a [[process-funnel]] by giving each step of a multi-step task a clear, unambiguous call to action. This pattern is also the worked example used to introduce the six-part pattern format in [[web-design-patterns]].

## Further reading

Victor Ponamariov's *50 Tips to Improve User Interface* (self-published ebook, no stated license — not ingested into this wiki; see `raw/copyrighted/50_ui_tips.pdf`) adds one concrete constraint: only one primary (high-emphasis) button should appear per form or view. Multiple competing primary buttons undermine the visual hierarchy that makes any single call to action findable — addressed in full in [[form-design]].
