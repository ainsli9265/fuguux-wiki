---
type: concept
title: Mobile-First Design
tags: [responsive-design, mobile-design, progressive-enhancement, strategy]
related: [responsive-web-design, expanding-and-fixed-screen-width, accessibility, wikipedia-2026-responsive-web-design]
sources:
  - "https://en.wikipedia.org/wiki/Responsive_web_design"
created: 2026-06-25
updated: 2026-06-25
---

# Mobile-First Design

**Mobile-first design** is a sequencing strategy for responsive design: begin by designing for the smallest, most constrained device — typically a smartphone with a narrow viewport, limited bandwidth, and touch input — and then progressively enhance the design for larger screens and more capable devices.

The logic is one of constraint-driven clarity. A small screen forces ruthless prioritization: only content and actions that genuinely matter to the user can fit. Starting there ensures that the core experience is solid for the most constrained context. Enhancements for tablet or desktop — wider layouts, richer imagery, additional columns of secondary content — are then layered on top of that working foundation, not the other way around.

This contrasts with the more historically common approach of designing for desktop first and then trying to compress or adapt that design for mobile — a process that often results in a degraded, afterthought mobile experience, because features designed for a wide canvas rarely reduce gracefully.

Mobile-first predates [[responsive-web-design]] as a concept and complements it in practice. RWD provides the technical mechanism (fluid grids, breakpoints) for adapting layout across screen sizes; mobile-first provides the *design priority order* for deciding which content and interactions receive that adaptation effort first. The two are often combined: a responsive site built mobile-first uses the smallest breakpoint as its baseline and adds layout complexity as viewport width grows.

Mobile-first is also relevant beyond screen size: designing for mobile often surfaces [[accessibility]] improvements that benefit all users — simpler navigation, larger tap targets, reduced cognitive load from fewer simultaneous choices.
