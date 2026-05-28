---
lab-id: lab-27-pattern-01
plan-source: _MASTER-PLAN/phase-07-frontend-fundamentals/02-FrontendFundamentals_week-by-week.md
concept-notes: ["Flexbox — Mental Model & Common Patterns"]
---

# Pattern 01 — Center child

## Objective

Drill the canonical "center one child both horizontally and vertically in a full-viewport container" pattern across 3 rounds, building muscle memory toward the <30-second target by round 3.

## Why this lab exists

- **Reinforces Concept Notes:** 3
- **Frontend resource chapters covered:** CSS-Tricks A Complete Guide to Flexbox (parent properties); MDN Basic concepts of flexbox; Flexbox Froggy levels 1-3
- **Decision Gate N connection:** direct prep for Gate 4 — Vue components arrange children with this exact primitive; the canonical center test is the single most-asked frontend interview question per deliverables.md.

## Prerequisites

Verify each tool works before starting:

- [ ] Browser dev tools open
- [ ] `cd round-1 && ls 01-center-child.html` (empty file exists at all 3 round paths)

If any fail, fix per Phase 00 install notes before continuing.

## Estimated time

Round 1: 12 min. Round 2: 6 min. Round 3: 4 min (target: 30 sec by round 3).

## Design brief

**What to build:**

A single self-contained `.html` file with embedded `<style>` block. One container div, one child div. Child centered horizontally and vertically. Container fills the viewport vertically.

## Acceptance criteria

1. Verify a single container div wraps a single child div in the `<body>` of `round-1/01-center-child.html`.
2. Inspect the embedded `<style>` block — verify `display: flex` is set on the container.
3. Verify `justify-content` is set to `center` and `align-items` is set to `center` on the container, with no `flex-direction` override needed because the default row applies.
4. Verify `min-height: 100vh` is set on the container so vertical centering renders against the full viewport.
5. Compare the rendered output across the three round files — note the round-1, round-2, round-3 timings in lab-notes.md.
6. Note in lab-notes.md the flexbox vocabulary applied for this pattern: prefer `display: flex` on the parent; choose `justify-content` and `align-items` on the parent (the default `flex-direction` row applies — no override required); cover full-viewport via `min-height: 100vh`; recognize that `gap`, `flex-wrap`, `flex-basis`, `flex-grow`, `flex-shrink`, `flex: 1`, `flex: 2`, and `media query` are vocabulary reserved for other patterns and are not used here.

## Stretch goals

- Apply a background color to the container and a contrasting color to the child — verify the centering visual holds.
- Run the rendered file at 320px, 768px, 1280px viewport widths via DevTools device emulation — verify centering survives all three.

## Screenshots + Live URL deliverable

(Optional — drag round-3 .html onto Netlify Drop for a shareable preview URL.)

## Deliverable checklist

The lab is done when:

- [ ] All acceptance criteria checked across all 3 rounds
- [ ] `round-1/01-center-child.html` + `round-2/01-center-child.html` + `round-3/01-center-child.html` all render the centered child
- [ ] Round 3 completion time in lab-notes.md is <60 seconds
- [ ] Lab-notes.md "What I tried that didn't work" section captures any wrong-property dead-ends from rounds 1 and 2

## Common pitfalls

- Did you set `min-height: 100vh` on the container? Without it, vertical centering renders against the child's own height, not the viewport.
- Did you remember `display: flex` on the container? `justify-content` + `align-items` alone do nothing without it.
- Did you verify the round-3 timing without notes open? Round 3 is muscle memory — no Googling allowed.

## References

- Concept Notes 3
- [CSS-Tricks — A Complete Guide to Flexbox (justify-content)](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#justify-content) [sha256:912ddec15f66] 2026-05-28
- [MDN — Basic concepts of flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Flexible_box_layout/Basic_concepts#The flex container) [sha256:aef288d2d19d] 2026-05-28
- [MDN — Aligning items in a flex container](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Flexible_box_layout/Aligning_items#Alignment) [sha256:af16fcef75cc] 2026-05-28
- [Flexbox Froggy](https://flexboxfroggy.com/#Flexbox Froggy) [sha256:6304b774e9c7] 2026-05-28

<!-- citations-v1.1
- [CSS-Tricks — A Complete Guide to Flexbox (justify-content)](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#justify-content) [sha256:912ddec15f66] 2026-05-28
- [MDN — Basic concepts of flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Flexible_box_layout/Basic_concepts#The flex container) [sha256:aef288d2d19d] 2026-05-28
- [MDN — Aligning items in a flex container](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Flexible_box_layout/Aligning_items#Alignment) [sha256:af16fcef75cc] 2026-05-28
- [Flexbox Froggy](https://flexboxfroggy.com/#Flexbox Froggy) [sha256:6304b774e9c7] 2026-05-28
<!-- /citations-v1.1 -->

*Last updated: 2026-05-28*
