---
type: concept
title: Affordance
tags: [affordance, perception, hci, design-principles]
related: [action-buttons, gestalt-psychology, seven-stages-of-action, wikipedia-2026-affordance, wikipedia-2026-design-of-everyday-things, form-design, loading-states]
sources: ["https://en.wikipedia.org/wiki/Affordance", "https://en.wikipedia.org/wiki/The_Design_of_Everyday_Things"]
created: 2026-06-25
updated: 2026-06-25
---

# Affordance

What an object or environment makes possible for an actor to do with it, and — crucially for design — what of that the actor can readily *perceive* without being told.

## Gibson's original sense

Psychologist James J. Gibson coined the term in 1966, refined in his 1979 book *The Ecological Approach to Visual Perception*: "the affordances of the environment are what it offers the animal, what it provides or furnishes, either for good or ill." Gibson's affordances are **relational** (a knee-high step affords climbing to an adult but not a crawling infant) and **objective** — they exist independent of whether the actor notices them. By this definition a chair affords throwing as well as sitting, whether or not anyone perceives the option.

## Norman's design sense, and signifiers

In 1988, Donald Norman narrowed the term for Human-Computer Interaction to only those action possibilities an actor can **readily perceive** — the version that stuck in design and HCI via *The Design of Everyday Things*. Where Gibson's chair affords both sitting and throwing, Norman's (perceived) affordances capture only the likelihood someone sits on it — what the object's appearance actually *suggests*.

Norman later said this narrowing was unintentional, and in a 2013 revision of the same book introduced a second term, **signifiers**, to split the two jobs cleanly: "Affordances determine what actions are possible. Signifiers communicate where the action should take place. We need both." This split matters most for digital interfaces — a touchscreen's flat glass has no physical property that affords tapping the way a [[action-buttons|raised button]] affords pressing, so on-screen designs lean almost entirely on signifiers (shading, icons, labels) to point at affordances that the hardware itself doesn't supply.

The book's own running example is doors: a flat plate signifies pushing, a small finger-sized button signifies pressing, a long rounded bar signifies pulling — Norman discusses door handles at particular length, to the point that a badly-signified door (one whose handle suggests the wrong action) is the field's go-to bad example. The same book is also where Norman's [[seven-stages-of-action|seven-stages-of-action model]] comes from — affordances and signifiers are specifically what narrows that model's **gulf of execution**, by making a system's allowable actions visible rather than hidden.

## Perceivable, hidden, and false affordances

William Gaver's three-way split, used widely alongside Norman's definition:

- **Perceivable** — the action possibility is apparent to the actor, e.g. a door knob shaped to suggest how it's gripped and turned, or a teapot's handle and spout shaped to suggest pouring.
- **Hidden** — a real action possibility exists but isn't apparent from looking, e.g. a shoe can pry a cork from a wine bottle, but nothing about a shoe's appearance suggests this.
- **False** — an apparent action possibility with no real function behind it, e.g. a placebo button that produces no actual effect but is perceived as doing something.

A well-designed [[action-buttons|action button]] is a deliberate perceivable affordance: a shaded, three-dimensional appearance borrows prior knowledge (physical buttons, learned GUI behavior) so the button's clickability doesn't have to be explained.

## Usage drift

Beyond the technical Gibson/Norman distinction, "affordance" has drifted toward an uncountable noun describing general discoverability ("this button has good affordance"), and "afford" has correspondingly drifted from its dictionary sense toward "suggest" or "invite." This drift is common enough in design writing to be worth naming, even though it blurs Gibson's original, more precise sense.

## Further reading

Victor Ponamariov's *50 Tips to Improve User Interface* (self-published ebook, no stated license — not ingested into this wiki; see `raw/copyrighted/50_ui_tips.pdf`) applies perceivable affordance to two UI patterns: showing a partially-visible item at the bottom of a dropdown or scrollable list as a signal that more options exist (scroll affordance rather than a hidden one), and ensuring links are visually distinct from body text — colored, underlined, or otherwise marked — without relying on hover state, so the interaction possibility is perceivable before the cursor moves.

## Notes for the wiki

Extracted from [[wikipedia-2026-affordance]]. The term had been used informally on [[action-buttons]] since that page's creation, without being explained — this page supplies the underlying theory the pattern was already leaning on, and [[action-buttons]] now links here instead of carrying the explanation itself.

Left out (per `schema.md`'s ingestion-report requirement): Jenny L. Davis's mechanisms-and-conditions framework (2016/2020) — a sociology-of-technology reframing ("how does X afford, for whom, under what circumstances") that's a step removed from the design/HCI usage the rest of this wiki documents, and didn't have an existing page or pattern to attach it to; the language-education and other cross-disciplinary extensions (criminology, sports science, AI, fire-safety signage) as named only in passing with no design-specific content.
