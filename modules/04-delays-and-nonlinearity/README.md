# Module 04 — Delays & Nonlinearity

**Phase 1 · Foundations**

Loops explain direction; delays and nonlinearity explain the drama. A balancing loop with a
long delay doesn't settle gently — it oscillates. A reinforcing loop that hits a limit
doesn't grow forever — it overshoots and crashes. This module is about why systems surprise
even the people running them.

## Objectives

By the end of this module you should be able to:

1. Explain why a **delay** in a balancing feedback loop causes **oscillation** and
   **overshoot** instead of smooth settling.
2. Describe the **overshoot-and-collapse** pattern and the conditions that produce it (a
   reinforcing loop, a limit, and a delay in perceiving the limit).
3. Distinguish **exponential growth** from an **S-curve**, and explain what bends the curve
   over.
4. Define **nonlinearity** — response not proportional to input — and connect **bounded
   rationality** to why capable people still steer systems into trouble.

## Key concepts

- **Delays change everything.** A stock takes time to respond, and information about a stock
  takes time to arrive and be acted on. Put a delay inside a balancing loop and the corrective
  action keeps arriving *late*: you overcorrect, then overcorrect the other way. The result is
  oscillation around the goal instead of a smooth approach.
- **The Beer Game.** The classic supply-chain simulation (from Sterman / the MIT tradition):
  a chain of players each ordering to refill inventory, with shipping and ordering delays.
  Small changes in customer demand get amplified into wild swings up and down the chain — the
  **bullwhip effect** — purely because of the delays. No villain required; the *structure*
  oscillates.
- **Overshoot and collapse.** When a reinforcing loop drives growth against a limit, *and*
  there's a delay in sensing the limit (or the limit itself is erodible), the system sails
  past what it can sustain and then falls hard — instead of leveling off. Overloading a
  system past a resource it degrades is the recipe.
- **Growth shapes.** Pure exponential growth (constant reinforcing loop) is unsustainable in
  any real environment. Real growth usually traces an **S-curve (logistic)**: reinforcing
  early, then a balancing loop (a carrying capacity, saturation, cost) bends it into a
  plateau. Which curve you're on determines whether "more of the same" is wise.
- **Nonlinearity.** In a nonlinear relationship, doubling the input doesn't double the output
  — it might barely move it, or it might blow past a threshold. Nonlinearities are why loops
  change dominance, why "one more request" tips a healthy service into collapse, and why
  responses have knees and cliffs rather than straight lines.
- **Bounded rationality.** Meadows' explanation for why systems surprise us: each actor makes
  reasonable decisions on the limited, delayed, local information they actually have. Put
  rational actors in a badly structured system with delays and they will still produce
  bullwhips, bubbles, and tragedies. The fix is usually the *structure*, not the people.

## Assigned readings

- Meadows, *Thinking in Systems* — **Chapter 2**, the two-stock systems and the effect of
  **delays** on oscillation.
- Meadows, *Thinking in Systems* — the **"Why Systems Surprise Us"** material (bounded
  rationality, nonlinearity, delays, and the limits of our mental models).

See [reading-list.md](../../resources/reading-list.md) for full references.
[Insight Maker](https://insightmaker.com/) or [LOOPY](https://ncase.me/loopy/) both let you
add a delay to a loop and watch it start to oscillate.

## Work this module in order

1. Read the assigned readings.
2. Do the [exercises](exercises.md).
3. Work the [case study](case-study.md) against a real system you've seen.
4. Answer the [self-check](self-check.md) from memory.
5. Write up your [notes](notes.md) in your own words.
6. Tick this module off in the [progress tracker](../../README.md#progress).
