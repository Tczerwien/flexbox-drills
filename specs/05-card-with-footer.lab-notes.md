# Pattern 05 — Card With Footer Pinned — Practice Log

**Date round 1:** _____
**Date round 2:** _____
**Date round 3:** _____
**Time spent:** _____
**Status:** Draft

---

## How to run this drill

This is a muscle-memory drill, not a one-and-done lab. Three rounds across three different days; each round you rebuild `05-card-with-footer.html` from scratch in a fresh file. Round 1 may lean on the reference; by round 3 it should be recall only, under 30 seconds. The timing is the deliverable.

- [ ] Round 1 built in `round-1/05-card-with-footer.html`
- [ ] Round 2 built in `round-2/05-card-with-footer.html` (a different day)
- [ ] Round 3 built in `round-3/05-card-with-footer.html` (a different day)

---

## The target

A single self-contained `.html` file with an embedded `<style>` block. One card box wraps three stacked sections — a header strip at the top, a middle content area, and a footer strip at the bottom. The three sections sit one above the other (not side by side). The card has a fixed overall height (or fills the page when the card is the page itself).

The behavior that defines this pattern: the footer hugs the bottom edge of the card no matter how tall or short the middle content is. Feed the middle area one short word and the footer sits at the bottom; feed it several paragraphs and the footer is still flush against the bottom edge. The middle area absorbs all the leftover vertical room between header and footer.

Give the header and footer a contrasting background from the middle so you can see, by eye, that the footer's top edge meets the bottom slab of the card and never floats up into empty space.

Sketch of the goal:

```
+---------------------------+   <- top of card
|         header            |
+---------------------------+
|                           |
|   middle (any height —    |
|   absorbs the leftover    |
|   room, short or tall)    |
|                           |
+---------------------------+
|         footer            |
+---------------------------+   <- bottom of card / page
```

Self-verify visually: resize the middle content text from one word to many lines and confirm the footer never lifts off the bottom edge.

---

## Properties recall (write from memory before each round)

Each round, before opening any reference, list every property this pattern needs and the value each takes — for the card box and for each of the three sections. Then build, then compare against what you actually used. Naming them cold is the whole skill; the slots stay empty until you fill them by hand.

**Round 1 recalled before building:**

> 

**Round 2 recalled before building:**

> 

**Round 3 recalled before building:**

> 

---

## Round log

### Round 1

**Time to a card with the footer pinned to the bottom edge:** _____

**Did I need the reference? Which part?**

> 

**Where I hesitated, or a wrong property I reached for first:**

> 

---

### Round 2

**Time to a card with the footer pinned to the bottom edge:** _____

**Did I need the reference? Which part?**

> 

**Where I hesitated, or a wrong property I reached for first:**

> 

---

### Round 3 (cold, timed)

**Time to a card with the footer pinned to the bottom edge:** _____

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

Wrong-property dead-ends from any round — especially any version where the footer floated up into empty space instead of pinning to the bottom edge. Note which box you put the leftover-room property on and what the footer did as a result. The misfires are the signal for what to drill next.

> 

---

## Gate 3 connection

**Could I drop this card-with-pinned-footer pattern into a larger responsive layout right now, from memory, without breaking stride?**

> 

**If the design called for the footer to sit directly under the middle content (riding up with short content) instead of pinned to the card's bottom edge, what would I change, and on which box?**

> 

*Last updated: 2026-06-05*
