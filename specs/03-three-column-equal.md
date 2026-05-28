---
lab-id: lab-27-pattern-03
plan-source: _MASTER-PLAN/phase-07-frontend-fundamentals/02-FrontendFundamentals_week-by-week.md
concept-notes: ["Flexbox — Mental Model & Common Patterns"]
---

# Pattern 03 — 3-column equal

## Objective

Drill the canonical "three equal-width sibling columns" pattern across 3 rounds, building muscle memory toward the <30-second target by round 3.

## Why this lab exists

- **Reinforces Concept Notes:** 3
- **Frontend resource chapters covered:** CSS-Tricks A Complete Guide to Flexbox (flex shorthand); MDN flex; MDN flex-grow
- **Decision Gate N connection:** direct prep for Gate 4 — Vue layout columns rely on `flex: 1` to share remaining space equally.

## Prerequisites

Verify each tool works before starting:

- [ ] Browser dev tools open
- [ ] `cd round-1 && ls 03-three-column-equal.html` (empty file exists at all 3 round paths)

If any fail, fix per Phase 00 install notes before continuing.

## Estimated time

Round 1: 12 min. Round 2: 6 min. Round 3: 4 min.

## Design brief

**What to build:**

A single self-contained `.html` file with embedded `<style>` block. One container div wraps three sibling column divs. Each column takes one-third of the container width with `flex: 1`. Default row `flex-direction` applies.

## Acceptance criteria

1. Verify three sibling column divs are wrapped by one container div in the `<body>` of `round-1/03-three-column-equal.html`.
2. Inspect the embedded `<style>` block — verify `display: flex` is set on the container.
3. Verify each of the three columns has `flex: 1` so each takes an equal share of the container width.
4. Verify the default `flex-direction` row applies — no override is set on the container — so the columns line up left-to-right.
5. Compare the rendered column widths across the three rounds and note the round-1, round-2, round-3 timings in lab-notes.md.
6. Note in lab-notes.md the flexbox vocabulary applied for this pattern: prefer `display: flex` on the parent; choose `flex: 1` on each child (the `flex-grow` portion of the shorthand splits remaining space equally — `flex: 2` is reserved for the unequal variant); the default `flex-direction` row applies — no override required; use `gap` for inter-column spacing; recognize that `justify-content`, `align-items`, `flex-wrap`, `flex-basis`, `flex-shrink`, `min-height: 100vh`, and `media query` are vocabulary reserved for other patterns and are not used here.

## Stretch goals

- Apply a `gap` value on the container — verify the column widths recompute to share remaining space after the gap.
- Run the rendered file with five sibling columns instead of three — verify each takes one-fifth of the width.

## Screenshots + Live URL deliverable

(Optional — drag round-3 .html onto Netlify Drop for a shareable preview URL.)

## Deliverable checklist

The lab is done when:

- [ ] All acceptance criteria checked across all 3 rounds
- [ ] `round-1/03-three-column-equal.html` + `round-2/03-three-column-equal.html` + `round-3/03-three-column-equal.html` all render three equal columns
- [ ] Round 3 completion time in lab-notes.md is <60 seconds
- [ ] Lab-notes.md "What I tried that didn't work" section captures any per-column-width dead-ends from rounds 1 and 2

## Common pitfalls

- Did you set `flex: 1` on each column (not on the container)? The shorthand applies per-child.
- Did you remember `display: flex` on the container? `flex: 1` on children does nothing without it.
- Did you avoid setting fixed widths on the columns? Fixed widths defeat the `flex-grow` portion of `flex: 1`.

## References

- Concept Notes 3
- [CSS-Tricks — A Complete Guide to Flexbox (flex)](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#flex) [sha256:fd5601b58d77] 2026-05-28
- [MDN — flex](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/flex#Syntax) [sha256:af065b6bc02c] 2026-05-28
- [MDN — flex-grow](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/flex-grow#Syntax) [sha256:0598192daa72] 2026-05-28

<!-- citations-v1.1
- [CSS-Tricks — A Complete Guide to Flexbox (flex)](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#flex) [sha256:fd5601b58d77] 2026-05-28
- [MDN — flex](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/flex#Syntax) [sha256:af065b6bc02c] 2026-05-28
- [MDN — flex-grow](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/flex-grow#Syntax) [sha256:0598192daa72] 2026-05-28
<!-- /citations-v1.1 -->

*Last updated: 2026-05-28*
