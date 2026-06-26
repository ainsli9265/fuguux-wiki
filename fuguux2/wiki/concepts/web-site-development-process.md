---
type: concept
title: Web Site Development Process
tags: [ux-process, design-methodology, project-management]
related: [iterative-design, rapid-prototyping, usability-evaluation-methods, customer-centered-design, know-your-customers, personas-and-scenarios, action-buttons, search-action-module, homepage-portal, up-front-value-proposition, amazon, google, uswds-2025-design-principles, vanduyne-2006-developing-customer-centered-sites, digitalgov-2026-content-introduction]
sources: [vanDuyne_05_3PP_097-116.pdf, "Design principles _ U.S. Web Design System (USWDS).pdf", "https://designsystem.digital.gov/design-principles/", digitalgov-introduction-to-content.html]
created: 2026-06-24
updated: 2026-06-24
---

# Web Site Development Process

A seven-phase end-to-end process for building or redesigning a Web site that embeds [[customer-centered-design]] and [[iterative-design]] at every stage — both across the whole project and within each individual phase. The process is explicitly non-linear: a team in a later phase that discovers a gap routinely jumps back to an earlier one, and doing so is framed as time and money saved rather than a setback, since [[iterative-design|fixing problems earlier is always cheaper]].

The first four phases — **Discovery, Exploration, Refinement, Production** — are "the design process": each moves the site from general to specific, each runs its own tight design→prototype→evaluate loop (more iterations early, fewer as designs firm up), and each ends with a client presentation and a concrete deliverable. The last three — **Implementation, Launch, Maintenance** — build, ship, and sustain the site; some design firms hand off to a different team (in the client's organization or a third firm) once Production is complete and never touch these phases themselves.

## 1. Discovery

Determines the project's scope, the client's business goals, and target customers' needs — sometimes starting with whether a Web site is even the right solution. Key activities: defining the site's purpose with the client; interviewing, surveying, or running focus groups with target customers (see [[know-your-customers]]); evaluating the existing site and competitors' sites (see [[usability-evaluation-methods]]); settling on an [[up-front-value-proposition]] — the site's value stated convincingly in one sentence, which becomes the unifying theme for everything on the site; and considering branding, personalization, and internationalization early.

Two named risks: **skipping Discovery** entirely under client pressure (usually a recipe for failure since scope and customer needs are never pinned down), and **gold-plating** — investing heavily in a technically interesting feature with little real customer benefit instead of shipping the essentials first and adding features in stages. A related discipline is getting "fundamentals right first": don't build advanced features (e.g. personalized recommendations) on top of a still-broken core flow (e.g. a shopping cart or checkout).

Discovery produces three deliverables:

- **Customer analysis document** — characteristics, needs, and tasks of intended customers, often using personas (see [[know-your-customers]], [[personas-and-scenarios]]).
- **Business analysis document** — a business plan, competitive analysis, and metrics for success (e.g. conversion rate, repeat-visitor rate).
- **Specification (requirements) document** — project description; a list of tasks/scenarios/storyboards labeled easy/moderate/difficult that later evaluations will be built around; a comprehensive feature list classified as "must have / should have / could have"; overall design goals; and metrics for each goal (e.g. download time under five seconds for 90% of customers). The chapter calls *not writing one* "the biggest risk you can take" — it is the step most often skipped, despite being cheap to produce and central to keeping client and team aligned.

## 2. Exploration

Generates several rough, alternative site designs — reflecting site structure and navigation, not yet color, imagery, or typography — and tests each quickly with customers. Produces medium-fidelity [[rapid-prototyping|site maps, storyboards, and schematics]] for each alternative, drawing on patterns such as [[homepage-portal]] for the structure of the homepage itself; the client picks one (or funds two for further comparison) based on which best serves the business, client, and customer goals established in Discovery.

## 3. Refinement

Takes the chosen design and polishes its navigation, layout, and flow, iteratively refining and informally testing it. Typeface, image treatment, and color palettes get decided; the site gets broken into page *templates* (e.g. homepage, second-level page) rather than designing every page individually. Deliverable: a single set of medium-to-high-fidelity site maps, storyboards, and schematics, now rich with real images, icons, and color, for client sign-off.

## 4. Production

Produces a final, highly detailed set of deliverables embodying the chosen design, with patterns shifting toward more low-level, technical concerns (e.g. [[action-buttons]] for how buttons should look pressable). Typical deliverables: a **design document** (site maps/storyboards/schematics describing exact interaction flow), an **interactive prototype**, **technical specifications** (server, languages, database, performance targets, sometimes a feasibility prototype), **design guidelines** (fonts, link colors, logo placement — a standing reference to keep the site internally consistent), and **Web page templates** (reusable HTML skeletons for each page class).

## 5. Implementation

Builds the actual HTML, images, database, and software. Content work intensifies here; tooling choices (revision control, bug tracking) should be proven, not experimental, since this is the wrong phase to learn a new tool. Naming conventions for files/folders get fixed, and SECURE CONNECTIONS-style features may require obtaining digital certificates from a certification authority (these are typically bound to a specific server name, so moving one between a test and production server can break). Testing during this phase includes feature completeness against the spec, cross-browser/cross-screen-size compatibility (including text-only browsers for blind customers), download time over slow connections, stress-testing for concurrent load, and copyediting — producing bug reports that drive fixes. Deliverables: the completed site, a maintenance document, a test plan document, and updated versions of earlier documents.

## 6. Launch

Live deployment, limited to only minor final polish (typos, broken links/images) since major issues should already be caught. Sites are sometimes rolled out in stages — core functionality first, to early adopters on a beta site, with feedback driving the rest — but staging poorly (e.g. shipping a visibly thin site) risks losing potential customers who judge it too early. A post-launch postmortem is a common way to capture what worked and what didn't for next time.

## 7. Maintenance

The longest and most expensive phase, and the most often neglected. Ongoing work includes bug fixes, collecting usability/satisfaction metrics, link-checking, enforcing design guidelines, periodic off-site backups, and maintaining server logs of traffic and search terms. Sustaining this well takes more than passive log review: a visible channel for customers to report bugs, dedicated analytics tooling rather than ad hoc data pulls, and publishing some of those metrics back to stakeholders (and sometimes the public) keep maintenance accountable rather than invisible. Content itself needs the same ongoing review as code and metrics: a full content audit at least once a year (e.g. the USDA's four-step process — set goals, establish scope, build a data-collection spreadsheet, then audit) catches accuracy drift and stale material before it undermines [[trust-and-credibility|customer trust]]. The central recurring decision is when a revision is warranted, and how big a revision: small redesigns can skip re-deriving the business analysis but should still respect the existing specification, design document, and guidelines to preserve a consistent look and feel; complete overhauls (triggered by shifting customer expectations/behavior, new technology, or a site that looks dated) restart the whole seven-phase process. Before fully switching to a redesigned site, get customer feedback first — via new usability tests, an opt-in preview link, or **virtual testing** (showing the new design to a small subset of customers and comparing their behavior to everyone else's, a method the chapter credits to [[amazon]] and [[google]] — the same technique [[usability-evaluation-methods]] documents under its standard Web-design name, A/B testing). Deliverables: periodic site metrics, severity-rated bug reports, and periodic backups.
