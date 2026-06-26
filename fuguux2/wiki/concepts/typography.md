---
type: concept
title: Typography
tags: [typography, legibility, readability, typeface, visual-hierarchy, layout]
related: [clear-first-reads, color-theory, accessibility, gestalt-psychology, grid-layout, wikipedia-2026-typography, wikipedia-2026-web-typography]
sources: ["https://en.wikipedia.org/wiki/Typography", "https://en.wikipedia.org/wiki/Web_typography"]
created: 2026-06-25
updated: 2026-06-25
---

# Typography

Typography is the art and technique of arranging type to make written language **legible**, **readable**, and **appealing**. In UX practice it governs typeface selection, point size, line length, line spacing (leading), letter spacing (tracking), and kerning — choices that, made well, should be invisible to the reader and, made poorly, directly impede comprehension or discourage reading.

## Legibility vs. Readability

These are distinct but related concepts, often conflated:

**Legibility** is perception: how easily individual characters can be distinguished from one another. A font is legible when characters like *b* and *h*, or numerals *3* and *8*, remain distinguishable at small sizes; brush scripts and decorative faces are notorious for poor legibility. All-caps text reduces legibility because lowercase letterforms carry more variation than capitals. Walter Tracy's definition: "the quality of being decipherable and recognizable."

**Readability** is comprehension: the ease of reading a body of text as a whole, not just individual characters. Margins, word spacing, line spacing, line length, and structural clarity (headings, consistent hierarchy) all affect readability independently of how legible the chosen typeface is. A legible typeface can still become unreadable through poor setting. Sans-serif fonts, for example, are legible at small sizes but have lower readability for extended prose — the eye tires across long runs without serifs as anchors.

The Royal College of Art's Readability of Print Unit (Spencer, Coe, Reynolds) demonstrated that **saccadic rhythm** governs comfortable reading: the eye moves in discrete jumps, recognizing roughly three words per saccadic jump; lines requiring more than three-to-four jumps introduce strain and reading errors. This translates directly into line-length guidance — overly wide columns are harder to read not because of the font but because of the extra jumps required per line.

## Typeface Selection

Different content categories have accumulated typographic conventions; working against them requires deliberate justification. Practical defaults:

- **Long-form body text**: serif "text romans" or "book romans" — serifs aid horizontal tracking and differentiate letterforms in dense text
- **Newspapers and compact layouts**: tightly-fitted serif faces maximizing readability per column inch
- **Short introductory copy or incidental text**: sans-serif works at short lengths; breaks down for extended reading
- **Headlines**: larger display typefaces designed for contrast against body text; proportion and visual weight signal hierarchy before words are read

Late-twentieth-century convention pairs sans-serif headings with serif body text, using typeface category, weight, and size as the hierarchy signal.

Typeface selection is also a **tone signal** that precedes reading: the typeface chosen immediately cues the register of the content. Classical serifs with historical models suggest authority and permanence; geometric sans-serifs convey clean, contemporary neutrality; bold faces assert and attract attention. A 2020 study found subjects rated music "more pleasant" when CD covers featured round typefaces — even incidental typographic choices carry mood. Typographers must understand the text's context and intent before selecting faces, not after.

## Text Composition

Even distribution is the goal: a well-composed text block creates transparency — the reader attends to the content, not the container. Several variables interact:

- **Line length**: controls the number of saccadic jumps per line; three-to-four jumps is the comfortable upper bound
- **Leading (line spacing)**: generous vertical space helps the eye distinguish lines and return accurately; tightly packed lines cause doubling errors (re-reading the same line)
- **Justification**: full justification requires tight control of word spacing and hyphenation — standard software defaults rarely manage this well, leaving rivers of whitespace. Ragged-right setting is more reliable without expert intervention
- **Underlining**: disrupts descending letters (p, g, y, q) that differentiate letterforms, reducing legibility; prefer weight or italic for emphasis
- **Tracking and kerning**: overly tight or loose letter-spacing reduces readability; correct defaults assume normal reading distances and sizes

"Color" in typographic usage — distinct from [[color-theory]] — refers to the overall ink density of a text block, determined primarily by typeface weight but also by word spacing, leading, and margin depth. A dense block feels heavy; loose spacing feels airy. This interplays with white space and hierarchy to create tone that precedes reading.

## Display vs. Text Typography

Display typography (advertisements, headlines, signs, posters, packaging, logos, motion graphics) prioritizes visual impact and can trade some readability for attraction. At larger sizes, letterform details are magnified and small legibility imperfections become prominent; color and size carry more communicative weight than text design does at the word level.

Overusing display techniques in body context — bold colors, multiple competing typefaces, heavily decorated backgrounds — creates visual noise that prevents the message from being received. The guiding rule: every typographic variable (typeface change, size change, color, decoration) must serve the hierarchy rather than add to it. [[clear-first-reads]] relies on exactly this principle — font is one of four levers (alongside color, size, and position) for establishing a single dominant visual element; adding a second competing typeface without clear reason undermines the first read.

