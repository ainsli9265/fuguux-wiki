---
type: source
title: "Wikipedia: Web Colors"
tags: [color, accessibility, web-standards, color-models]
related: [color-theory, accessibility, wcag, wikipedia-2026-web-colors]
created: 2026-06-25
updated: 2026-06-25
authors: []
year: 2026
url: "https://en.wikipedia.org/wiki/Web_colors"
venue: Wikipedia
---

# Wikipedia: Web Colors

Wikipedia's article on web colors. Covers hex triplet notation, the 16 basic and ~140 extended HTML/CSS named colors (derived from X11), CSS color functional syntax (RGB, RGBA, HSL, HSLA, HWB), CSS Color Level 4/5 features (wider gamuts, OKLab, color-mix()), the 216-color web-safe palette (mid-1990s, now obsolete), and accessibility guidance on specifying both foreground/background colors and WCAG contrast ratios.

**License:** CC BY-SA 4.0 — https://creativecommons.org/licenses/by-sa/4.0/

**Raw file:** `raw/safe/wikipedia-web-colors.html`

**Media:** Five diagrams/tables (basic HTML colors, X11 color chart, SVG 1.1 named colors, 216-color web-safe table, 22-color "safest" table) — all on Wikimedia Commons; not downloaded, consistent with all Wikipedia ingestions.

## What was extracted

- Updated [[color-theory]]: added HSL as a designer-intuitive color model; added a new "Web color standards and historical constraints" section covering sRGB as the web baseline, web-safe colors as a now-obsolete 1990s constraint, and the dithering problem that motivated the 216-color palette.
- Updated [[accessibility]]: added the "specify both foreground and background colors" rule; added the specific WCAG contrast ratios (4.5:1 AA normal text, 3:1 AA large text, 7:1 AAA); added the dyslexia nuance (maximum AAA contrast is not universally optimal).

## What was excluded

- Hex triplet byte-level conversion math — code implementation.
- CSS color functional syntax (RGB(), HSL(), color-mix() etc.) — code implementation.
- CSS Color Level 4/5 wide-gamut color spaces (OKLab, OKLCH, Display P3, REC.2020) — color-science and CSS specification detail beyond practical design guidance; no UX concept page warranted (single source, highly technical, no direct design-decision implication documented in the article).
- Named color catalog (140+ names with hex/RGB values) — reference table, not a concept.
- RebeccaPurple memorial note — human-interest, not UX guidance.
- X11 / Mosaic / Netscape browser history — platform history, not UX design guidance.
- HWB color model — mentioned briefly, no design-application content beyond what HSL already covers.
- System colors (deprecated CSS feature) — deprecated implementation detail.
