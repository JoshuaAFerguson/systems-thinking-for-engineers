# Module 09 — Exercises

Work these after the readings. This module is hands-on: you'll actually build and run a model.
Commit the model file (Insight Maker link, Vensim `.mdl`, or a Python script/notebook) alongside
your answers.

---

### Exercise 9.1 — State the purpose first

Pick one small system to model: **SaaS customers** (signups − churn), a **support backlog**
(arrivals − resolutions), or **tech-debt accumulation** (debt added − debt paid down). Before
building anything, write:

- the one-sentence **question** your model should help answer,
- the **stock(s)**, the **flow(s)**, and the one **feedback** that makes it interesting,
- what you're deliberately leaving **outside** the boundary.

> _Purpose:_
>
> _Stocks / flows / feedback:_
>
> _Out of scope:_

---

### Exercise 9.2 — Build it step by step

In your chosen tool, build the model incrementally and note what you did at each step:

1. Create the stock with a starting value.
2. Add the inflow and outflow.
3. Make one flow **depend on the stock** (the feedback).
4. Set initial parameter values.
5. Run it and plot the stock over time.

> _Model link/file:_
>
> _What each step did to the behavior:_

---

### Exercise 9.3 — Vary one parameter

Hold everything constant and change a single parameter (e.g. `churn_rate`, arrival rate, or
debt-per-feature) across two or three values. Record the behavior-over-time for each run.

| Parameter value | Behavior you observed (shape, ceiling, oscillation…) |
|-----------------|------------------------------------------------------|
| | |
| | |
| | |

> _What the sweep told you about the structure:_

---

### Exercise 9.4 — Compare to reality

Compare your model's behavior to what you've actually seen in the real system. Where do they
agree? Where do they diverge — and what missing structure would explain the gap?

> _Agreement:_
>
> _Divergence + likely missing structure:_

---

### Exercise 9.5 — Document one surprise

Every useful model produces at least one "huh." Write the one thing the simulation showed you that
your head-math had wrong.

> _The surprise:_
