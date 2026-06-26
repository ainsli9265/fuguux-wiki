---
type: concept
title: Loading States
tags: [feedback, ux-patterns, performance, progressive-disclosure]
related: [interface-design-principles, affordance, action-buttons, visual-hierarchy, form-design]
created: 2026-06-25
updated: 2026-06-25
---

# Loading States

Every delay between a user action and a system response is an opportunity to lose trust or cause confusion. Loading states bridge that gap: they signal that something is happening, set expectations about what is coming, and minimize disruption when content arrives.

## Empty states

An empty state is the version of a page or component when there is no content to show — a new user's dashboard, a fresh project, an empty search result. An empty state that offers no explanation or path forward reads as a broken or abandoned page. Effective empty states explain why nothing is there and give the user a clear action to take.

## Skeleton screens vs. spinners

**Skeleton screens** show the layout structure that will be occupied by incoming content, rendered as neutral placeholder blocks. They communicate not just "loading" but "content of approximately this shape is coming," and they prevent layout shift — the disorienting reflow that occurs when a page reorganizes itself around content that arrives after the initial render. Skeletons are appropriate for large content blocks where layout shift would be most disruptive.

**Spinners** signal activity without making any spatial promise about what's coming. They suit smaller, contained loads — confirming a button action, an inline data refresh — where there's no layout to preview. A static text message is simpler still but can become indistinguishable from a stalled page; an animated indicator at least proves the browser is still responsive. See [[interface-design-principles]] (principle 2) for the general tradeoff between what a loader can credibly promise and what it commits to.

## Button loading states

When a button triggers an action that takes time to complete, the button can switch to a loading indicator to prevent double-submission and confirm the action was received. Keeping the button's dimensions stable during the loading state — so the surrounding layout doesn't shift — is part of the same layout-stability goal that makes skeleton screens valuable for larger content.

## Timing and long operations

Not every action needs a loader: for very fast responses, showing one at all can create a brief visual flash that reads as a glitch. For genuinely long operations, a loader that never updates its state eventually reads as frozen, regardless of what it actually shows. Updating a loader's message or appearance during a long wait reassures users that the system is still working.

## Further reading

Victor Ponamariov's *50 Tips to Improve User Interface* (self-published ebook, no stated license — not ingested into this wiki; see `raw/copyrighted/50_ui_tips.pdf`) covers the full cluster with specifics not captured above: an informative message plus a clear CTA for empty states (rather than a blank or minimal screen); the layout-shift rationale for choosing skeletons over spinners for large content blocks; a specific button-loading technique — setting the button text to transparent (not removed) so the button holds its exact original width while a spinner occupies the same space; delaying the loader's appearance by approximately 0.5–1 second so fast responses complete before the indicator ever shows; and updating the loader's message text after 5–10 seconds to reassure users that the system hasn't stalled.
