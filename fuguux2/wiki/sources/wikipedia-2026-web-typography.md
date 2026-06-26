---
type: source
title: "Wikipedia: Web Typography"
tags: [typography, web-fonts, font-stacks, web-design]
related: [typography, accessibility, wikipedia-2026-typography]
created: 2026-06-25
updated: 2026-06-25
authors: []
year: 2026
url: "https://en.wikipedia.org/wiki/Web_typography"
venue: Wikipedia
---

# Wikipedia: Web Typography

Wikipedia's article on web typography. Covers CSS font properties, web-safe fonts, Microsoft's Core Fonts for the Web (1996–2002), the CSS font-family fallback mechanism, the five generic font families, web font history (@font-face in CSS2, EOT, WOFF, Google Fonts 2010), Unicode fonts, and pre-web-font alternatives (image replacement, Flash/sIFR, JavaScript VML/SVG).

**License:** CC BY-SA 4.0 — https://creativecommons.org/licenses/by-sa/4.0/

**Raw file:** `raw/safe/wikipedia-web-typography.html`

**Media:** Two images (Web fonts.svg diagram; "3 Core Fonts for the Web.png" showing Arial, Georgia, Verdana) — both on Wikimedia Commons; not downloaded, consistent with all Wikipedia ingestions.

## What was extracted

- Updated [[typography]]: added a new "## Web Typography and Font Stacks" section covering web-safe fonts and the Core Fonts for the Web historical context; the fallback font stack mechanism and its design implications; the five generic font families as last-resort fallbacks; web fonts (@font-face, Google Fonts) as a source of full typographic freedom at a performance cost; and image replacement as a named anti-pattern with its specific failure modes (inaccessible, unselectable, SEO-damaging, bandwidth-heavy).

## What was excluded

- CSS font-property syntax (font-family, @font-face, etc.) — code implementation.
- Font file format specifications (EOT, WOFF, TrueType, OpenType, SVG fonts) — format/encoding detail, no design-decision guidance.
- Browser compatibility version lists — implementation detail.
- CSS Fonts Working Draft 4 `ui-*` tags — draft spec with limited support, no current design guidance.
- Unicode code-point limits (65,535 glyph cap in TrueType) — encoding detail, not design guidance.
- TrueDoc / Bitstream history — deprecated technology history.
- Flash/sIFR and JavaScript VML/SVG text techniques — now-obsolete workarounds; image replacement is the only one worth naming in the wiki as a cautionary pattern, since it still appears in discussions of typographic control.
- Håkon Wium Lie — individual credited with web font format advocacy; single source, author/advocate role, out of scope per purpose.md.
- Microsoft as a new entity — appears here for Core Fonts initiative and IE, but first appearance in the wiki; no dedicated entity page until second source.
