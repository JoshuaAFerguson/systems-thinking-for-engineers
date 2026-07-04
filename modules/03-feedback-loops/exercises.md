# Module 03 — Exercises

Work these after the readings. Build the loops in [LOOPY](https://ncase.me/loopy/) where you
can, then paste a screenshot or link so the trail is visible.

---

### Exercise 3.1 — Draw a thermostat (balancing) loop

Build a CLD of any goal-seeking system you like (thermostat, autoscaler tracking target CPU,
a team keeping WIP at a limit). Include a *gap* variable (goal − current state) and show the
corrective action. Mark every link `+` or `−`, confirm the loop is balancing (odd number of
`−` links), and label it **B**.

> _Sketch / LOOPY link:_
>
> _Why it's balancing:_

---

### Exercise 3.2 — Draw a viral-growth (reinforcing) loop

Build a CLD of something that grows on itself (viral signups, compound interest, a burnout
spiral, an outage that generates more load). Show at least two variables feeding back into
each other. Confirm the loop is reinforcing (even number of `−` links) and label it **R**.

> _Sketch / LOOPY link:_
>
> _Why it's reinforcing — and is it virtuous or vicious?_

---

### Exercise 3.3 — Determine the polarity

For each mini-loop below, mark each link and give the overall loop sign (R or B):

1. Bank balance → interest earned → bank balance.
2. Stress → mistakes → rework → stress.
3. Room temperature → gap from setpoint → heater output → room temperature.
4. Price → demand → inventory → price.

> _1._
>
> _2._
>
> _3._
>
> _4._

---

### Exercise 3.4 — Couple the two

Take your reinforcing loop from 3.2 and add a balancing loop that eventually stops the
growth (saturation, cost, fatigue, a rate limit). Describe in words how the two loops trade
dominance over time.

> _The balancing loop I added:_
>
> _How dominance shifts over time:_
