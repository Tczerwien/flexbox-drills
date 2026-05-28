---
lab-id: lab-27-pattern-07
plan-source: _MASTER-PLAN/phase-07-frontend-fundamentals/02-FrontendFundamentals_week-by-week.md
concept-notes: ["Flexbox — Mental Model & Common Patterns"]
---

# Pattern 07 — Sticky footer (page)

## Objective

Drill the canonical "page-level sticky footer — footer pinned to the bottom of the viewport when content is short, pushed below the viewport when content is long" pattern across 3 rounds, building muscle memory toward the <30-second target by round 3.

## Why this lab exists

- **Reinforces Concept Notes:** 3
- **Frontend resource chapters covered:** CSS-Tricks Sticky Footer (five ways → flexbox); MDN Basic concepts of flexbox; MDN flex-direction
- **Decision Gate N connection:** direct prep for Gate 4 — the Phase 12 referral project page chrome (header + content + footer) uses this primitive end-to-end.

## Prerequisites

Verify each tool works before starting:

- [ ] Browser dev tools open
- [ ] `cd round-1 && ls 07-sticky-footer.html` (empty file exists at all 3 round paths)

If any fail, fix per Phase 00 install notes before continuing.

## Estimated time

Round 1: 12 min. Round 2: 6 min. Round 3: 4 min.

## Design brief

**What to build:**

A single self-contained `.html` file with embedded `<style>` block. The `<body>` (or a single wrapper inside it) sets `min-height: 100vh` and uses `display: flex` with `flex-direction: column` to stack a header, a main content area, and a footer. The main content area takes `flex: 1` so the footer pins to the viewport bottom when content is short.

## Acceptance criteria

1. Verify the `<body>` (or a single wrapper inside it) wraps a header element, a main content element, and a footer element in `round-1/07-sticky-footer.html`.
2. Inspect the embedded `<style>` block — verify `min-height: 100vh` is set on the body (or wrapper) so the layout fills the viewport vertically.
3. Verify `display: flex` is set on the body (or wrapper) and `flex-direction` is set to `column` to stack header, main, and footer vertically.
4. Verify the main content element has `flex: 1` so the `flex-grow` portion of the shorthand pushes the footer to the bottom edge of the viewport when content is short.
5. Compare the rendered file across short, medium, and long main content — confirm the footer pins to the viewport bottom for short content and sits naturally below long content. Note the round-1, round-2, round-3 timings in lab-notes.md.
6. Note in lab-notes.md the flexbox vocabulary applied for this pattern: prefer `display: flex` on the body or wrapper; choose `flex-direction: column` to stack vertically; cover the viewport via `min-height: 100vh`; apply `flex: 1` on the main content (the `flex-grow` portion pushes the footer to the bottom edge); no `align-items` override is required because the default cross-axis stretching is what the layout wants; recognize that `justify-content`, `flex-wrap`, `flex-basis`, `flex-shrink`, `flex: 2`, `gap`, and `media query` are vocabulary reserved for other patterns and are not used here.

## Stretch goals

- Apply a contrasting background color to the footer — verify the boundary between main and footer sits at the viewport bottom for short content.
- Run the rendered file with a tall header (e.g., 200px) and confirm the main content still grows to push the footer down.

## Screenshots + Live URL deliverable

(Optional — drag round-3 .html onto Netlify Drop for a shareable preview URL.)

## Deliverable checklist

The lab is done when:

- [ ] All acceptance criteria checked across all 3 rounds
- [ ] `round-1/07-sticky-footer.html` + `round-2/07-sticky-footer.html` + `round-3/07-sticky-footer.html` all render the sticky footer
- [ ] Round 3 completion time in lab-notes.md is <60 seconds
- [ ] Lab-notes.md "What I tried that didn't work" section captures any footer-floating dead-ends from rounds 1 and 2

## Common pitfalls

- Did you set `min-height: 100vh` on the body (or wrapper)? Without it, the layout collapses to content height and the footer rides up.
- Did you set `flex-direction: column`? Without it, header / main / footer render horizontally.
- Did you set `flex: 1` on main rather than on footer? Setting it on footer pushes the footer to grow rather than pinning it.

## References

- Concept Notes 3
- [CSS-Tricks — Sticky Footer (flexbox)](https://css-tricks.com/couple-takes-sticky-footer/#There is flexbox) [sha256:623051ecb86b] 2026-05-28
- [MDN — Basic concepts of flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Flexible_box_layout/Basic_concepts#The flex container) [sha256:aef288d2d19d] 2026-05-28
- [MDN — flex-direction](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/flex-direction#Syntax) [sha256:877e3999d65f] 2026-05-28

<!-- citations-v1.1
- [CSS-Tricks — Sticky Footer (flexbox)](https://css-tricks.com/couple-takes-sticky-footer/#There is flexbox) [sha256:623051ecb86b] 2026-05-28
- [MDN — Basic concepts of flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Flexible_box_layout/Basic_concepts#The flex container) [sha256:aef288d2d19d] 2026-05-28
- [MDN — flex-direction](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/flex-direction#Syntax) [sha256:877e3999d65f] 2026-05-28
<!-- /citations-v1.1 -->

*Last updated: 2026-05-28*
