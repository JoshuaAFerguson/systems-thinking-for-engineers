# Module 08 — Exercises

Work these after the readings. Keep answers here (or link out) so the trail is visible.

---

### Exercise 8.1 — Place the intervention on the ladder

For each intervention, name which of Meadows' twelve leverage points it acts on (a number, a
delay, a loop, an information flow, a rule, a goal, a paradigm…).

| # | Intervention | Leverage point (12→1) |
|---|--------------|-----------------------|
| a | Raise the connection-pool size from 50 to 100. | |
| b | Show each team its own cloud spend on a shared dashboard. | |
| c | Change on-call comp so reliability work is rewarded, not just feature shipping. | |
| d | Cut the deploy feedback delay from 2 weeks to 20 minutes. | |
| e | Redefine the team's north-star metric from "features shipped" to "customer time-to-value." | |
| f | Let teams reorganize their own service boundaries as the product evolves. | |
| g | Add a bigger retry buffer queue in front of a flaky consumer. | |

> _Your answers:_

---

### Exercise 8.2 — Rank by leverage

Here are five candidate fixes for a service that keeps falling over under load. Rank them by
**leverage** (highest first) and justify the order.

- Add two more replicas.
- Add a load-shedding rule that rejects low-priority traffic first.
- Publish per-caller latency back to each calling team so they see the cost they impose.
- Shorten the autoscaler's reaction delay.
- Redefine the service's goal from "never drop a request" to "protect p99 for paying users."

> _Your ranking and reasoning:_

---

### Exercise 8.3 — Three levels on one real problem

Pick a real problem you own. Brainstorm at least one intervention at **each** of three different
leverage levels:

- **A parameter (point 12):** _the dial you'd normally reach for._
- **A loop or information flow (points 8–6):** _a change to feedback strength or who sees what._
- **A goal or paradigm (points 3–2):** _a change to what the system is for, or the mindset behind it._

Then say which you'd actually pursue, and what makes the higher-leverage option hard.

> _Problem:_
>
> _Parameter-level:_
>
> _Loop / information-flow-level:_
>
> _Goal / paradigm-level:_
>
> _What I'd pursue, and why:_

---

### Exercise 8.4 — Wrong direction

Meadows warns that people push high-leverage points the *wrong way*. Give one example — from work
or the readings — where someone changed a rule, goal, or information flow and made things worse
because the direction was backwards.

> _Your answer:_
