# flexbox-drills

*Phase 07 Frontend Fundamentals — 7 flexbox layout patterns, 3 reps each.*

**Status:** building — Scaffolded for Phase 07; content lands during execution.

<!-- WRITE during Phase 07: 1-sentence description of which 7 patterns these drills cover, in your own voice. -->

## What's here

<!-- WRITE during Phase 07: a bulleted list of the 7 patterns as their .html files
     land, formatted `NN-pattern-slug.html — one-line layout description`.
     Files use the `NN-pattern-slug.html` naming convention per CLAUDE.md. Each
     pattern is one self-contained HTML file with an embedded <style> block — no
     external CSS, no Tailwind (that's Phase 09). -->

## Pattern specs

| #  | Pattern title              | What it demonstrates                                             | Spec                                  | Concept Notes |
|----|----------------------------|------------------------------------------------------------------|---------------------------------------|---------------|
| 01 | Center child               | `display: flex; justify-content: center; align-items: center;`   | [./specs/01-center-child.md](./specs/01-center-child.md)               | 3             |
| 02 | Navbar                     | `justify-content: space-between; align-items: center;`           | [./specs/02-navbar.md](./specs/02-navbar.md)                     | 3             |
| 03 | 3-column equal             | 3 siblings, each `flex: 1`                                       | [./specs/03-three-column-equal.md](./specs/03-three-column-equal.md)         | 3             |
| 04 | 3-column unequal           | first+last `flex: 1`, middle `flex: 2`                           | [./specs/04-three-column-unequal.md](./specs/04-three-column-unequal.md)       | 3             |
| 05 | Card with footer pinned    | `flex-direction: column` + middle `flex: 1` + footer at bottom   | [./specs/05-card-with-footer.md](./specs/05-card-with-footer.md)           | 3             |
| 06 | Responsive grid            | `flex-wrap: wrap` + `flex-basis` + media queries                 | [./specs/06-responsive-grid.md](./specs/06-responsive-grid.md)            | 3             |
| 07 | Sticky footer (page)       | body `min-height: 100vh; display: flex; flex-direction: column;` | [./specs/07-sticky-footer.md](./specs/07-sticky-footer.md)              | 3             |

## Round cross-tab

Each pattern is built 3 times across 3 different days (round-1 → round-2 → round-3) for muscle-memory development. Round 1: 12 min target. Round 2: 6 min. Round 3: 4 min (canonical center pattern → 30 sec target).

| #  | Pattern              | Round 1                                  | Round 2                                  | Round 3                                  | Live URL (Netlify Drop) |
|----|----------------------|------------------------------------------|------------------------------------------|------------------------------------------|-------------------------|
| 01 | Center child         | ./round-1/01-center-child.html           | ./round-2/01-center-child.html           | ./round-3/01-center-child.html           | _____                   |
| 02 | Navbar               | ./round-1/02-navbar.html                 | ./round-2/02-navbar.html                 | ./round-3/02-navbar.html                 | _____                   |
| 03 | 3-column equal       | ./round-1/03-three-column-equal.html     | ./round-2/03-three-column-equal.html     | ./round-3/03-three-column-equal.html     | _____                   |
| 04 | 3-column unequal     | ./round-1/04-three-column-unequal.html   | ./round-2/04-three-column-unequal.html   | ./round-3/04-three-column-unequal.html   | _____                   |
| 05 | Card with footer     | ./round-1/05-card-with-footer.html       | ./round-2/05-card-with-footer.html       | ./round-3/05-card-with-footer.html       | _____                   |
| 06 | Responsive grid      | ./round-1/06-responsive-grid.html        | ./round-2/06-responsive-grid.html        | ./round-3/06-responsive-grid.html        | _____                   |
| 07 | Sticky footer (page) | ./round-1/07-sticky-footer.html          | ./round-2/07-sticky-footer.html          | ./round-3/07-sticky-footer.html          | _____                   |

Live URLs: drag the round-3 .html files onto [Netlify Drop](https://app.netlify.com/drop) for a free no-signup preview link once each pattern is built.

## How this maps to the plan

See `_MASTER-PLAN/phase-07-frontend-fundamentals/03-FrontendFundamentals_deliverables.md`
for the canonical pattern inventory and acceptance criteria.

*Note: the `Fontend` filename typo is canonical per Phase 1 HYG-08 ratification —
do not "correct" it.*

## About

<!-- WRITE during Phase 07: 1-sentence "About me" line + link to GitHub profile, per
     CLAUDE.md README Conventions (Repo-Level). -->

---
*Scaffolded via GSD Phase 4. Pattern specs + round files added via GSD Phase 14. Content lands during Phase 07 execution.*
