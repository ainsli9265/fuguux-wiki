# Research Log

## 2026-06-26 (48)

- Wikipedia "Progressive disclosure" → `raw/safe/wikipedia-progressive-disclosure.html` (CC BY-SA 4.0), source page [[wikipedia-2026-progressive-disclosure]]. Short article (stub-length). No new concept page created — [[progressive-disclosure]] was written this session during the lint pass; updated it with this source's additions.
- Updated [[progressive-disclosure]]: (1) refined opening definition — added "when it becomes relevant to the task at hand" (task-relevance framing, more precise than "on demand" alone); (2) added the macOS print dialog as the canonical concrete example (default collapsed view → "Show Details" expands advanced options); (3) added the theme park queue analogy to the Rationale section as a physical-world illustration of the same metered-exposure logic. Fixed pre-existing `related:` duplicate (hicks-law appeared twice — removed duplicate). Added Wikipedia URL to `sources:` and `wikipedia-2026-progressive-disclosure` to `related:`.
- Excluded: Kristina Hooper Woolsey (Apple Human Interface Group, 1985 quote — individual, out of scope per `purpose.md`); UXPin article (commercial tool vendor, no design substance); Donald Norman's *User Centered System Design* (1986) — cited in the Wikipedia references but the article adds no content from it beyond a bare citation; "Disclosure widget" and "Chunking (writing)" see-also links (no content, one-line cross-references only).

## 2026-06-26 (47)

- Lint pass (61 files). Found and fixed: 1 orphan, 2 stale prose claims, 6 missing cross-references, 3 missing concept pages.
- **Orphan fixed**: [[barnes-and-noble]] had no inbound body links — added `[[barnes-and-noble]]` reference and `related:` entry to [[shopping-cart]] wish list section.
- **Stale prose fixed**: [[vanduyne-2006-advanced-e-commerce]] called Group F "not yet ingested" in two places — updated first paragraph to link `[[vanduyne-2006-basic-e-commerce]]`, updated excluded-patterns list to remove F and note it has been ingested with links to the four new concept pages. [[multiple-destinations]] called Group F "not yet ingested" — replaced parenthetical with `[[quick-flow-checkout]]` link. Added `vanduyne-2006-basic-e-commerce` and `barnes-and-noble` to `vanduyne-2006-advanced-e-commerce` `related:`.
- **Cross-references fixed**: [[featured-products]] — added forward links to `[[clean-product-details]]` and `[[shopping-cart]]` in body and `related:`; [[cross-selling-and-up-selling]] — added `[[clean-product-details]]`, `[[shopping-cart]]`, `[[quick-flow-checkout]]` in body and `related:`; [[order-tracking-and-history]] — added `[[easy-returns]]` in body and `related:`; [[clean-product-details]] — added `[[above-the-fold]]` wikilinks in intro paragraph and section lead; [[quick-flow-checkout]] — added `[[above-the-fold]]` in order-summary step and `above-the-fold` to `related:`; [[multiple-destinations]] — added `quick-flow-checkout` to `related:`.
- **New concept pages**: [[progressive-disclosure]] — deferring additional information on demand to reduce decision load; cites Hick's Law as the formal rationale; applications: menus, above-the-fold/below-the-fold structure, multi-step funnels, show-more patterns, progressive loading; covers limits (findability tradeoff, expert-user friction). [[page-template]] — reusable structural layout per page type holding nav/content regions in predictable positions; common template classes (homepage, category, detail, search, checkout); relationship to six Group I layout patterns; ties to web-site-development-process Refinement and Production phases; note that Pattern D1 will expand this when ingested. [[ab-testing]] — controlled live experiment comparing two versions differing by one variable; statistical significance requirement; multivariate variant; distinction from qualitative usability testing (which vs. why); placement late in design lifecycle; disambiguates "virtual testing" (van Duyne term) from the standard A/B/split-testing label.
- Excluded from new pages: specific software tools for running A/B tests (implementation); progressive-disclosure history/origin attribution (too thin); page-template HTML/CSS specifics (implementation).

## 2026-06-25 (46)