## Typography in Digital Contexts

Digital character encoding separates text presentation from content meaning, allowing identical text to reflow with context-appropriate typefaces across devices. Screen rendering constraints (anti-aliasing, pixel density, dark mode, operating-system font rendering) introduce variables that print does not face. The core principles — legibility, readability, appropriate tone, structural hierarchy — hold across media; the specific defaults adapt. WCAG luminance-contrast requirements (see [[accessibility]]) add a minimum measurable bar for typographic color contrast that print typography historically relied on judgment for.

## Web Typography and Font Stacks

Web typography adds a practical constraint to the principles above: unlike print, a designer cannot guarantee which typefaces are installed on a reader's system. Managing this gracefully requires understanding the browser's font-resolution chain.

**Web-safe fonts** are typefaces reliably present on the vast majority of operating systems, making them safe to specify without a fallback. The core set was largely established by Microsoft's "Core Fonts for the Web" initiative (1996–2002), which distributed Arial, Georgia, Verdana, Times New Roman, Courier New, and several others under a freely-distributable license — these faces became the de facto fonts of the early web and remain ubiquitous today.

**Font stacks and the fallback mechanism**: the CSS `font-family` property accepts a comma-separated priority list. The browser tries each name in order, moving to the next if the font is not available, and ultimately falls back to its own default. A well-designed stack provides typographically similar alternatives at each step, ensuring the design intent is approximated even when the preferred face is absent. Every stack should end with one of the five **generic font families** — the last-resort fallback categories that guarantee at least the correct broad character:

- **sans-serif** — no decorative strokes; generally cleaner for screen reading at small sizes
- **serif** — decorative strokes; traditional association with print body text
- **monospace** — all characters equal-width; standard for code display
- **cursive** — script-like; legibility degrades quickly at small sizes
- **fantasy** — decorative/symbolic; unsuitable for body text

**Web fonts**: CSS `@font-face` allows loading custom typefaces from a server, giving designers typographic freedom equivalent to print — any typeface, not just those pre-installed on the viewer's system. Freely-licensed libraries (Google Fonts, launched 2010, reaching 800+ families by 2016) have made this accessible at no cost, and by 2016 the majority of websites used web fonts. The trade-off is performance: each web font is an additional network request and file download, adding to page load time and potentially introducing a brief delay where a fallback font renders before the intended face arrives. A well-matched fallback stack reduces the visual disruption during that interval.

**Image replacement (anti-pattern)**: before web fonts were practical, designers sometimes substituted images rendered in the desired typeface for the actual text. This resolved the font-availability problem but introduced serious costs: the text becomes unselectable by users, invisible to screen readers and assistive technology, excluded from search-engine indexing, and adds unnecessary download weight. Web fonts have made image replacement of body text or headings an obsolete workaround; if typographic control is the goal, a web font with a good fallback stack is the appropriate tool.

## Further reading

Victor Ponamariov's *50 Tips to Improve User Interface* (self-published ebook, no stated license — not ingested into this wiki; see `raw/copyrighted/50_ui_tips.pdf`) adds three concrete applications of principles in this page: specific line-height multipliers (approximately 1–1.4× for headlines, 1.3–1.6× for body text) as actionable defaults for the leading guidance above; the headline proximity rule — a headline should be physically closer to the body copy it introduces than to the element above it, applying [[gestalt-psychology|Gestalt proximity]] to text layout; and the full-width text container problem — stretching a text block to the full browser width forces a Z-pattern scan instead of the left-to-right saccadic rhythm discussed in the Text Composition section.

Matthew Butterick's *Typography in Ten Minutes* (practicaltypography.com — commercial publication, no open license; see `raw/copyrighted/butterick-typography-in-ten-minutes.pdf`) gives specific numeric targets for the four variables most responsible for body-text quality. Point size: 10–12pt in print, 15–25px on the web (with the caveat that apparent size varies across typefaces, so adjustment per face is necessary). Line spacing: 120–145% of point size — expressed as a unitless CSS `line-height` value of 1.2–1.45; Butterick flags that single-line spacing is typically too tight and 1.5-line too loose. (The 50_ui_tips range of 1.3–1.6× for body text and Butterick's 1.2–1.45× are not perfectly aligned; both sit within a broadly accepted 120–160% comfort band, and the right value within that band depends on the specific typeface and point size.) Line length: 45–90 characters per line, equivalently 2–3 lowercase alphabets wide — in web contexts, this means preventing the text block from stretching to the browser-window edge. On font choice: Butterick recommends against Times New Roman and Arial for body text, and suggests purchasing a professional typeface when budget allows over relying on free web fonts — a position that should be read alongside the Web Typography and Font Stacks section above, where well-chosen web fonts are presented as a legitimate and common alternative.
