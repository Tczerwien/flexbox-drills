# Pattern 04 — Three-Column Unequal (middle 2× wider) — Practice Log

**Date round 1:** _____
**Date round 2:** _____
**Date round 3:** _____
**Time spent:** _____
**Status:** Draft

---

## How to run this drill

This is a muscle-memory drill, not a one-and-done lab. Three rounds across three different days; each round you rebuild `04-three-column-unequal.html` from scratch in a fresh file. Round 1 may lean on the reference; by round 3 it should be recall only, under 30 seconds. The timing is the deliverable.

- [ ] Round 1 built in `round-1/04-three-column-unequal.html` (today)
- [ ] Round 2 built in `round-2/04-three-column-unequal.html` (a different day)
- [ ] Round 3 built in `round-3/04-three-column-unequal.html` (a different day)

---

## The target

What to build, described by how it looks and behaves — not by which rules produce it. You build it, then eyeball it against this picture to self-verify.

One outer box holds three side-by-side child boxes. The two outer children are the same width as each other. The middle child is **twice as wide** as either outer child — so the three widths read as a 1 : 2 : 1 split, and together they fill the full width of the outer box with no empty strip left over on either end.

```
+--------------------------------------------------+
|            |                        |            |
|   left     |        middle          |   right    |
|  (narrow)  |   (twice as wide)      |  (narrow)  |
|            |                        |            |
+--------------------------------------------------+
   ^ 1 unit         ^ 2 units            ^ 1 unit
```

Behavior to confirm by eye in the browser:

- The three children sit in one horizontal row, left-to-right, in the same sequence they appear in the HTML.
- The middle column is visibly double the width of each flank — hold a finger to the screen: two lefts stacked side by side should match the middle.
- The row spans the entire outer box edge-to-edge; the right flank's right edge touches the outer box's right edge.
- Give each child a distinct background color so the three bands and their proportions are obvious at a glance.

**Self-check (no tooling needed):** if the middle looks the same width as a flank, or wider/narrower than exactly-double, the proportion rule is off. If one flank is fatter than the other, the two flanks aren't sharing equally.

### Stretch variation (optional, after round 3)

- Push the middle from "twice as wide" to "three times as wide" as a flank (a 1 : 3 : 1 read, middle = three-fifths of the box). Confirm the middle visibly grows and the flanks shrink to match.
- Shrink the browser to a phone-narrow width and note whether the proportions still read cleanly or collapse.

---

## Properties recall (write from memory before each round)

Each round, before opening any reference, list every CSS property this pattern needs and the value each one takes — the one that turns the outer box into a row, and the ones that set the three children's width shares. Then build, then compare against what you actually used.

**Round 1 recalled before building:**

>

**Round 2 recalled before building:**

>

**Round 3 recalled before building:**

>

---

## Round log

### Round 1

**Time to a working 1 : 2 : 1 row:** _____

**Did I need the reference? Which part?**

>

**Where I hesitated, or a wrong property I reached for first:**

>

---

### Round 2

**Time to a working 1 : 2 : 1 row:** _____

**Did I need the reference? Which part?**

>

**Where I hesitated, or a wrong property I reached for first:**

>

---

### Round 3 (cold, timed)

**Time to a working 1 : 2 : 1 row:** _____

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

Wrong-property dead-ends and proportion-math misfires from any round — e.g., the row came out as equal thirds, or the children stacked vertically instead of sitting in a row, or the middle landed at some ratio other than exactly double. Write what you reached for and what the browser actually showed. The misfires are the signal for what to drill next.

>

---

## Gate 3 connection

**Could I drop this unequal three-column row into a larger responsive Tailwind layout right now, from memory, without breaking stride — pinning a wide center reading column between two narrower side rails?**

>

**If the brief changed so the middle had to be three times a flank instead of twice, which single value would I change, and would I touch the flanks at all?**

>

*Last updated: 2026-06-05*
