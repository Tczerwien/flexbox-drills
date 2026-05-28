---
lab-id: lab-27-pattern-05
plan-source: _MASTER-PLAN/phase-07-frontend-fundamentals/02-FrontendFundamentals_week-by-week.md
concept-notes: ["Flexbox — Mental Model & Common Patterns"]
---

# Pattern 05 — Card with footer pinned

## Objective

Drill the canonical "card with variable middle content and a footer pinned to the card's bottom edge" pattern across 3 rounds, building muscle memory toward the <30-second target by round 3.

## Why this lab exists

- **Reinforces Concept Notes:** 3
- **Frontend resource chapters covered:** CSS-Tricks A Complete Guide to Flexbox (flex-direction); MDN flex-direction; MDN flex-grow; Flexbox Froggy level 10
- **Decision Gate N connection:** direct prep for Gate 4 — Vue card grids commonly require footers (price, CTA) pinned regardless of body content height.

## Prerequisites

Verify each tool works before starting:

- [ ] Browser dev tools open
- [ ] `cd round-1 && ls 05-card-with-footer.html` (empty file exists at all 3 round paths)

If any fail, fix per Phase 00 install notes before continuing.

## Estimated time

Round 1: 12 min. Round 2: 6 min. Round 3: 4 min.

## Design brief

**What to build:**

A single self-contained `.html` file with embedded `<style>` block. One card div wraps a header div, a middle content div, and a footer div. The card stacks its children vertically with `flex-direction: column`. The middle div takes the remaining card height via `flex: 1` so the footer pins to the card's bottom edge regardless of content height.

## Acceptance criteria

1. Verify the card div wraps a header div, a middle content div, and a footer div in the `<body>` of `round-1/05-card-with-footer.html`.
2. Inspect the embedded `<style>` block — verify `display: flex` is set on the card and `flex-direction` is set to `column` to stack the three sections vertically.
3. Verify the middle content div has `flex: 1` so the `flex-grow` portion of the shorthand consumes the remaining card height between header and footer.
4. Verify the footer div pins to the bottom of the card even when the middle content is shorter than the card's overall height.
5. Compare the rendered card across the three rounds using short, medium, and long middle-content strings — confirm the footer stays pinned across all three lengths and note the round-1, round-2, round-3 timings in lab-notes.md.
6. Note in lab-notes.md the flexbox vocabulary applied for this pattern: prefer `display: flex` on the card; choose `flex-direction: column` to stack vertically; apply `flex: 1` on the middle child (the `flex-grow` portion pushes the footer to the bottom edge); cover the parent card height via `min-height: 100vh` when the card is the page itself; recognize that `justify-content`, `align-items`, `flex-wrap`, `flex-basis`, `flex-shrink`, `flex: 2`, `gap`, and `media query` are vocabulary reserved for other patterns and are not used here.

## Stretch goals

- Apply a fixed footer background color and a contrasting middle background — verify the boundary between them sits at the bottom edge of the card.
- Run the rendered file with the middle content set to one short word and again with several paragraphs — verify the footer stays pinned in both cases.

## Screenshots + Live URL deliverable

(Optional — drag round-3 .html onto Netlify Drop for a shareable preview URL.)

## Deliverable checklist

The lab is done when:

- [ ] All acceptance criteria checked across all 3 rounds
- [ ] `round-1/05-card-with-footer.html` + `round-2/05-card-with-footer.html` + `round-3/05-card-with-footer.html` all render the card with pinned footer
- [ ] Round 3 completion time in lab-notes.md is <60 seconds
- [ ] Lab-notes.md "What I tried that didn't work" section captures any footer-floating dead-ends from rounds 1 and 2

## Common pitfalls

- Did you set `flex-direction: column` on the card? Without it, the children render horizontally instead of stacking.
- Did you set `flex: 1` on the middle div rather than on the footer? Setting it on the footer makes the footer grow, not the middle.
- Did you give the card a fixed height (or `min-height: 100vh` if it is the page itself)? Without a height for the card, the footer has nothing to pin against.

## References

- Concept Notes 3
- [CSS-Tricks — A Complete Guide to Flexbox (flex-direction)](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#flex-direction) [sha256:98f61dc83ad5] 2026-05-28
- [MDN — flex-direction](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/flex-direction#Syntax) [sha256:877e3999d65f] 2026-05-28
- [MDN — flex-grow](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/flex-grow#Syntax) [sha256:0598192daa72] 2026-05-28
- [Flexbox Froggy](https://flexboxfroggy.com/#Flexbox Froggy) [sha256:6304b774e9c7] 2026-05-28

<!-- citations-v1.1
- [CSS-Tricks — A Complete Guide to Flexbox (flex-direction)](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#flex-direction) [sha256:98f61dc83ad5] 2026-05-28
- [MDN — flex-direction](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/flex-direction#Syntax) [sha256:877e3999d65f] 2026-05-28
- [MDN — flex-grow](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/flex-grow#Syntax) [sha256:0598192daa72] 2026-05-28
- [Flexbox Froggy](https://flexboxfroggy.com/#Flexbox Froggy) [sha256:6304b774e9c7] 2026-05-28
<!-- /citations-v1.1 -->

*Last updated: 2026-05-28*