- `raw/safe/vanDuyne_F_3PP_431-490.pdf` (Pattern Group F, Basic E-Commerce). Created [[vanduyne-2006-basic-e-commerce]]. Created four concept pages: [[quick-flow-checkout]] (F1 + checkout steps F4–F8 detailed), [[clean-product-details]] (F2), [[shopping-cart]] (F3), [[easy-returns]] (F9). Created entity [[barnes-and-noble]] — now at 2+ sources (Group G + Group F for wish list pattern). Updated [[amazon]]: added Pattern Group F examples (product page hiding Add to Cart on out-of-stock items, shopping cart cross-selling, checkout guest path and address book, return process with trackable label). Updated [[process-funnel]]: added cross-reference to [[quick-flow-checkout]] as the full elaboration; added Group F to `sources:`. Updated [[trust-and-credibility]]: added opening paragraph on payment security signals (privacy policy link, HTTPS lock at payment entry) and return policy as a purchase-time trust signal; added Group F to `related:` and `sources:`.
- Extracted into concept bodies (F1): distraction elimination during checkout; deal-breaker questions upfront (shipping/returns/stock/tax/gift wrap); guest checkout path; trust signals at each step; four-step structure (account ID → shipping → order summary + payment → confirmation); account-creation deferral. (F2): above-fold element set (nav, thumbnail, needs-oriented description, price, options pick list, ratings, delivery estimate, Add to Cart); below-fold element set (full description, reviews, related products, comparator); standardized per-category template; customer-oriented vs. company-oriented description ordering. (F3): persistent access via header cart indicator; guest browsing before account; Add to Cart clarity and confirmation; cart item details (name, description, availability, price, quantity, remove); shipping estimate; cart persistence; wish lists as separate holding area; cross-sell as secondary; localized terminology. (F4–F8 in quick-flow-checkout body): address book for returning customers; single-column form, right-aligned labels, minimal fields, "Use This Address" pattern; shipping method radio/list with simultaneous cost+time display, live update; payment security signals, stored cards by last 4, promo code at payment step; order summary with all-information + per-section editing, "Place Order" above and below fold, "not yet placed" clarity; confirmation with order number, email, printable, post-completion cross-sell. (F9): return policy on every product/checkout/category/homepage page; four-step return funnel (find order → select items → reason → print label); trackable label; credit speed as repeat-purchase driver.
- Excluded: specific checkout abandonment rate statistics (numeric thresholds from source); "cart" vs. "basket" vs. "bag" specific percentages from 2002 study (dated numeric data); screenshots and site-specific layout descriptions (illustration only); particular implementation details for cookie-based guest account persistence (code implementation); international shipping forms details for F5 (implementation); specific credit card API fields in F6 (implementation). Entity threshold not met: Nordstrom (appears in F4/F5/F7, single source — below threshold), Snapfish (appears in F4/F7/F8, single source — below threshold), Half.com (appears in F1/F4/F6, single source — below threshold), Room & Board (single mention, F2), Netflix (single mention, F2), babyGap (single mention, F5), Buy.com (single mention, F9), United Airlines (single mention, F1), Cooking.com (single mention, F2). Barnes & Noble now at 2 sources (Group F + Group G both cite wish list implementation) — entity page created.

## 2026-06-25 (45)

