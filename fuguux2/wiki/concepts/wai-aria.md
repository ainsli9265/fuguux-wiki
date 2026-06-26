---
type: concept
title: WAI-ARIA (Accessible Rich Internet Applications)
tags: [accessibility, wcag, standards, assistive-technology]
related: [wai, accessibility, wcag, wikipedia-2026-wai-aria]
sources: ["https://en.wikipedia.org/wiki/WAI-ARIA"]
created: 2026-06-24
updated: 2026-06-24
---

# WAI-ARIA (Accessible Rich Internet Applications)

One of [[wai|WAI]]'s five specification families, alongside [[wcag]]. Where WCAG covers content generally, WAI-ARIA specifically addresses **rich Internet applications** — custom, JavaScript-driven controls (custom dropdowns, tabs, live-updating regions) and partial-page content updates that plain HTML has no vocabulary to describe. A screen reader can announce a native `<button>` correctly because HTML already says what it is; it can't do the same for a `<div>` that JavaScript has turned into a tab control, because nothing in the markup says "this is a tab, and it's currently selected."

## What it adds

WAI-ARIA lets a page declare extra metadata on top of existing markup, organized into three kinds:

- **Roles** — what a component *is* (e.g. marking a list of links as a navigation region, or a custom widget as a tab).
- **Properties** — relatively stable characteristics of a component.
- **States** — its current, changeable condition (e.g. whether a menu is expanded or collapsed right now).

This metadata feeds the **accessibility tree** — the structured representation of a page that assistive technology actually reads, separate from (but built from) the visual DOM — letting a screen reader or other tool present a dynamic custom widget as meaningfully as it would a native one.

## The first rule: prefer native HTML

WAI-ARIA's own guidance is explicit that it's a fallback, not a first choice — codified as the **Five Rules of ARIA**:

1. Don't use ARIA if the same semantics are achievable with a native HTML element or attribute.
2. Don't change the semantics of native HTML, unless there's no real alternative.
3. Every interactive ARIA control must be usable with the keyboard alone.
4. Don't remove semantics or hide focusable elements (e.g. applying `role="presentation"` or `aria-hidden="true"` to something a keyboard user can still tab to).
5. Every interactive element needs an accessible name.

The consensus reason for rule 1 specifically: incorrect or contradictory ARIA actively misleads assistive technology in a way that absent ARIA doesn't — "bad ARIA" is worse than "no ARIA." This is the same design discipline [[accessibility]] already argues for with color and clickable targets: prefer the option that can't be gotten subtly wrong over a more powerful one that can.

## Version history

WAI-ARIA work began in 2006 (first published September 26, 2006); WAI-ARIA 1.0 reached W3C Recommendation status March 20, 2014; 1.1 followed December 14, 2017; 1.2 reached Recommendation status June 6, 2023.

## Notes for the wiki

A local snapshot is saved at `raw/safe/wikipedia-wai-aria.html` alongside the live URL. Licensed CC BY-SA 4.0, consistent with this wiki's other Wikipedia sources — content here is paraphrased, not quoted. Kept this page at the design-principle level (why custom widgets need this, the roles/states/properties model, the five-rules hierarchy) and deliberately left out attribute-syntax detail (specific `aria-*` attribute names and values beyond the two used as rule examples above) as "specific code implementation" per `purpose.md`'s scope — the same line drawn for Pattern Group L's image/HTML implementation detail.
