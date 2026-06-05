# Pattern 01 — Center Child — Practice Log

**Date round 1:** _____
**Date round 2:** _____
**Date round 3:** _____
**Time spent:** _____
**Status:** Draft

---

## How to run this drill

This is a muscle-memory drill, not a one-and-done lab. Three rounds spaced across three different days; each round you rebuild `01-center-child.html` from scratch in a fresh file, with one container and one child. Round 1 may lean on the reference; by round 3 it should be recall only, under 30 seconds, with nothing open. The timing is the deliverable — log it honestly each round.

- [ ] Round 1 built in `round-1/01-center-child.html`
- [ ] Round 2 built in `round-2/01-center-child.html` (a different day)
- [ ] Round 3 built in `round-3/01-center-child.html` (a different day)

---

## The target

What you are building, so you can self-verify by eye — figure out the rules that get you there.

- One container wrapping one child.
- The container fills the whole height of the browser window, top to bottom, even when the child is small.
- The child sits dead center: the same gap on the left as on the right, and the same gap above as below.
- Resize the window and the child stays centered — no scrollbar appears just from the empty space around it.
- It survives a narrow phone width, a tablet width, and a wide desktop width with no extra rules added for each — the same single approach holds at every width (sanity-check it at roughly 320px, 768px, and 1280px in the device emulator).

A rough sketch of the win condition:

```
+----------------------------------+  <- top of the window
|                                  |
|                                  |
|              +------+            |
|              | child|            |
|              +------+            |
|                                  |
|                                  |
+----------------------------------+  <- bottom of the window
        equal gaps on all four sides
```

---

## Properties recall (write from memory before each round)

Each round, before opening any reference, list the CSS properties this pattern needs and the value each takes. Then build, then compare against what you actually used. The gap between what you could recall and what you actually needed is the thing this drill is closing.

**Round 1 recalled before building:**

> 

**Round 2 recalled before building:**

> 

**Round 3 recalled before building:**

> 

---

## Round log

### Round 1

**Time to a working centered child:** _____

**Did I need the reference? Which part?**

> 

**Where I hesitated, or a wrong property I reached for first:**

> 

---

### Round 2

**Time to a working centered child:** _____

**Did I need the reference? Which part?**

> 

**Where I hesitated, or a wrong property I reached for first:**

> 

---

### Round 3 (cold, timed)

**Time to a working centered child:** _____

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

**Round-4 trigger:** if round 3 still needed Googling or a reference, or ran over 60 seconds, add a round 4 the next day and log its time below.

> 

---

## What I tried that didn't work

Wrong-property dead-ends from any round — the rules you reached for that left the child off-center, stuck to one edge, or the container too short. Note what you saw on screen and what you switched to. The misfires are the signal for what to drill next; don't paste the fix you landed on, just name where it went sideways.

> 

---

## Gate 3 connection

**Could I drop this centered-child pattern into a larger responsive layout right now, from memory, without breaking stride?**

> 

**If the child had to sit pinned to the bottom edge of the container instead of dead center, what would I reach for, and which of the rules I used here would stay the same?**

> 

*Last updated: 2026-06-05*
