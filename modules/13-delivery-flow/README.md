# Module 13 — Delivery Flow

**Phase 3 · Technical applications**

Work is a *flow* through *queues* — and queues are invisible stocks. This module gives you the
quantitative side of that intuition: Little's Law relates work-in-progress, throughput, and lead
time; the Theory of Constraints tells you that only one thing sets the pace, so optimizing
anything else is wasted effort. This is Module 02's stocks-and-flows made measurable.

## Objectives

By the end of this module you should be able to:

1. See a delivery pipeline as **work flowing through queues**, and recognize each queue as an
   invisible **stock** (a PR backlog, a ticket column, a deploy queue).
2. Apply **Little's Law** (L = λW): work-in-progress = throughput × lead time. Given any two,
   derive the third — and use it to predict how WIP changes lead time.
3. Use the **Theory of Constraints** five focusing steps — identify → exploit → subordinate →
   elevate → repeat — to find and relieve the one bottleneck that sets a system's pace.
4. Explain why **high WIP and large batch size** lengthen lead time and hide problems, and why
   limiting WIP is a leverage point (Module 08).

## Key concepts

- **Queues are invisible stocks.** In Module 02 a stock was a bathtub; here the bathtub is a
  queue of unfinished work — the PRs awaiting review, the tickets in "ready," the changes waiting
  to deploy. You can't manage what you don't see, and queues are the least-visible, most costly
  part of most pipelines (Reinertsen's central point).
- **Little's Law: L = λW.** For any stable queue, the average work-in-progress **L** equals the
  average arrival/throughput rate **λ** times the average time-in-system **W**. Rearranged:
  `lead time = WIP / throughput`. It's arithmetic, not opinion — if WIP doubles and throughput
  holds, lead time doubles. Measure any two of the three and you get the third.
- **The Theory of Constraints: one thing sets the pace.** Goldratt's insight is that a system's
  throughput is governed by a single **constraint** (the bottleneck). Improving any non-bottleneck
  step produces *no* system improvement — it just piles inventory in front of the constraint. The
  five focusing steps: **identify** the constraint, **exploit** it (waste none of its capacity),
  **subordinate** everything else to it, **elevate** it (add capacity), then **repeat** because
  the constraint moves.
- **High WIP is a false economy.** Starting more work feels productive but, by Little's Law, more
  WIP means longer lead times — each item waits behind more other items. High WIP also *hides*
  problems (a defect sits undiscovered in a long queue) and raises context-switching cost.
- **Large batches lengthen everything.** Big releases, long-lived branches, and quarterly
  deploys increase the queue's residence time, delay feedback, and make failures harder to
  localize. Small batches shorten the feedback loops that *Accelerate* ties to delivery
  performance.
- **WIP limits are a leverage point.** Capping WIP (Module 08's "rules of the system" / "flows")
  is a small structural change with outsized effect: it forces finishing over starting, surfaces
  the constraint, and pulls lead time down without anyone working faster.

## Assigned readings

- Eliyahu Goldratt, *The Goal* — the **Theory of Constraints** and the five focusing steps, in
  novel form. Watch the plant's bottleneck (the "Herbie" chapter) as the model for your pipeline.
- Gene Kim et al., *The Phoenix Project* — the same ideas ported to IT/software delivery; the
  "four types of work" and the WIP problem.
- Donald Reinertsen, *The Principles of Product Development Flow* — **queues, WIP, batch size,
  and Little's Law**. The rigorous case for managing invisible queues.
- Forsgren, Humble & Kim, *Accelerate* — **small batch size, short lead time, and fast feedback**
  as measured drivers of performance.

See [reading-list.md](../../resources/reading-list.md) for full references.

## Work this module in order

1. Read the assigned readings.
2. Do the [exercises](exercises.md).
3. Work the [case study](case-study.md) against a real delivery pipeline you've worked in.
4. Answer the [self-check](self-check.md) from memory.
5. Write up your [notes](notes.md) in your own words.
6. Tick this module off in the [progress tracker](../../README.md#progress).
