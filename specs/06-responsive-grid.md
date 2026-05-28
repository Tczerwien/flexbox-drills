---
lab-id: lab-27-pattern-06
plan-source: _MASTER-PLAN/phase-07-frontend-fundamentals/02-FrontendFundamentals_week-by-week.md
concept-notes: ["Flexbox — Mental Model & Common Patterns"]
---

# Pattern 06 — Responsive grid

## Objective

Drill the canonical "card grid that shows four cards per row on desktop, wraps to two cards per row at tablet, and one card per row at mobile" pattern across 3 rounds, building muscle memory toward the <30-second target by round 3.

## Why this lab exists

- **Reinforces Concept Notes:** 3
- **Frontend resource chapters covered:** CSS-Tricks A Complete Guide to Flexbox (flex-wrap, flex-basis); MDN flex-wrap; MDN @media; Flexbox Froggy levels 14-17
- **Decision Gate N connection:** direct prep for Gate 4 — the Phase 12 referral project home grid uses this primitive end-to-end.

## Prerequisites

Verify each tool works before starting:

- [ ] Browser dev tools open
- [ ] `cd round-1 && ls 06-responsive-grid.html` (empty file exists at all 3 round paths)

If any fail, fix per Phase 00 install notes before continuing.

## Estimated time

Round 1: 12 min. Round 2: 6 min. Round 3: 4 min.

## Design brief

**What to build:**

A single self-contained `.html` file with embedded `<style>` block. One container div wraps several card divs. The container wraps card rows via `flex-wrap`. Each card claims a starting size via `flex-basis` (or via the `flex` shorthand). A media query at a tablet breakpoint shifts each card's basis to claim half the row; a second media query at a mobile breakpoint shifts each card's basis to claim the full row.

## Acceptance criteria

1. Verify the container div wraps four or more card divs in the `<body>` of `round-1/06-responsive-grid.html`.
2. Inspect the embedded `<style>` block — verify `display: flex` is set on the container and `flex-wrap` is set to `wrap` so card rows can wrap.
3. Verify each card has a `flex-basis` (or `flex` shorthand value carrying the basis) that yields four cards per row at desktop widths.
4. Apply a media query at a tablet breakpoint — verify the card `flex-basis` (or `flex` shorthand) shifts so two cards fit per row.
5. Apply a second media query at a mobile breakpoint — verify the card `flex-basis` (or `flex` shorthand) shifts so one card fills the row.
6. Compare the rendered grid at 320px, 768px, and 1280px viewport widths — confirm the 1-col, 2-col, 4-col layouts each render cleanly and note the round-1, round-2, round-3 timings in lab-notes.md.
7. Note in lab-notes.md the flexbox vocabulary applied for this pattern: prefer `display: flex` on the container; choose `flex-wrap: wrap` to allow card rows to wrap; set per-card `flex-basis` (or use the `flex` shorthand carrying a basis); switch the basis values via a `media query` at tablet and mobile breakpoints; recognize that `flex-grow`, `flex-shrink`, `flex: 1`, `flex: 2`, and `gap` can compose with this pattern as stretch goals; recognize that `justify-content`, `align-items`, `flex-direction`, and `min-height: 100vh` are vocabulary reserved for other patterns and are not used here.

## Stretch goals

- Apply `gap` on the container — verify the card widths recompute to share remaining space after the gap.
- Run the rendered file with eight cards instead of four — verify the grid wraps cleanly into two desktop rows.
- Apply `flex-grow: 1` on each card alongside the basis — verify the last row fills the container width even when the card count is odd.

## Screenshots + Live URL deliverable

(Optional — drag round-3 .html onto Netlify Drop for a shareable preview URL.)

## Deliverable checklist

The lab is done when:

- [ ] All acceptance criteria checked across all 3 rounds
- [ ] `round-1/06-responsive-grid.html` + `round-2/06-responsive-grid.html` + `round-3/06-responsive-grid.html` all render the responsive grid
- [ ] Round 3 completion time in lab-notes.md is <60 seconds
- [ ] Lab-notes.md "What I tried that didn't work" section captures any breakpoint dead-ends from rounds 1 and 2

## Common pitfalls

- Did you set `flex-wrap: wrap`? Without it, cards stay on one row and compress.
- Did you set `flex-basis` rather than `width`? Width values can collide with the flex shorthand and produce surprising widths.
- Did you remember to set both the tablet and the mobile media query? A single breakpoint produces only a 2-col or 1-col stretch, not the three-tier shape.

## References

- Concept Notes 3
- [CSS-Tricks — A Complete Guide to Flexbox (flex-wrap)](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#flex-wrap) [sha256:9b30ac46885b] 2026-05-28
- [CSS-Tricks — A Complete Guide to Flexbox (flex-basis)](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#flex-basis) [sha256:3e026459fdac] 2026-05-28
- [MDN — flex-wrap](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/flex-wrap#Syntax) [sha256:a52f89fdd79f] 2026-05-28
- [MDN — @media](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@media#Syntax) [sha256:326a7728fa03] 2026-05-28
- [Flexbox Froggy](https://flexboxfroggy.com/#Flexbox Froggy) [sha256:6304b774e9c7] 2026-05-28

<!-- citations-v1.1
- [CSS-Tricks — A Complete Guide to Flexbox (flex-wrap)](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#flex-wrap) [sha256:9b30ac46885b] 2026-05-28
- [CSS-Tricks — A Complete Guide to Flexbox (flex-basis)](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#flex-basis) [sha256:3e026459fdac] 2026-05-28
- [MDN — flex-wrap](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/flex-wrap#Syntax) [sha256:a52f89fdd79f] 2026-05-28
- [MDN — @media](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@media#Syntax) [sha256:326a7728fa03] 2026-05-28
- [Flexbox Froggy](https://flexboxfroggy.com/#Flexbox Froggy) [sha256:6304b774e9c7] 2026-05-28
<!-- /citations-v1.1 -->

*Last updated: 2026-05-28*
