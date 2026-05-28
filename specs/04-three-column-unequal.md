---
lab-id: lab-27-pattern-04
plan-source: _MASTER-PLAN/phase-07-frontend-fundamentals/02-FrontendFundamentals_week-by-week.md
concept-notes: ["Flexbox — Mental Model & Common Patterns"]
---

# Pattern 04 — 3-column unequal (middle 2× wider)

## Objective

Drill the canonical "three sibling columns with the middle column twice as wide as either flank" pattern across 3 rounds, building muscle memory toward the <30-second target by round 3.

## Why this lab exists

- **Reinforces Concept Notes:** 3
- **Frontend resource chapters covered:** CSS-Tricks A Complete Guide to Flexbox (flex-grow); MDN flex-grow; MDN flex
- **Decision Gate N connection:** direct prep for Gate 4 — content-vs-rail Vue layouts pin the middle reading column wider than the side rails using this exact ratio.

## Prerequisites

Verify each tool works before starting:

- [ ] Browser dev tools open
- [ ] `cd round-1 && ls 04-three-column-unequal.html` (empty file exists at all 3 round paths)

If any fail, fix per Phase 00 install notes before continuing.

## Estimated time

Round 1: 12 min. Round 2: 6 min. Round 3: 4 min.

## Design brief

**What to build:**

A single self-contained `.html` file with embedded `<style>` block. One container div wraps three sibling column divs. Outer columns take a `flex: 1` share; the middle column takes a `flex: 2` share — producing a 1:2:1 ratio that makes the middle column twice as wide as either flank.

## Acceptance criteria

1. Verify three sibling column divs are wrapped by one container div in the `<body>` of `round-1/04-three-column-unequal.html`.
2. Inspect the embedded `<style>` block — verify `display: flex` is set on the container.
3. Verify the first column has `flex: 1` and the last column has `flex: 1` so the two flanks share equal width.
4. Verify the middle column has `flex: 2` so the `flex-grow` ratio yields a 1:2:1 column width split.
5. Compare the rendered column widths across the three rounds — confirm the middle column is visibly twice as wide as either flank and note the round-1, round-2, round-3 timings in lab-notes.md.
6. Note in lab-notes.md the flexbox vocabulary applied for this pattern: prefer `display: flex` on the parent; choose `flex: 1` on the flank children and `flex: 2` on the middle child (the `flex-grow` portion of the shorthand splits remaining space in a 1:2:1 ratio); the default `flex-direction` row applies — no override required; use `gap` if inter-column spacing is desired; recognize that `justify-content`, `align-items`, `flex-wrap`, `flex-basis`, `flex-shrink`, `min-height: 100vh`, and `media query` are vocabulary reserved for other patterns and are not used here.

## Stretch goals

- Apply `flex: 3` on the middle column instead of `flex: 2` — verify the ratio shifts to 1:3:1 and the middle becomes three-fifths of the container width.
- Run the rendered file at a 320px viewport width — note whether the 1:2:1 ratio still reads clearly at narrow widths.

## Screenshots + Live URL deliverable

(Optional — drag round-3 .html onto Netlify Drop for a shareable preview URL.)

## Deliverable checklist

The lab is done when:

- [ ] All acceptance criteria checked across all 3 rounds
- [ ] `round-1/04-three-column-unequal.html` + `round-2/04-three-column-unequal.html` + `round-3/04-three-column-unequal.html` all render the 1:2:1 column shape
- [ ] Round 3 completion time in lab-notes.md is <60 seconds
- [ ] Lab-notes.md "What I tried that didn't work" section captures any ratio-math dead-ends from rounds 1 and 2

## Common pitfalls

- Did you set `flex: 2` on the middle column rather than `flex: 1`? Equal values yield equal widths regardless of column count.
- Did you remember `display: flex` on the container? `flex: 1` and `flex: 2` on children do nothing without it.
- Did you verify the ratio matches 1:2:1 in the rendered output, not just in the CSS values? Padding or per-column borders can mask the math.

## References

- Concept Notes 3
- [CSS-Tricks — A Complete Guide to Flexbox (flex-grow)](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#flex-grow) [sha256:d5a9174a70f2] 2026-05-28
- [MDN — flex-grow](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/flex-grow#Syntax) [sha256:0598192daa72] 2026-05-28
- [MDN — flex](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/flex#Syntax) [sha256:af065b6bc02c] 2026-05-28

<!-- citations-v1.1
- [CSS-Tricks — A Complete Guide to Flexbox (flex-grow)](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#flex-grow) [sha256:d5a9174a70f2] 2026-05-28
- [MDN — flex-grow](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/flex-grow#Syntax) [sha256:0598192daa72] 2026-05-28
- [MDN — flex](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/flex#Syntax) [sha256:af065b6bc02c] 2026-05-28
<!-- /citations-v1.1 -->

*Last updated: 2026-05-28*
