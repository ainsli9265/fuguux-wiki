---
type: concept
title: Trust and Credibility
tags: [trust, credibility, privacy, security, ux-principles]
related: [homepage-portal, myths-of-customer-centered-design, customer-centered-design, uswds-2025-design-principles, digitalgov-2026-content-introduction, personalized-recommendations, recommendation-community, quick-flow-checkout, easy-returns, vanduyne-2006-advanced-e-commerce, vanduyne-2006-basic-e-commerce]
sources: ["Design principles _ U.S. Web Design System (USWDS).pdf", https://designsystem.digital.gov/design-principles/, digitalgov-introduction-to-content.html, vanDuyne_G_3PP_491-544.pdf, vanDuyne_F_3PP_431-490.pdf]
created: 2026-06-24
updated: 2026-06-25
---

# Trust and Credibility

Trust in a Web site is never assumed by default — it has to be actively earned, and re-earned on every visit, through consistent and verifiable signals rather than a one-time claim.

Two e-commerce-specific trust signals deserve explicit treatment: payment security and return policy visibility. At payment entry, a visible privacy policy link and a secure-connection indicator (HTTPS lock icon) address the specific anxiety of handing over financial information — this is the highest-stakes trust moment in the checkout flow (see [[quick-flow-checkout]]). A clear, accessible return policy linked from every product page is a purchase-time trust signal, not only a post-purchase concern: customers who can see the policy before committing buy more confidently and return more often (see [[easy-returns]]).

- **Signal legitimacy clearly and consistently** — make it obvious, on every page, what the site is and who's responsible for it: clear ownership, real contact information, and a connection that visibly matches what it claims to be. HTTPS with a current, valid certificate is now a baseline trust signal, not an optional extra; for an official/institutional site, explicit identification as such (a visible badge or banner) matters too. This extends to content design generally — distinguishing official from non-official sources consistently (e.g. via shared design-system components) is one concrete way sites demonstrate the authoritativeness this signals.
- **Keep content current and retire it carefully** — review content regularly for accuracy (at least an annual audit), mark when something was last updated, give time-bound campaigns a defined end, and promptly remove or properly redirect outdated or rarely-used material rather than leaving it to silently rot. The same logic applies at the link level: actively find and fix broken/rotted links rather than letting them accumulate, and give proper notice (and a forwarding path) when content itself is moved or removed, instead of leaving visitors at a dead end. Stale, undated, broken, or abandoned content undercuts the same trust that an active bug-reporting channel builds (below) — a site that looks unmaintained reads as untrustworthy even if nothing is technically broken.
- **Protect what customers hand over** — sensitive data deserves protection appropriate to its sensitivity, and privacy commitments need to be both real and visible. This is the same trust burden [[homepage-portal]] already flags when discussing personalization: customers need to trust a site enough to hand over the data it runs on. [[personalized-recommendations]] is a concrete instance: disclose what behavioral/purchase data feeds a recommendation and how it's used, and get explicit opt-in before reusing it for anything beyond the recommendation itself (e.g. outside marketing).
- **Plan for user-generated content's legal exposure, not just its UX.** A [[recommendation-community|review system]] opens a site to obscenity, libel, and copyrighted material posted by customers — published use policies and filtering catch the routine cases, but the genuinely risky ones (a minor's data, a libelous claim) are a legal question as much as a design one, worth involving counsel on rather than treating as a pure interface decision.
- **Be reliable, and own it when you're not** — redundancy minimizes how much a single failure costs customers, and when something does break, a visible, responsive process for bugs and incidents does more for trust than silence.
- **Communicate honestly, in plain language** — content written so customers can actually understand it builds more trust than reassuring copy or polish. Concretely, that means writing for skimming and scanning rather than dense paragraphs, since almost nobody reads a page start to finish. This echoes one of the [[myths-of-customer-centered-design]]: customers have little patience for documentation, so trust has to come from the interface and content actually being clear, not from a fallback explanation customers have to go dig for.

**Forces:** trust signals (security indicators, plain language, visible policies) compete for the same above-the-fold space that [[homepage-portal]] already has to divide between branding, navigation, and content — earning trust isn't free; it costs real space and attention on the page itself.

This page overlaps with, but isn't identical to, *The Design of Sites*' own Pattern Group E, "Building Trust and Credibility" — not yet ingested into this wiki, and the source of the still-unexplained SITE BRANDING and PRIVACY POLICY patterns flagged in earlier lint passes. When Group E is eventually ingested, expand this page with that material rather than creating a separate one.

## Further reading

Victor Ponamariov's *50 Tips to Improve User Interface* (self-published ebook, no stated license — not ingested into this wiki; see `raw/copyrighted/50_ui_tips.pdf`) adds one concrete example: displaying a post date on articles is a direct credibility signal. The absence of a date leaves readers unable to judge whether content is current, which alone can undercut the trustworthiness this page describes — consistent with the "keep content current" point above, applied at the individual article level.
