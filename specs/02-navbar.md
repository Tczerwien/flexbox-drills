---
lab-id: lab-27-pattern-02
plan-source: _MASTER-PLAN/phase-07-frontend-fundamentals/02-FrontendFundamentals_week-by-week.md
concept-notes: ["Flexbox — Mental Model & Common Patterns"]
---

# Pattern 02 — Navbar

## Objective

Drill the canonical "logo on the left, nav links on the right, all vertically centered" navbar pattern across 3 rounds, building muscle memory toward the <30-second target by round 3.

## Why this lab exists

- **Reinforces Concept Notes:** 3
- **Frontend resource chapters covered:** CSS-Tricks A Complete Guide to Flexbox (justify-content); MDN justify-content; MDN align-items; Flexbox Froggy levels 5-7
- **Decision Gate N connection:** direct prep for Gate 4 — Vue layout components pin a top-bar with this exact primitive.

## Prerequisites

Verify each tool works before starting:

- [ ] Browser dev tools open
- [ ] `cd round-1 && ls 02-navbar.html` (empty file exists at all 3 round paths)

If any fail, fix per Phase 00 install notes before continuing.

## Estimated time

Round 1: 12 min. Round 2: 6 min. Round 3: 4 min.

## Design brief

**What to build:**

A single self-contained `.html` file with embedded `<style>` block. One `<nav>` element wraps a logo span and a links list. Logo pinned to the left, links pinned to the right, all vertically centered. Horizontal padding inside the nav.

## Acceptance criteria

1. Verify the `<nav>` element wraps the logo span and the links list in the `<body>` of `round-1/02-navbar.html`.
2. Inspect the embedded `<style>` block — verify `display: flex` is set on the `<nav>`.
3. Verify `justify-content` is set to `space-between` so the logo pins to the left edge and the links pin to the right edge of the nav.
4. Verify `align-items` is set to `center` so the logo and the links share a vertical baseline on the default row `flex-direction`.
5. Verify horizontal padding is set on the nav and `gap` is set between the link items in the right-side list.
6. Note in lab-notes.md the flexbox vocabulary applied for this pattern: prefer `display: flex` on the `<nav>`; choose `justify-content: space-between` and `align-items: center`; the default `flex-direction` row applies — no override required; use `gap` for spacing between link items; recognize that `flex-wrap`, `flex-basis`, `flex-grow`, `flex-shrink`, `flex: 1`, `flex: 2`, `min-height: 100vh`, and `media query` are vocabulary reserved for other patterns and are not used here.

## Stretch goals

- Apply a media query to stack the navbar vertically below 480px viewport width — verify the stacked layout renders cleanly.
- Run the rendered file with logo+3 links versus logo+5 links — verify `justify-content: space-between` behaves consistently across both shapes.

## Screenshots + Live URL deliverable

(Optional — drag round-3 .html onto Netlify Drop for a shareable preview URL.)

## Deliverable checklist

The lab is done when:

- [ ] All acceptance criteria checked across all 3 rounds
- [ ] `round-1/02-navbar.html` + `round-2/02-navbar.html` + `round-3/02-navbar.html` all render the navbar shape
- [ ] Round 3 completion time in lab-notes.md is <60 seconds
- [ ] Lab-notes.md "What I tried that didn't work" section captures any spacing dead-ends from rounds 1 and 2

## Common pitfalls

- Did you set `justify-content: space-between`? Alternatives like `space-around` or `space-evenly` shift the logo off the left edge.
- Did you remember `display: flex` on the `<nav>`? Without it, `justify-content` does nothing.
- Did you choose `gap` for the link spacing rather than per-item margins? Margins compound at the edges; `gap` does not.

## References

- Concept Notes 3
- [CSS-Tricks — A Complete Guide to Flexbox (justify-content)](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#justify-content) [sha256:912ddec15f66] 2026-05-28
- [MDN — justify-content](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/justify-content#Syntax) [sha256:0fb6d877ff07] 2026-05-28
- [MDN — align-items](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/align-items#Syntax) [sha256:4b19c6e93f50] 2026-05-28
- [Flexbox Froggy](https://flexboxfroggy.com/#Flexbox Froggy) [sha256:6304b774e9c7] 2026-05-28

<!-- citations-v1.1
- [CSS-Tricks — A Complete Guide to Flexbox (justify-content)](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#justify-content) [sha256:912ddec15f66] 2026-05-28
- [MDN — justify-content](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/justify-content#Syntax) [sha256:0fb6d877ff07] 2026-05-28
- [MDN — align-items](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/align-items#Syntax) [sha256:4b19c6e93f50] 2026-05-28
- [Flexbox Froggy](https://flexboxfroggy.com/#Flexbox Froggy) [sha256:6304b774e9c7] 2026-05-28
<!-- /citations-v1.1 -->

*Last updated: 2026-05-28*
