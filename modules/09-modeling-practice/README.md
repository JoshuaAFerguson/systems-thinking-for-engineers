# Module 09 — Modeling Practice

**Phase 2 · Tools & Patterns**

So far the diagrams have been qualitative. This module makes one *runnable*. You'll take a mental
model, make its stocks, flows, and feedback explicit, put numbers on it, and simulate it forward in
time — then compare the output to reality and learn from the gap. The goal is not prediction. A
model earns its keep by producing **insight**: showing you a behavior your intuition missed.

## Objectives

By the end of this module you should be able to:

1. Turn an informal mental model into an explicit stock-and-flow model with feedback.
2. Run the **modeling loop**: define purpose → identify stocks/flows/feedback → parameterize →
   simulate → compare to reality → learn → revise.
3. Simulate the model (in a tool or in code), vary one parameter, and read the resulting change in
   behavior over time.
4. State plainly what your model is *for* and where it stops being trustworthy — models are for
   insight, not forecasting.

## Key concepts

- **A model is a purpose-built simplification.** Before touching a tool, write one sentence: *what
  question is this model meant to answer?* The purpose decides the boundary — what's a stock,
  what's a flow, what's left outside as an assumption.
- **Stocks and flows, made runnable.** A stock accumulates; flows change it. In discrete time the
  engine is just: `stock(t+dt) = stock(t) + (inflow − outflow) · dt`. Everything else is deciding
  what the inflow and outflow *depend on* — and that's where feedback enters.
- **Feedback closes the loop.** The moment a flow depends on the stock it feeds (churn depends on
  the customer count; hiring rate depends on the backlog), you have a loop, and the behavior stops
  being a straight line. This is why you simulate instead of solving in your head.
- **The modeling loop is iterative.** First run is always wrong. You compare its behavior-over-time
  to what you've actually seen, find where they diverge, and ask what missing structure explains
  the gap. The learning is in the *comparison*, not the first output.
- **Models are for insight, not prediction.** Sterman's line: all models are wrong; some are
  useful. A good model surprises you, sharpens a question, or kills a bad intuition. Treating its
  numbers as a forecast is the classic misuse.
- **Parameter sweeps reveal structure.** Change one input, hold the rest, and watch the behavior
  mode shift — smooth growth to oscillation, convergence to overshoot. The *shape* of the response
  teaches more than any single run.

A minimal worked example you can build: **SaaS customers.** One stock (`customers`), one inflow
(`signups`), one outflow (`churn = customers × churn_rate`). Because churn depends on the stock, the
system approaches an equilibrium at `signups / churn_rate` — a balancing loop you can *see* by
simulating. Vary `churn_rate` and watch the ceiling move. Other good small builds: a **support
backlog** (arrivals in, resolutions out, with resolution rate depending on backlog-driven staffing)
or **tech-debt accumulation** (debt added per feature vs. debt paid down, with velocity falling as
debt rises — a reinforcing trap).

## Assigned readings

- Meadows, *Thinking in Systems* — **Chapters 1–2** for the stock/flow/feedback structure you're
  making runnable. Re-skim if it's gone fuzzy.
- Sterman, *Business Dynamics* — **light skim only.** Read the modeling-process overview (the
  iterative modeling loop) and his "all models are wrong, some are useful" framing. Don't attempt
  the whole book; borrow its discipline, not its depth.

## Tools (pick one)

- **[Insight Maker](https://insightmaker.com/)** — free, browser-based stock-and-flow simulation.
  Fastest path to a running model with no install.
- **[Vensim PLE](https://vensim.com/free-download/)** — free for personal use; more powerful, a
  steeper start.
- **Python** — if you'd rather model in code: plain NumPy/Matplotlib for the discrete-time loop,
  or [PySD](https://pysd.readthedocs.io/) / [BPTK-Py](https://bptk.transentis.com/) for
  system-dynamics-style models. Commit the notebook or script into the module.

See [reading-list.md](../../resources/reading-list.md) for full references.

## Work this module in order

1. Read the assigned readings.
2. Do the [exercises](exercises.md) — this is where you build the model.
3. Work the [case study](case-study.md): build, simulate, and analyze **your own** model.
4. Answer the [self-check](self-check.md) from memory.
5. Write up your [notes](notes.md) in your own words.
6. Tick this module off in the [progress tracker](../../README.md#progress).