- Triage: Bargas-Avila et al. (2010), *Simple but Crucial User Interfaces in the World Wide Web: Introducing 20 Guidelines for Usable Web Form Design* (InTech, ISBN 978-953-307-084-1) → **copyrighted** (user decision). License is CC BY-NC-SA 3.0 — an explicit stated license permitting non-commercial use, but user elected to treat the NC/SA restrictions as placing it in the copyrighted bucket. Moved to `raw/copyrighted/bargas-avila-2010-web-form-design.pdf`. No source page created; not added to any page's `sources:` frontmatter.
- Updated [[form-design]] `## Further reading`: added Bargas-Avila et al. pointer covering six areas the body does not address — (1) label positioning: Penzo eye-tracking finding that top-aligned labels are fastest (one fixation), left-aligned is usable when deliberate consideration is desired; (2) required field marking: color outperforms asterisk alone empirically; full visual separation fastest of all; (3) input type selection: checkboxes > list boxes for multi-select; ≤4-option threshold for radio buttons vs. dropdowns; (4) format restriction communication: stating the rule without an example reduces errors most efficiently; (5) inline validation timing: real-time inline errors counter-intuitively increase consecutive errors vs. post-submit embedded errors; (6) post-submission behavior: never clear completed fields on error, disable submit immediately, show confirmation page and email, avoid reset buttons.
- Nothing added to [[form-design]] body: all substantive content was encountered through this copyrighted source. Self-check confirmed that even points independently attributable to Nielsen (never clear fields, disable submit) were noted here specifically because the paper included them — consistent with the schema's strict "did I learn it from this source" test.
- Excluded entirely (not even Further reading): input ordering by familiarity (general UX principle already implied by existing pages); date-entry field formatting specifics (implementation detail); single-column layout guideline (common UX knowledge but not adding substance beyond what's in body/existing FR); polite/apologetic error message tone (one sentence, below concept threshold given existing [[interface-design-principles]] and [[form-design]] coverage).

## 2026-06-25 (44)

- Triage: Apple Human Interface Guidelines — Color (developer.apple.com/design/human-interface-guidelines/color) → **copyrighted**. Apple Inc. copyright; no open license stated. Moved to `raw/copyrighted/apple-color-hig.pdf`. No source page created; not added to any page's `sources:` frontmatter.
- Updated [[color-theory]] body: added new section "Color consistency in interface design" — using the same color for two different semantic roles within an interface dissolves both signals; once a color carries a role, that role must be held stable. Sourced from common knowledge / [[interface-design-principles]] consistency principle; Apple HIG provided the prompt but the body does not reproduce Apple's framing.
- Updated [[visual-hierarchy]] body: added sentence to the Color paragraph noting that color's hierarchy power is self-depleting per Von Restorff — applying it to every element simultaneously neutralizes its contrast signal. Derived from Von Restorff effect already on the page; independently sourceable.
- Added `## Further reading` to [[color-theory]] pointing to `raw/copyrighted/apple-color-hig.pdf`, covering six Apple-specific points that cannot appear in page bodies: (1) consistent color semantics with interactive/non-interactive example; (2) three-context design requirement — light, dark, and increased contrast variants for every custom color; (3) environmental lighting effects on perceived color (bright/sunny darkens and mutes, dim/dark brightens and saturates); (4) sparing application for emphasis — reserve color for status indicators and primary actions; monochromatic controls preferred over colorful backgrounds; (5) Stocks app red/green locale reversal as concrete worked example of culture-bound color symbolism; (6) Display P3 at 16 bits per channel for wide-color-display authoring.
- Excluded from body: three-context (light/dark/high-contrast) design requirement — Apple-specific framing and the specific "provide all three variants" prescription came from this source; body only states the general consistent-use principle. Environmental lighting test guidance — too platform-specific (True Tone, tvOS TVs) to generalize cleanly into body. Display P3 / wide color specifics — extends color-theory.md's sRGB note but the 16-bit/PNG/P3 prescriptions are Apple implementation detail. Liquid Glass color — Apple-proprietary UI material, entirely out of scope. Hard-coding system color values / dynamic semantic colors / UIWhitePointAdaptivityStyle — implementation/API detail, out of scope.

## 2026-06-25 (43)

- Triage: *Typography in Ten Minutes* (Matthew Butterick, practicaltypography.com) → **copyrighted**. Site states the book is supported by reader payment; no open license declared. Moved to `raw/copyrighted/butterick-typography-in-ten-minutes.pdf`. No source page created; not added to any page's `sources:` frontmatter.
- Updated [[typography]] `## Further reading`: added Butterick pointer with four specific numeric targets the body cannot reproduce — point size (10–12pt print, 15–25px web), line spacing (120–145%, equivalently CSS `line-height` 1.2–1.45), line length (45–90 characters / 2–3 lowercase alphabets), and font-choice opinion (avoid Times New Roman and Arial; buy professional typeface where possible). Also noted the partial tension between Butterick's line-spacing range and the 50_ui_tips range already in Further reading (both within a broadly accepted 120–160% band).
- Nothing excluded from body that could have gone there: all substantive content is numeric thresholds Butterick introduced, which the schema flags for Further reading regardless of independent derivability. The "body text quality determines document quality" framing is Butterick's voice rather than a new concept; principle already implicit in [[typography]]'s existing treatment.

## 2026-06-25 (42)

- Wikipedia "Web typography" → `raw/safe/wikipedia-web-typography.html` (CC BY-SA 4.0), source page [[wikipedia-2026-web-typography]]. No new concept pages; all new content folded into [[typography]].
- Updated [[typography]]: added new section "Web Typography and Font Stacks" — web-safe fonts and the Core Fonts for the Web historical context (Microsoft, 1996–2002, established Arial/Georgia/Verdana/etc. as de facto web fonts); font stack fallback mechanism (comma-separated priority list, browser tries each in order); five generic font families as last-resort fallbacks (sans-serif, serif, monospace, cursive, fantasy) with brief characterizations; web fonts (@font-face / Google Fonts launched 2010, 800+ families, majority of sites by 2016) as the mechanism for full typographic freedom at a performance cost; image replacement named as an anti-pattern (unselectable, inaccessible, SEO-damaging, bandwidth-heavy) now obsolete due to web fonts.
- Excluded: CSS font-property and @font-face syntax (code implementation); font file formats EOT/WOFF/TrueType/OpenType/SVG (format/encoding detail); browser version compatibility lists (implementation detail); CSS Fonts WD4 `ui-*` tags (draft, no current design guidance); Unicode glyph-count limits (encoding detail); TrueDoc/Bitstream and sIFR/Flash/VML JavaScript techniques (deprecated workarounds — image replacement is the only one worth naming as a cautionary pattern since it still recurs); Håkon Wium Lie (individual, author/advocate, single source, out of scope per purpose.md); Microsoft as new entity (first appearance in wiki — no page until second source).
- Media: two Wikimedia Commons images (web fonts SVG diagram; Core Fonts PNG showing Arial/Georgia/Verdana) — not downloaded, consistent with all Wikipedia ingestions; no `raw/media/` subfolder.

## 2026-06-25 (41)

- Wikipedia "Web colors" → `raw/safe/wikipedia-web-colors.html` (CC BY-SA 4.0), source page [[wikipedia-2026-web-colors]]. No new concept pages; all new content folded into existing pages.
- Updated [[color-theory]]: expanded "Color models" section to add HSL (hue/saturation/lightness) as a designer-intuitive screen color model, distinct from RGB and mapped to the same sRGB gamut; added new section "Web color standards and historical constraints" — sRGB as the web baseline color space (the gamut against which WCAG contrast ratios are calculated), and web-safe colors as a now-obsolete mid-1990s design constraint (216-color 6³ palette to avoid dithering on 256-color displays, superseded by TrueColor in the early 2000s).
- Updated [[accessibility]]: added two new concrete color rules — (1) always specify *both* foreground and background colors explicitly to avoid browser-theme combination failures; (2) WCAG 1.4.3 contrast ratios stated explicitly for the first time in the wiki: 4.5:1 AA normal text, 3:1 AA large text, 7:1 AAA — plus the dyslexia nuance that AAA maximum contrast is not universally optimal.
- Excluded: hex triplet byte-level conversion math (code implementation); CSS color functional syntax (code implementation); CSS Color Level 4/5 wide-gamut spaces and color-mix() (color science/CSS spec, no design-decision guidance in the article beyond noting they exist); named color catalog 140+ entries (reference table); RebeccaPurple memorial (human interest); X11/Mosaic/Netscape browser history (platform history); HWB color model (one-sentence mention, no design guidance beyond what HSL covers); system colors (deprecated CSS feature).
- Media: five color diagrams and tables (basic HTML colors, X11 chart, SVG 1.1 named colors, 216-color web-safe table, 22-color "safest" table) — all on Wikimedia Commons; not downloaded, consistent with all Wikipedia ingestions; no `raw/media/` subfolder.

## 2026-06-25 (40)

- Wikipedia "Responsive web design" → `raw/safe/wikipedia-responsive-web-design.html` (CC BY-SA 4.0), source page [[wikipedia-2026-responsive-web-design]].
- Created [[responsive-web-design]]: definition ("content is like water"); three UX-level pillars — fluid proportion-based grids, flexible images, breakpoint-driven layout shifts; UI plasticity as the governing principle; device-diversity rationale (mobile became majority of traffic ~2013); relationship to [[expanding-and-fixed-screen-width]] and [[grid-layout]]; complementary role of [[mobile-first-design]]; testing implication (validate across viewport sizes). Term coined May 2010 in *A List Apart*.
- Created [[mobile-first-design]]: constraint-driven sequencing strategy — design for the smallest device first to force prioritization; progressively enhance for larger screens; contrasted with desktop-first compression; complementary role alongside RWD; accessibility overlap (simpler nav, larger targets, lower cognitive load).
- Updated [[expanding-and-fixed-screen-width]]: added closing paragraph noting RWD as the generalizing framework that subsumes the fixed-vs.-expanding binary; added `responsive-web-design` to `related:`.
- Excluded from any page: CSS3 media query syntax (code implementation); RESS server-side implementation (code implementation); Mobilegeddon search-ranking algorithm (SEO, not UX design); named individuals Ethan Marcotte, Cameron Adams, Luke Wroblewski (authors, single source, below entity threshold, and authors are out of scope per `purpose.md`); Audi.com, Razorfish (incidental mentions, single source, below entity threshold); browser devtool specifics and Adobe Edge Inspect (implementation/tooling, no UX guidance beyond "test on devices").
- Media: comparative desktop/mobile Wikipedia screenshots hosted on Wikimedia Commons — not downloaded, consistent with all Wikipedia ingestions; no `raw/media/` subfolder created.

## 2026-06-25 (39)

- Re-ingested `raw/copyrighted/50_ui_tips.pdf` (Victor Ponamariov, *50 Tips to Improve User Interface*) under updated schema. Two new concept pages created with common-knowledge bodies and copyrighted content in `## Further reading`:
  - [[form-design]] — visible labels vs. placeholders, label proximity, input width as affordance signal, friction reduction, option selectors, progress indicators, validation placement, modal form tradeoffs, single primary action button.
  - [[loading-states]] — empty states, skeleton screens vs. spinners, button loading state stability, timing (delay and long-operation updates).
- `## Further reading` sections updated on: [[interface-design-principles]] (replaced old FR with links to new pages + three additional patterns: spatial separation of dangerous actions, icon labeling, no dead ends); [[accessibility]] (expanded with image-overlay contrast technique and placeholder accessibility note); [[typography]] (added line-height multipliers, headline proximity, full-width text → Z-pattern); [[gestalt-psychology]] (added form proximity examples and Miller's Law mention); [[fitts-law]] (clickable area via padding; gallery slider dots vs. clickable areas); [[hicks-law]] (≤5–7 options → revealed choices over dropdown); [[action-buttons]] (single primary button per view); [[trust-and-credibility]] (post date as credibility signal); [[affordance]] (scroll affordance via partial visibility; link affordance without hover); [[process-funnel]] (goal gradient effect in multi-step forms; complex forms in modals); [[browsable-content]] (scroll affordance; no dead ends; frequency-first ordering).
- `schema.md` updated: added concrete definition of "common knowledge" for copyrighted-source ingestion, specific red flags (numeric thresholds, named effects applied by the source, implementation techniques, mirrored problem lists), and a self-check rule. Added that an empty body is acceptable if all content belongs in Further reading.
- Excluded from new pages (in body or FR): icon design consistency (thin — one-to-two sentences, folded into [[interface-design-principles]] FR); copy-to-clipboard button (utility tip, below concept threshold); horizontal menu vs. sidebar (layout preference, too thin); auto-submit verification codes (micro-interaction, too thin); large data handling / ellipsis (too thin for a page; [[browsable-content]] FR covers overflow hint); Miller's Law (named in one sentence in context of form grouping — only mentioned in [[gestalt-psychology]] FR, no dedicated page because single source and thin).

## 2026-06-25 (38)

- Wikipedia "Visual hierarchy" → `raw/safe/wikipedia-visual-hierarchy.html`, source page [[wikipedia-2026-visual-hierarchy]]. Created [[visual-hierarchy]]: Gestalt-psychology foundation and Von Restorff (isolation) effect; four physical characteristics driving contrast (color, size, alignment, character); negative space as isolation tool; UX application (aligning visual order with conceptual order, navigational prioritization); squint test as informal hierarchy evaluation.
- Cross-links: [[gestalt-psychology]] `related:` updated with `visual-hierarchy`; [[clear-first-reads]] `related:` updated with `visual-hierarchy` and `wikipedia-2026-visual-hierarchy`.
- Excluded: cartography section (not UX/UI); Fréchet-distance eye-tracking study details (academic methodology); camouflage example (illustrative only); Jacques Bertin's visual variables (one sentence, single source — too thin for an entity page); Bauhaus "See also" (no content). Media: Wikimedia-hosted images not downloaded (consistent with all Wikipedia ingestions).

## 2026-06-25 (37)

- Wikipedia "Typography" → `raw/safe/wikipedia-typography.html`, source page [[wikipedia-2026-typography]]. Created [[typography]]: legibility vs. readability as distinct concepts (perception vs. comprehension); saccadic rhythm and line-length implications (Spencer/Coe/Reynolds, RCA); typeface selection by content category (long-form body → serif romans; compact layouts → tight serif; short copy → sans-serif; headlines → display); text composition variables (leading, justification, underlining, tracking); typographic "color" (ink density); display vs. text typography tradeoffs; typeface as tone/mood signal; digital typography.
- Cross-links: [[clear-first-reads]] updated — `typography` added to `related:`, URL added to `sources:`, font lever now wikilinks to [[typography]].
- Excluded: movable-type history (Gutenberg, Bi Sheng, Wang Zhen, Korea) — history, not UX; experimental/Dada typography (Picabia, David Carson) — artistic, not practical guidance; historical type designers (Garamond, Jenson, Griffo, Caslon) — specific historical names; inscriptional/stone-carving — craft, not digital UX; etymology; International Typographic Style / Swiss style history; Steve Jobs / font naming confusion; ATypI / Type Directors Club (first source only, below entity threshold); Miles Tinker's experimental methodology details (finding retained, procedure omitted). Media: article images on Wikimedia Commons — not downloaded (consistent with all Wikipedia ingestions).

## 2026-06-25 (36)

- Wikipedia "Color theory" → `raw/safe/wikipedia-color-theory.html`, source page [[wikipedia-2026-color-theory]]. Concept page [[color-theory]] and source page existed from a prior session; [[clear-first-reads]] and [[accessibility]] were updated then — but `index.md`, `log.md`, and `overview.md` were not. This entry completes the ingestion.
- [[color-theory]] covers: RGB/additive vs. CMYK/subtractive (CMYK weak on orange and some purples); four color-wheel schemes (complementary, analogous, split-complementary, triadic); Chevreul's three contrast types (simultaneous, successive, mixed) — perceptual, distinct from WCAG luminance ratios; warm/cool (mostly saturation/value effect, not hue); color harmony as function of individual + cultural + contextual + temporal factors (~2.3M perceivable colors makes fixed formulae "fundamentally unsound"); color symbolism is culture-bound, no universal meaning.
- Cross-links: [[clear-first-reads]]'s "complementary colors" → [[color-theory]]; [[accessibility]]'s "never rely on color alone" extended with culture-bound-symbolism reason; [[wcag]] linked from contrast section.
- Excluded: history of theorists (Aristotle through Bauhaus — Kandinsky, Itten, Birren, Albers — named, not elaborated); Munsell/RYB detail beyond RGB/CMYK; split-primary-palette and tints-and-shades (painting technique, no UI application); camouflage/heat-paint/Disney (one-sentence examples). Media: nine figures in article, all on Wikimedia Commons — not downloaded; no `raw/media/` subfolder (consistent with all Wikipedia ingestions, where images are externally hosted).

## 2026-06-25 (35)

- Wikipedia "The Design of Everyday Things" → `raw/safe/wikipedia-design-of-everyday-things.html`, source page [[wikipedia-2026-design-of-everyday-things]]. Verified against raw HTML — caught WebFetch summary asserting "Norman doors," "forcing functions," "discoverability," "mental model/system image" as covered; raw HTML has zero matches for any of them. None extracted.
- Created [[seven-stages-of-action]]: four-execution/three-evaluation action cycle, gulf of execution + gulf of evaluation, four principles (visibility, conceptual model, mapping, feedback) — kept on one page since each is one sentence in the article. Added to [[affordance]] as confirming second source (this book is the origin of Norman's 1988 narrowing). Added historical footnote to [[customer-centered-design]]: Norman coined "user-centered design" 1986/1988; this wiki's term is *The Design of Sites*' deliberate widening.
- Excluded: other chapter titles (no elaborating content); Reception section's industrial-designer anecdote (too thin); "See also" (Action slip — already in [[usability-engineering]]; *Emotional Design*, Industrial/Interaction design, Interface design principles — already in [[interface-design-principles]]).

## 2026-06-25 (34)

- `raw/safe/vanDuyne_G_3PP_491-544.pdf` (Pattern Group G, Advanced E-Commerce). Created [[vanduyne-2006-advanced-e-commerce]] and seven concept pages: [[featured-products]] (G1), [[cross-selling-and-up-selling]] (G2), [[personalized-recommendations]] (G3), [[recommendation-community]] (G4), [[multiple-destinations]] (G5), [[gift-giving]] (G6), [[order-tracking-and-history]] (G7) — kept separate because G1–G4 are non-exclusive techniques, not alternative answers to one decision.
- First media extraction: used `pypdf` (no `pdftoppm`/`pdfimages` available) → 40 raster images in `raw/media/vanduyne-2006-advanced-e-commerce/`, mapped to figure numbers. G6.2/G7.2 each yielded more chunks than expected — verified by opening each, confirmed sequential multi-step screenshots, named with letter suffixes (G6.2a–G6.2d, G7.2a–G7.2b). Seven vector "Solution" diagrams didn't extract; noted in source page.
- New entities: [[walmart]] and [[lands-end]] — both previously bare names, now have real depth here. Substantial additions to [[amazon]], [[ebay]], [[yahoo]]. Extended [[trust-and-credibility]]: personalization-data disclosure; UGC moderation as legal risk (libel, minors' data).
- Below threshold despite 2 mentions: Martha Stewart's site and Barnes & Noble (no substance beyond name-drop, per the CNN/Epicurious bar). Netflix: two mentions within this one chapter = single source. Excluded: G1.1/G1.2/G7.1/G7.2 cross-reference tables (prose instead); AJAX (implementation detail).

## 2026-06-25 (33)

- Created `raw/media/` convention: each source's extracted media goes in `raw/media/<source-page-slug>/`. Added to `schema.md` step 4. Applies to safe and copyrighted sources; copyrighted media still can't get source-page or index entries.

## 2026-06-25 (32)

- `schema.md` updated: laws reclassified as concepts (not entities). Moved [[fitts-law]] and [[hicks-law]] from `wiki/entities/` → `wiki/concepts/`, changed `type:`, added `sources:`. Slugs unchanged so no wikilinks broke. Incidental fix: [[gestalt-psychology]] had been miscategorized under Entities in `index.md` since creation — moved to Concepts.

## 2026-06-25 (31)

- `schema.md` updated: Wikipedia `sources:` entries use live URL, not local snapshot filename. Fixed 8 affected concept pages. `digitalgov-*.html` filenames left unchanged — request was Wikipedia-scoped.

## 2026-06-25 (30)

- Wikipedia "Affordance" → `raw/safe/wikipedia-affordance.html`, source page [[wikipedia-2026-affordance]]. Created [[affordance]]: Gibson's 1966/1979 relational sense; Norman's 1988 HCI narrowing (perceived action possibilities); Norman's 2013 "signifiers" addition (affordance = possible, signifier = where to act — critical for touchscreens); Gaver's perceivable/hidden/false split. Updated [[action-buttons]] to link rather than carry its own ad hoc explanation.
- Excluded: Jenny L. Davis's 2016/2020 mechanisms-and-conditions sociology framework (one step removed from design/HCI usage); cross-disciplinary extensions (language education, criminology, sports science, AI, fire safety — no design-specific content).

## 2026-06-24 (29)

- `raw/safe/vanDuyne_B_3PP_215-266.pdf` (Pattern Group B, Navigation Framework). Created [[vanduyne-2006-creating-navigation-framework]], [[multiple-ways-to-navigate]] (B1 — resolves long-flagged gap), [[browsable-content]] (B2 — resolves long-flagged gap), [[content-organization-schemes]] (B3–B7 merged: five schemes as a menu for one decision), [[category-pages]] (B8).
- B9 (SITE ACCESSIBILITY): no new page — [[accessibility]] already covered the ground. Folded only genuinely new material: curb-cut-effect framing; green-unvisited/red-visited link-color example; 2005 Mankoff/Fait/Tran study (expert review with screen reader found most problems of four methods, but still only ~50% of full lab study); style-sheets/accessibility note. Added two techniques to [[card-sorting]] from B3: category identification and category description.
- Excluded: accessibility tools (WebXACT/Bobby, Vischeck, Fangs — defunct circa-2006 software); W3C "ten quick tips" (superseded by POUR/WCAG); HTML/CSS syntax (implementation); mobile tips (Group M not ingested).

## 2026-06-24 (28)

- Wikipedia "Card sorting" → `raw/safe/wikipedia-card-sorting.html`, source page [[wikipedia-2026-card-sorting]]. Folded into [[card-sorting]]: open/closed distinction; tree testing/reverse card sorting; Modified-Delphi method (Celeste Paul); semantic vs. syntactic analysis; remote/online tradeoff.
- Excluded: Hungarian algorithm, minimum-spanning-tree formula, multidimensional scaling (statistics, not card-sorting-specific).

## 2026-06-24 (27)

- Lint (60 files). Zero orphans/broken links/mismatches. Declined Jakob Nielsen entity page (named-practitioner precedent). Fixed 4 issues: stray `above-the-fold` from [[gestalt-psychology]]'s `related:`; stray `usability-evaluation-methods` from [[digitalgov-2026-interviews]]'s `related:`; added missing [[wikipedia-2026-web-accessibility-initiative]] to [[accessibility]]'s `related:`; deduplicated RITE method (full version on [[usability-evaluation-methods]], pointer on [[usability-engineering]]).

## 2026-06-24 (26)

- Wikipedia "Usability testing" → `raw/safe/wikipedia-usability-testing.html`, source page [[wikipedia-2026-usability-testing]]. Folded into [[usability-evaluation-methods]]: guerrilla/remote testing; A/B and multivariate testing; Nielsen's five-users claim and Nielsen-Landauer formula U=1−(1−p)ⁿ (55–95%+ variance in practice); sampling limitations (WHO: 1.3B people with disabilities, 16% of population; WEIRD bias).
- Excluded: 2015 medical-device and 1982 Apple IIe case studies; Education/Survey-research sections (pedagogy, not design).

## 2026-06-24 (25)

- Wikipedia "Usability engineering" → `raw/safe/wikipedia-usability-engineering.html`, source page [[wikipedia-2026-usability-engineering]]. Created [[usability-engineering]]: 1988 Whiteside & Bennett origin; Nielsen's 1993 five attributes (learnability, efficiency, memorability, errors, satisfaction); ISO 9241 definition; slip/mistake/mode-error taxonomy.
- Excluded: bare practitioner list (Mayhew, Norman, Cooper, Nielsen, Carroll, Constantine, Rosson, Krug); defunct tools (Web Metrics Tool Suite, WebSAT/WebCAT/WebVIP/FLUD — implementation); NIST biometrics (too narrow).

## 2026-06-24 (24)

- Wikipedia "Gestalt psychology" → `raw/safe/wikipedia-gestalt-psychology.html`, source page [[wikipedia-2026-gestalt-psychology]]. Created [[gestalt-psychology]] (type: concept — eight sub-principles, not one quantifiable law). Named previously-implicit uses: [[grid-layout]]'s proximity/similarity and Wichita State placement research; [[clear-first-reads]]'s figure-ground.
- Excluded: Gestalt school history (social psychology, Nazi-era emigration); cartography examples already illustrated via [[grid-layout]]/[[clear-first-reads]].

## 2026-06-24 (23)

- Wikipedia "Stroop effect" → `raw/safe/wikipedia-stroop-effect.html`, source page [[wikipedia-2026-stroop-effect]]. No new page — single source, below threshold, thin on design relevance. Folded one sentence into [[accessibility]]: automaticity-theory explanation for why conflicting color/text cues create friction. Excluded: three competing theories, experimental methodology, emotional-Stroop variant, clinical uses. Revisit if a second source connects Stroop to interface design.

## 2026-06-24 (22)

- Wikipedia "Hick's law" → `raw/safe/wikipedia-hicks-law.html`, source page [[wikipedia-2026-hicks-law]]. Created [[hicks-law]]: formula T = b·log₂(n+1); design implications (organized vs. unstructured choices, progressive disclosure, menu design). Linked from [[fitts-law]] and [[homepage-portal]] (95/5 above-the-fold rule as progressive disclosure instance).
- Excluded: entropy-based formula for unequal-probability choices (information theory, not UX).

## 2026-06-24 (21)

- Wikipedia "Fitts's law" → `raw/safe/wikipedia-fittss-law.html`, source page [[wikipedia-2026-fittss-law]]. Reverses earlier "stays inline" call — article supplied movement-time formula, index of difficulty, design implications (infinite edges, magic corners, touchscreen sizing, radial-menu handedness), and two related laws. Created [[fitts-law]]. Linked from [[know-your-customers]], [[accessibility]], [[organized-search-results]], [[action-buttons]].
- Excluded: full mathematical derivation/Shannon-formulation history; specific validating studies (academic detail, not design guidance).

## 2026-06-24 (20)

- Lint (54 files). Zero issues. Confirmed [[vanduyne-2006-glossary]] as "broad survey" exemption. Confirmed [[wai]] and [[wai-aria]] should stay separate (no content overlap; org/spec-output split mirrors hub/deep-dive pattern elsewhere). Fixed 2 cross-references. Watchlist: PAGE TEMPLATE (D1) and NAVIGATION BAR (K2) top gaps.

## 2026-06-24 (19)

- Wikipedia "WAI-ARIA" → `raw/safe/wikipedia-wai-aria.html`, source page [[wikipedia-2026-wai-aria]]. Created [[wai-aria]]: roles/states/properties model; accessibility tree; Five Rules of ARIA. Kept at design-principle level; excluded `aria-*` syntax beyond two rule examples (`role="presentation"`, `aria-hidden="true"`).

## 2026-06-24 (18)

- Wikipedia "Web Accessibility Initiative" → `raw/safe/wikipedia-wai.html`, source page [[wikipedia-2026-web-accessibility-initiative]]. Created entity [[wai]]: W3C body (founded 1997) producing WCAG + ATAG (v2.0/2015), UAAG (v2.0/2015), WAI-ARIA (since 2014), discontinued XAG (2002). Folded 71%-abandonment stat into [[accessibility]]. ATAG/UAAG/WAI-ARIA one sentence deep here — stayed inline, below threshold.

## 2026-06-24 (17)

- Wikipedia "Web Content Accessibility Guidelines" → `raw/safe/wikipedia-wcag.html`, source page [[wikipedia-2026-web-content-accessibility-guidelines]] (CC BY-SA 4.0 — first explicit note; applies to all Wikipedia sources in this log). Split [[wcag]] out of [[accessibility]]: 61 success criteria in 2.0 (+17 in 2.1, +9/−1 in 2.2 Oct 2023), unfinished 3.0 draft; legal mandates (2024 US DOJ, EU 2016/2025, UK 2018, Canada *Jodhan*).
- **Caught factual error**: earlier WebFetch summary for [[wikipedia-2026-web-accessibility]] reported 65 criteria for WCAG 2.0; raw HTML confirms 61. Corrected in [[accessibility]] and [[wcag]], annotated in both source pages.

## 2026-06-24 (16)

- Lint (48 files). Zero issues. Merge candidates re-checked — none. Fixed 6 cross-references (mechanical). Gap watchlist: PAGE TEMPLATE (D1) and NAVIGATION BAR (K2) top.

## 2026-06-24 (15)

- Wikipedia "Web Accessibility" → `raw/safe/wikipedia-web-accessibility.html`, source page [[wikipedia-2026-web-accessibility]] (CC BY-SA 4.0; content paraphrased throughout — applies to all Wikipedia sources). Folded into [[accessibility]]: POUR principles; WCAG A/AA/AAA levels; assistive-tech examples beyond screen readers; 2018 WebAIM training-rarity stat. Excluded: country-by-country legislation/litigation (legal reference, not design guidance). Note: 65 success-criteria figure here corrected to 61 in (17).

## 2026-06-24 (14)

- Three digital.gov pages (public domain, GSA/TTS basis). Created [[digitalgov-2026-usability-testing]], [[digitalgov-2026-interviews]], [[digitalgov-2026-content-introduction]]; saved HTML snapshots to `raw/safe/`. No new concept pages — all folded: session structure/recruiting/scenarios → [[usability-evaluation-methods]]; 5 Whys/word-mirroring → [[customer-research-methods]]; authoritativeness/content-currency → [[trust-and-credibility]] and [[web-site-development-process]]. Excluded "default to HTML" and "optimize for search" (SEO/implementation). Added Source Triage section to `schema.md`.

## 2026-06-24 (13)

- `raw/50_ui_tips.pdf` (Ponamariov) — copyrighted: self-published, no license. Moved to `raw/copyrighted/` (first use). No source page, no concept pages, not in index. "Further reading" pointers added to [[interface-design-principles]] and [[accessibility]] only. Other tips (link styling, justified text, modals, icon consistency) have no existing page or are pure visual-implementation detail.

## 2026-06-24 (12)

- User saved `raw/safe/Design principles _ U.S. Web Design System (USWDS).pdf` — local snapshot for [[uswds-2025-design-principles]]. Verified against existing pages — no contradictions. Additional "Earn Trust" specifics (link-rot fixes, skim-writing, open code/data) documented in source page for future pass. Updated `sources:` on four citing pages; confirmed public-domain status (17 U.S.C. § 105).

## 2026-06-24 (11)

- USWDS "Design Principles" — wiki's first non-book source. Created [[uswds-2025-design-principles]] and [[trust-and-credibility]] ("Earn Trust" — overlaps but doesn't replace un-ingested Group E). Folded others: WCAG 2.1/Section 508 → [[accessibility]]; cross-device consistency → [[interface-design-principles]]; analytics/bug reporting → [[web-site-development-process]] Maintenance. Excluded "Start with Real User Needs" (redundant with [[know-your-customers]]).

## 2026-06-24 (10)

- Lint (42 files). No issues. Fixed 11 cross-references; dropped 3 unjustified `related:` entries. Gap-priority list: PAGE TEMPLATE (D1, 9 files), NAVIGATION BAR (K2, 8), SHOPPING CART (F3, 7), MULTIPLE WAYS TO NAVIGATE (B1, 6), SITE BRANDING (E1, 5).

## 2026-06-24 (9)

- `vanDuyne_L_3PP_759-792.pdf` (Pattern Group L, Speeding Up). Created [[vanduyne-2006-speeding-up-your-site]]. L1–L5 (file count, image formats, table-splitting, markup-vs-images, caching) excluded — pure performance implementation. L6 (perceived speed, progress indicators: static message, marching ants, thermometer, progressive display) folded into [[interface-design-principles]] feedback principle.

## 2026-06-24 (8)

- `vanDuyne_J_3PP_661-676.pdf` (Pattern Group J, Site Search). Created [[vanduyne-2006-making-site-search-fast-and-relevant]], [[straightforward-search-forms]] (J2), [[organized-search-results]] (J3); expanded [[search-action-module]] (J1). Created entity [[ibm]] — now substantive in two sources (Ch. 1 business case + ThinkPad synonym-handling). Epicurious second mention still no substance — stays below threshold.

## 2026-06-24 (7)

- `vanDuyne_I_3PP_631-660.pdf` (Pattern Group I, Page Layouts). Created [[vanduyne-2006-designing-effective-page-layouts]], [[grid-layout]] (I1), [[above-the-fold]] (I2), [[clear-first-reads]] (I3), [[expanding-and-fixed-screen-width]] (I4+I5 combined — book always contrasts them directly), [[consistent-sidebars-of-related-content]] (I6). Excluded implementation content (HTML attributes, style-sheet code). Flagged PAGE TEMPLATE (D1) as top-priority gap.

## 2026-06-24 (6)

- `vanDuyne_Glos_3PP_867-896.pdf` (Glossary, A–X). Created [[vanduyne-2006-glossary]] as terminology cross-check — no contradictions found. Folded three refinements: personalization (system-inferred) vs. customization (customer-chosen) into [[homepage-portal]]; profile into [[personas-and-scenarios]]; Yahoo! directory example into [[yahoo]]. Excluded: AJAX, CSS, cookies, image formats, server/scripting tech (implementation).

## 2026-06-24 (5)

- Lint (33 files). No issues. Fixed stale entity-threshold claims in [[vanduyne-2006-web-design-patterns]]; fixed 4 one-directional cross-references. Flagged SITE BRANDING (E1) / PRIVACY POLICY (E4) — in un-ingested Group E.

## 2026-06-24 (4)

- `vanDuyne_C_3PP_267-282.pdf` (Pattern Group C, Powerful Homepage). Created [[vanduyne-2006-creating-powerful-homepage]], [[homepage-portal]] (C1), [[up-front-value-proposition]] (C2). Added "Patterns documented in full" list to [[web-design-patterns]].

## 2026-06-24 (3)

- `vanDuyne_01_3PP_001-018.pdf` (Ch. 1). Created [[vanduyne-2006-customer-centered-web-design]], [[design-centering-styles]], [[myths-of-customer-centered-design]]. Expanded [[customer-centered-design]] with five-factor definition and business case (IBM 400% sales jump; 5%→25% satisfaction-to-revenue). Entity pages created: [[yahoo]], [[amazon]], [[google]], [[ebay]] — all crossed 2+-source threshold with Ch. 1's substantive mentions, reversing the Ch. 5 call in (2).

## 2026-06-24 (2)

- `vanDuyne_05_3PP_097-116.pdf` (Ch. 5). Created [[vanduyne-2006-developing-customer-centered-sites]] and [[web-site-development-process]] (7-phase Discovery→Maintenance cycle). Amazon/Google now at 2 sources but both mentions shallow — no page yet (reversed in (3)).

## 2026-06-24

- Project created.
- `vanDuyne_02_3PP_019-038.pdf` (Ch. 2). Created [[vanduyne-2006-web-design-patterns]], [[web-design-patterns]], [[customer-centered-design]], [[action-buttons]], [[search-action-module]], [[process-funnel]].
- `vanDuyne_03_3PP_039-068.pdf` (Ch. 3). Created [[vanduyne-2006-knowing-your-customers]], [[know-your-customers]], [[accessibility]], [[task-analysis]], [[personas-and-scenarios]], [[customer-research-methods]], [[card-sorting]].
