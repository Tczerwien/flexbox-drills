# Pattern 02 — Navbar — Practice Log

**Date round 1:** _____
**Date round 2:** _____
**Date round 3:** _____
**Time spent:** _____
**Status:** Draft

---

## How to run this drill

This is a muscle-memory drill, not a one-and-done lab. Three rounds across three different days; each round you rebuild `02-navbar.html` from scratch in a fresh file. Round 1 may lean on the reference; by round 3 it should be recall only, under 30 seconds. The timing is the deliverable.

- [ ] Round 1 built in `round-1/02-navbar.html`
- [ ] Round 2 built in `round-2/02-navbar.html` (a different day)
- [ ] Round 3 built in `round-3/02-navbar.html` (a different day)

---

## The target

Build a single self-contained `.html` file with an embedded `<style>` block. One `<nav>` element wraps two things: a logo on the one side, and a short list of nav links on the other. When it renders, the layout looks like this:

```
+--------------------------------------------------------------+
|                                                              |
|  LOGO                          Home    About    Contact      |
|                                                              |
+--------------------------------------------------------------+
```

Behavior to hit:

- The logo sits hard against the inner left edge; the link group sits hard against the inner right edge. The empty space all collects in the middle between them — it is not split into the outer edges.
- The logo and every link share one horizontal midline: nothing rides high or low, they all line up across the vertical center of the bar.
- There is breathing room on the inner left and right so neither the logo nor the last link kisses the bar's outer edge.
- The links in the right-side group are spaced apart from one another by an even, consistent amount of room — and that room should NOT pile up or double at the ends of the group.

**Responsive behavior (the breakpoint):** when the viewport gets narrow (roughly below a small-phone width), the bar reflows so the logo and the links stack on top of one another in a single vertical stack instead of sitting side by side, and the stacked layout still renders cleanly with no overflow. Above that width it returns to the single-line side-by-side shape. You decide the exact width to flip at and the mechanism that flips it.

Self-verify visually: resize the browser across the breakpoint, and try the bar once with 3 links and once with 5 links — the logo must stay pinned left and the links pinned right in both shapes.

---

## Properties recall (write from memory before each round)

Each round, before opening any reference, list — from memory — every CSS property this pattern needs and the value each one takes for the target above. Then build, then compare what you wrote against what you actually had to use. The difference between the two is the drill.

**Round 1 recalled before building:**

> 

**Round 2 recalled before building:**

> 

**Round 3 recalled before building:**

> 

---

## Round log

### Round 1

**Time to a working navbar:** _____

**Did I need the reference? Which part?**

> 

**Where I hesitated, or a wrong property I reached for first:**

> 

---

### Round 2

**Time to a working navbar:** _____

**Did I need the reference? Which part?**

> 

**Where I hesitated, or a wrong property I reached for first:**

> 

---

### Round 3 (cold, timed)

**Time to a working navbar:** _____

**Built with no notes open?**

> 

**Where I hesitated, or a wrong property I reached for first:**

> 

---

## Timing summary

| Round | Target  | My time |
|-------|---------|---------|
| 1     | ~12 min |         |
| 2     | ~6 min  |         |
| 3     | <30 sec |         |

**Round-4 trigger:** if round 3 still needed Googling or a reference, add a round 4 the next day and log its time below.

> 

---

## What I tried that didn't work

Wrong-property and wrong-value dead-ends from any round — especially anything about how the empty space between logo and links got distributed, how the links got spaced from each other, or how the vertical alignment landed. Note what you reached for and why it looked wrong on screen, not the fix. The misfires are the signal for what to drill next.

> 

---

## Gate 3 connection

**Could I drop this navbar pattern into a larger responsive page right now, from memory, without breaking stride — and make it reflow at the breakpoint?**

> 

**If the design changed so the link group had to sit in the dead center of the bar instead of pinned to the right edge, which single property would I change first, and to what?**

> 

*Last updated: 2026-06-05*
