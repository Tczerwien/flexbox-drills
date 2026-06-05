# Pattern 03 — 3-Column Equal — Practice Log

**Date round 1:** _____
**Date round 2:** _____
**Date round 3:** _____
**Time spent:** _____
**Status:** Draft

---

## How to run this drill

This is a muscle-memory drill, not a one-and-done lab. Three rounds across three different days; each round you rebuild `03-three-column-equal.html` from scratch in a fresh file. Round 1 may lean on the reference; by round 3 it should be recall only, well under a minute. The timing is the deliverable — not the prose.

- [ ] Round 1 built in `round-1/03-three-column-equal.html`
- [ ] Round 2 built in `round-2/03-three-column-equal.html` (a different day)
- [ ] Round 3 built in `round-3/03-three-column-equal.html` (a different day)

---

## The target

What to build, described by how it should look and behave — recall the CSS yourself.

One outer container box wraps three sibling column boxes. The three columns sit side by side in a single horizontal row, left to right, in source order. Each column is exactly the same width as the other two, and together the three columns consume the container's full inner width. When the container is made wider or narrower, all three columns grow or shrink together and stay equal — no column has a fixed pixel width, so any leftover horizontal space is split evenly three ways.

Give each column a different fill color so the boundaries are visible, and drop some placeholder text in each. Self-verify by eye: drag the browser window narrower and confirm the three stay equal and keep filling the row.

```text
+-----------------------------------------------------+
| container                                           |
| +---------------+ +---------------+ +-------------+  |
| |   column 1    | |   column 2    | |  column 3   |  |
| |   (1/3 wide)  | |   (1/3 wide)  | |  (1/3 wide) |  |
| +---------------+ +---------------+ +-------------+  |
+-----------------------------------------------------+
   <----------- columns always equal, fill the row ---->
```

**Behavioral checks to hit by eye:**

- Three columns, one row, left to right, equal widths.
- Resize the window: the columns stay equal and keep filling the row's full width.
- Even visible breathing room between adjacent columns (no columns touching), without breaking the equal-thirds split.

**Variant target (round 2 or 3, your call):** rebuild the same idea with five sibling columns instead of three and confirm by eye that each settles to one-fifth of the row. The recall should be the same move scaled up.

---

## Properties recall (write from memory before each round)

Each round, BEFORE opening any reference, list — from memory — every CSS property this pattern needs, which element it goes on (container vs. each column), and the value each takes. Then build. Then compare your recalled list against what you actually had to use to make it work.

**Round 1 recalled before building:**

>

**Round 2 recalled before building:**

>

**Round 3 recalled before building:**

>

---

## Round log

### Round 1

**Time to three working equal columns:** _____

**Did I need the reference? Which part?**

>

**Where I hesitated, or a wrong property I reached for first:**

>

---

### Round 2

**Time to three working equal columns:** _____

**Did I need the reference? Which part?**

>

**Where I hesitated, or a wrong property I reached for first:**

>

---

### Round 3 (cold, timed)

**Time to three working equal columns:** _____

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
| 3     | <60 sec |         |

**Round-4 trigger:** if round 3 still needed Googling or a reference, add a round 4 the next day and log its time below.

>

---

## What I tried that didn't work

Wrong-property and wrong-element dead-ends from any round — including anything that produced unequal column widths, columns that wrapped or stacked instead of staying in one row, or columns that wouldn't fill the container. Name the misfire and what it did on screen, not the fix. The misfires are the signal for what to drill next.

>

---

## Gate 3 connection

Gate 3 is building a responsive layout from a sketch, fast, with no AI.

**Could I drop this three-equal-column row into a larger responsive page right now, from memory, without breaking stride?**

>

**If the brief changed so the middle column had to be twice as wide as the two outer columns, which declaration would I reach for first, and on which element?**

>

**If the brief changed so the columns had to stack vertically on a narrow phone screen and return to a row on a wide screen, what would I add — and where?**

>

*Last updated: 2026-06-05*
