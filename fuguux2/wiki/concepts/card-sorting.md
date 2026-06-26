---
type: concept
title: Affinity Diagramming and Card Sorting
tags: [information-architecture, customer-research, content-organization]
related: [customer-research-methods, personas-and-scenarios, organized-search-results, vanduyne-2006-knowing-your-customers, wikipedia-2026-card-sorting, content-organization-schemes, vanduyne-2006-creating-navigation-framework]
sources: [vanDuyne_03_3PP_039-068.pdf, "https://en.wikipedia.org/wiki/Card_sorting", vanDuyne_B_3PP_215-266.pdf]
created: 2026-06-23
updated: 2026-06-24
---

# Affinity Diagramming and Card Sorting

Two techniques for turning the raw data gathered through [[customer-research-methods]] into a candidate information architecture.

**Affinity diagramming**: write every individual point or concept gathered from interviews/observations on its own note, then physically cluster related notes together on a wall-sized surface, drawing connections between related clusters and using color to build up a hierarchy of groups and super-groups. The result is a single visual map of customer problems and needs that the whole team can see at once, and it commonly becomes the first draft of a site's information architecture and a seed for later [[personas-and-scenarios|scenarios and storyboards]].

**Card sorting**: give people the names of content items and have them group the items into categories that make sense to them, then name the resulting categories. There is rarely one "correct" grouping — sorting a deck of cards by suit, by number, or by color are all valid, just useful for different purposes — and the same is true of content: sorting "Apples / Oranges / Bananas" comes out differently depending on whether the audience cares about local-vs-tropical sourcing, organic-vs-conventional farming, or botanical classification. Running card sorting with several people (customers or teammates) and comparing where their groupings disagree is the valuable part — disagreement flags ambiguous terminology or items that genuinely belong in more than one category.

This basic version is **open card sorting** — participants invent their own category names, which is why it surfaces vocabulary as well as grouping. Its counterpart is **closed card sorting**, where participants sort into a fixed set of category names you supply instead of inventing their own; closed sorting doesn't generate a new structure, it evaluates how well an existing or proposed one already matches people's expectations — useful once you have a candidate information architecture and want to validate it rather than discover one from scratch. A related but distinct check is **tree testing** (also called reverse card sorting): give participants a task and an existing category hierarchy, with none of a real site's navigational aids (search, breadcrumbs), and see whether they can find the right place for it — this isolates whether the structure itself supports the task, separate from how a site's actual UI might compensate for a weak one. For getting a usable result from fewer participants, **Modified-Delphi card sorting** (created by Celeste Paul) has only the first participant do a full independent sort, with each subsequent participant iterating on the previous one's result rather than starting over, building consensus faster.

Across all variants, the resulting sorts get analyzed in one of two ways: **semantically**, by comparing the category labels and descriptions participants used (e.g. grouping "Difficult to understand" and "Confusing" as the same underlying complaint even though the words differ); or **syntactically**, by comparing the actual groupings — how often two cards landed together across participants, summarized into a similarity structure (sometimes visualized as a dendrogram) that reveals the most consistent groupings without relying on participants' own labels at all.

Both techniques work best with multiple participants and are meant to be revisited rather than treated as a single, final pass at site organization. Running them remotely via Web-based tools reaches more participants at lower cost, at the price of losing the moderator's ability to ask a participant *why* they grouped something a particular way. The same vocabulary card sorting surfaces is also useful for anticipating likely search terms before launch — see [[organized-search-results]] — rather than waiting to discover vocabulary mismatches through post-launch search-log analysis.

Card sorting *generates* candidate categories and labels; two related techniques *test* them afterward, once a candidate [[content-organization-schemes|hierarchy]] exists: **category identification** (give people a list of category names plus a list of tasks, and see which category they'd pick for each task) and **category description** (give people just a category name and ask what they think it contains). Running both with a fresh set of participants catches labels that made sense to the people who invented them but not to anyone else.
