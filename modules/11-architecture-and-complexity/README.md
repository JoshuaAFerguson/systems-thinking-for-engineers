# Module 11 — Architecture & Complexity

**Phase 3 · Technical applications**

Now the tools meet code. This module treats a codebase as a system: technical debt is a
*stock*, coupling is *interconnection density*, and complexity is *emergent*. The reinforcing
loops you drew back in Module 03 explain why architectures rot — and where you can intervene.

## Objectives

By the end of this module you should be able to:

1. Model **technical debt as a stock**, driven by an inflow of shortcuts and an outflow of
   deliberate paydown — and explain why "we'll clean it up later" almost never happens on its own.
2. Describe **coupling as interconnection density** and reason about how it changes a system's
   behavior over time, not just its diagram.
3. Explain why **complexity is emergent** — it lives in the interactions between modules, not
   inside any one of them — and why that makes it invisible in code review.
4. Identify a **reinforcing loop of decay** in a real codebase, and name a **balancing loop**
   that could counter it before it runs away.

## Key concepts

- **Technical debt is a stock, not an event.** Using the stock-and-flow vocabulary from
  Module 02: debt *accumulates* through an inflow of shortcuts (skipped tests, copy-paste,
  "temporary" hacks) and only *drains* through a deliberate outflow of paydown (refactoring,
  deletion, tests added). Left alone, the stock only rises — because there's an inflow by
  default and no outflow by default.
- **Debt charges interest, and interest is a reinforcing loop.** A high debt stock makes every
  future change slower and riskier, which pressures people to take *more* shortcuts to hit the
  same deadline, which raises the stock further. That's the R1 loop from Module 03: harder to
  change → more shortcuts → harder to change. It compounds.
- **Coupling is interconnection density.** In Module 00's vocabulary, behavior lives in the
  *interconnections*. Tight coupling means a change in one element propagates to many others.
  You can't see coupling in a single file — you see it when a "one-line change" turns into a
  three-day change touching nine modules.
- **Complexity is emergent.** No module "contains" the complexity; it emerges from how modules
  interact — shared state, hidden dependencies, temporal ordering. Ousterhout's two symptoms —
  *change amplification* and *cognitive load* — are system-level properties, which is exactly
  why they slip past a file-at-a-time review.
- **Decay is a system trap, not a moral failing.** The reinforcing loop runs on its own. Blaming
  "sloppy engineers" is the linear story; the systemic story is that the structure rewards
  shortcuts and doesn't fund paydown. The fix is structural: change the flows, not the people.
- **Balancing loops are the brakes.** A refactoring budget, a "boy-scout rule," a complexity
  ceiling that blocks merges, an architecture fitness function — each is a balancing loop that
  pushes the debt stock back down toward a tolerable level.

## Assigned readings

- Meadows, *Thinking in Systems* — re-read the **stocks and flows** material (Ch. 1) and the
  **reinforcing loop** sections, this time reading "stock" as *technical debt* and "reinforcing
  loop" as *decay*.
- John Ousterhout, *A Philosophy of Software Design* — the chapters on **complexity** (its
  definition, symptoms, and causes: dependencies and obscurity).
- Forsgren, Humble & Kim, *Accelerate* — the material on **architecture, maintainability, and
  loosely coupled systems** as predictors of delivery performance.

See [reading-list.md](../../resources/reading-list.md) for full references.

## Work this module in order

1. Read the assigned readings.
2. Do the [exercises](exercises.md).
3. Work the [case study](case-study.md) against a real codebase you know.
4. Answer the [self-check](self-check.md) from memory.
5. Write up your [notes](notes.md) in your own words.
6. Tick this module off in the [progress tracker](../../README.md#progress).
