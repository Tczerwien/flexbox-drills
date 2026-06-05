# Pattern 06 — Responsive Grid — Practice Log

**Date round 1:** _____
**Date round 2:** _____
**Date round 3:** _____
**Time spent:** _____
**Status:** Draft

---

## How to run this drill

This is a muscle-memory drill, not a one-and-done lab. Three rounds across three different days; each round you rebuild `06-responsive-grid.html` from scratch in a fresh file. Round 1 may lean on the reference; by round 3 it should be recall only, under 60 seconds. The timing is the deliverable.

- [ ] Round 1 built in `round-1/06-responsive-grid.html`
- [ ] Round 2 built in `round-2/06-responsive-grid.html` (a different day)
- [ ] Round 3 built in `round-3/06-responsive-grid.html` (a different day)

---

## The target

One container holds a row of identical cards (start with four or more). The cards arrange themselves left-to-right, and when there is not enough room for the next card on the current row, the leftover cards drop down to start a new row underneath. Build a single self-contained `.html` file with one container element wrapping several card elements; size the cards so the layout settles into three different shapes as the viewport narrows:

- **Wide / desktop (~1280px):** four cards sit side by side on each row.
- **Medium / tablet (~768px):** the layout collapses to two cards per row.
- **Narrow / mobile (~320px):** each card takes the whole width, one card per row, stacked.

Self-verify visually by dragging the browser window (or the dev-tools responsive ruler) through 320px → 768px → 1280px and confirming the 1-, 2-, and 4-across shapes each appear cleanly with no card overflowing or compressing past its intended share.

```text
desktop (~1280px)          tablet (~768px)     mobile (~320px)
+----+----+----+----+      +------+------+      +-------------+
| 1  | 2  | 3  | 4  |      |  1   |  2   |      |     1       |
+----+----+----+----+      +------+------+      +-------------+
| 5  | 6  | 7  | 8  |      |  3   |  4   |      |     2       |
+----+----+----+----+      +------+------+      +-------------+
                           |  5   |  6   |      |     3       |
                           +------+------+      +-------------+
                                                |    ...      |
                                                +-------------+
```

The card count and content are GIVEN — what you must produce from memory is the styling that makes the cards line up, allow the rows to break, claim the right share of width at each size, and re-claim a different share at the two narrower sizes.

---

## Properties recall (write from memory before each round)

Each round, before opening any reference, list — from memory — every styling declaration this pattern needs: what makes the container lay its children out in a row, what lets the rows break instead of staying jammed on one line, what governs how much of the row each card claims, and the two width-share switches that retarget the cards at the tablet and mobile sizes. Name each property and the value it takes. Then build, then compare against what you actually used.

**Round 1 recalled before building:**

> 

**Round 2 recalled before building:**

> 

**Round 3 recalled before building:**

> 

---

## Round log

### Round 1

**Time to a working 4-→2-→1-across grid:** _____

**Did I need the reference? Which part?**

> 

**Where I hesitated, or a wrong property I reached for first:**

> 

---

### Round 2

**Time to a working 4-→2-→1-across grid:** _____

**Did I need the reference? Which part?**

> 

**Where I hesitated, or a wrong property I reached for first:**

> 

---

### Round 3 (cold, timed)

**Time to a working 4-→2-→1-across grid:** _____

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

**Round-4 trigger:** if round 3 still needed Googling or a reference, or the breakpoints didn't land on the first try, add a round 4 the next day and log its time below.

> 

---

## What I tried that didn't work

Wrong-property dead-ends and breakpoint misfires from any round — the card that wouldn't drop to the next row, the size that came out wider or narrower than the share you intended, the breakpoint that produced only a two-tier shape instead of three, or a sizing approach that fought the row layout. Note what you reached for and what the rendered grid actually did. The misfires are the signal for what to drill next.

> 

---

## Gate 3 connection

**Could I drop this responsive card-grid pattern into a larger Tailwind page from a sketch right now, from memory, without breaking stride?**

> 

**If the brief changed so the cards sat three per row at desktop instead of four (tablet and mobile unchanged), which declarations would I touch, and which would stay exactly as they are?**

> 

*Last updated: 2026-06-05*
