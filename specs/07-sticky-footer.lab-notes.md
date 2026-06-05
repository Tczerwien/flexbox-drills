# Pattern 07 — Sticky Footer (page) — Practice Log

**Date round 1:** _____
**Date round 2:** _____
**Date round 3:** _____
**Time spent:** _____
**Status:** Draft

---

## How to run this drill

This is a muscle-memory drill, not a one-and-done lab. Three rounds across three different days; each round you rebuild `07-sticky-footer.html` from scratch in a fresh file. Round 1 may lean on the reference; by round 3 it should be recall only, under a minute. The timing is the deliverable.

- [ ] Round 1 built in `round-1/07-sticky-footer.html`
- [ ] Round 2 built in `round-2/07-sticky-footer.html` (a different day)
- [ ] Round 3 built in `round-3/07-sticky-footer.html` (a different day)

---

## The target

Build a single self-contained `.html` file (embedded `<style>` block, no external CSS) whose page chrome is a header, a main content area, and a footer stacked top-to-bottom. The behavior to hit:

- **Short content:** the footer is pinned flush against the bottom edge of the viewport — there is no blank strip below it, and you cannot scroll past it. The header sits at the top, the footer sits at the very bottom, and the thin main content floats in the band between them.
- **Long content:** when the main content is taller than the viewport, the footer is pushed down to sit naturally *below* the last line of content — you scroll the whole page and the footer arrives after everything, never overlapping or floating mid-page.

The layout fills the full height of the viewport no matter how little content is inside it. There are no responsive breakpoints for this pattern — one layout, one behavior, verified by eye at three content lengths (short / medium / long).

Rough sketch of the short-content case (footer kissing the viewport floor):

```text
+--------------------------+  <- top of viewport
|         header           |
+--------------------------+
|                          |
|     main (a little)      |
|                          |
|                          |  <- empty band absorbed here
+--------------------------+
|         footer           |
+--------------------------+  <- bottom of viewport
```

Self-verify by rendering the same file with three amounts of main content and watching where the footer lands.

---

## Properties recall (write from memory before each round)

Each round, before opening any reference, list every CSS property this pattern needs, which element each goes on (the wrapping container vs. the main region), and the value each takes. Then build, then compare against what you actually used. The recall is the skill — getting the band to collapse the empty space and the footer to ride the floor is what you are drilling cold.

**Round 1 recalled before building:**

> 

**Round 2 recalled before building:**

> 

**Round 3 recalled before building:**

> 

---

## Round log

### Round 1

**Time to a footer that pins on short content and sits below long content:** _____

**Did I need the reference? Which part?**

> 

**Where I hesitated, or a wrong property I reached for first:**

> 

---

### Round 2

**Time to a footer that pins on short content and sits below long content:** _____

**Did I need the reference? Which part?**

> 

**Where I hesitated, or a wrong property I reached for first:**

> 

---

### Round 3 (cold, timed)

**Time to a footer that pins on short content and sits below long content:** _____

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

**Round-4 trigger:** if round 3 still needed Googling or a reference, or the footer floated mid-page on the first try, add a round 4 the next day and log its time below.

> 

---

## What I tried that didn't work

Wrong-property dead-ends from any round — especially any attempt where the footer rode up into the empty band, or where the chrome rendered side-by-side instead of stacked, or where the page collapsed to content height and lost the floor. Name what you reached for and what the render actually did. The misfires are the signal for what to drill next.

> 

---

## Gate 4 connection

The Phase 12 referral project page chrome (header + content + footer) is this primitive end-to-end.

**Could I drop this header/main/footer page shell into the referral project right now, from memory, without breaking stride?**

> 

**If the footer had to instead sit immediately under short content (no longer pinned to the viewport floor), which single piece of the recipe would I drop or change first?**

> 

*Last updated: 2026-06-05*
