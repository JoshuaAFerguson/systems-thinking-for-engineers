# Module 05 — Exercises

Work these after the readings. Keep answers here (or link out) so the trail is visible.

---

### Exercise 5.1 — Resilience assessment

Pick a real system you rely on (a service, a team, a deployment pipeline, a supply chain).
Ask: what disturbances can it absorb and recover from, and what would it *fail* to recover
from? List the loops or mechanisms that give it its bounce-back.

| | |
|---|---|
| Disturbances it recovers from | |
| Disturbances that would break it | |
| The mechanisms that give it resilience | |

> _Notes:_

---

### Exercise 5.2 — Where efficiency ate resilience

Find a place where slack, redundancy, or a buffer was removed to make a system leaner. What
was gained, what became fragile, and under what disturbance would the loss bite?

> _What was optimized away:_
>
> _What was gained:_
>
> _The disturbance that would expose the fragility:_

---

### Exercise 5.3 — Spot the sub-optimization

Name a case where a part optimized its own goal at the expense of the whole (a team hitting a
local metric, a service protecting itself by hurting a neighbor). What was the local goal,
what did the whole lose, and how would you rebalance the hierarchy?

> _The local goal:_
>
> _What the whole system lost:_
>
> _How you'd rebalance:_

---

### Exercise 5.4 — Trace the hierarchy

Draw the nested hierarchy of one system (subsystems within systems). Identify one place where
the hierarchy *reduces information load* (interactions stay local) and one place where it
*fragments* the system (a boundary that hides something important).

> _The nesting:_
>
> _Where hierarchy helps:_
>
> _Where hierarchy fragments:_
