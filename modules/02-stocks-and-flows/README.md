# Module 02 — Stocks & Flows

**Phase 1 · Foundations**

This is the grammar of system dynamics. Almost every system behavior you'll model reduces to
things that accumulate (stocks) and the rates that fill or drain them (flows). Get this one
into your bones and behavior-over-time graphs start reading like sentences.

## Objectives

By the end of this module you should be able to:

1. Define a **stock** as an accumulation — the system's memory — and a **flow** as a rate
   that changes a stock.
2. State the central rule: **you can only change a stock through its inflows and
   outflows**, never directly.
3. Explain how stocks create **delays** and **decouple** an inflow from an outflow, and why
   that decoupling is what makes systems stable (or sluggish).
4. Read and sketch a **behavior-over-time graph (BOTG)** for a rising, falling, or
   steady stock given its flows.

## Key concepts

- **Stock = accumulation = memory.** A stock is anything that builds up or drains down: water
  in a bathtub, money in an account, items in a backlog, headcount on a team, CO₂ in the
  atmosphere. It's the present *state* of the system, and it's the record of everything the
  flows have done so far. Stocks are what you can see and measure at a moment in time.
- **Flow = a rate.** A flow changes a stock *per unit of time*: water per minute, hires per
  quarter, tickets closed per day. Inflows raise the stock; outflows lower it. Flows are
  verbs; stocks are nouns.
- **The bathtub.** The canonical metaphor. Water level (stock) rises when the faucet
  (inflow) runs faster than the drain (outflow), falls when the drain wins, and holds steady
  when they match. You cannot change the water level by staring at it — only by adjusting a
  tap. Every stock obeys this.
- **Stocks decouple in from out.** Because a stock buffers the difference between its flows,
  the inflow and outflow don't have to match moment to moment. Inventory lets a factory ship
  steadily while producing in batches. This buffering is the source of a system's stability —
  and of its **delays**.
- **Delays.** A stock takes time to fill or drain. That lag between "turn the tap" and "level
  changes" is why systems respond slowly, overshoot, and surprise us — the theme of Module 04.
- **BOTGs.** The habit of sketching a variable against time — is it rising, falling,
  oscillating, leveling off? — before reaching for equations. The shape tells you which
  structure is at work.

## Assigned readings

- Meadows, *Thinking in Systems* — **Chapter 1**, the sections on **stocks and flows** and
  the **bathtub** examples.
- Meadows, *Thinking in Systems* — **Chapter 2, "A Brief Visit to the Systems Zoo,"** for
  the one- and two-stock systems and how their flows produce characteristic BOTGs.

See [reading-list.md](../../resources/reading-list.md) for full references. The optional
[Insight Maker](https://insightmaker.com/) tool lets you simulate the models below, but a
**pencil sketch** is all this module requires.

## Work this module in order

1. Read the assigned readings.
2. Do the [exercises](exercises.md).
3. Work the [case study](case-study.md) against a real system you've seen.
4. Answer the [self-check](self-check.md) from memory.
5. Write up your [notes](notes.md) in your own words.
6. Tick this module off in the [progress tracker](../../README.md#progress).
