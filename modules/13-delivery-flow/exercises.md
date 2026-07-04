# Module 13 — Exercises

Work these after the readings. Keep answers here (or link out) so the trail is visible. Treat
each queue as an invisible stock (Module 02) and connect WIP limits to the leverage points from
Module 08.

---

### Exercise 13.1 — Compute Little's Law for a real queue

Pick a real queue you can measure: PR review backlog, a ticket column, a support queue, a deploy
pipeline. **Measure two** of the three variables and **derive the third**:
- **L** = average work-in-progress (items sitting in the queue),
- **λ** = throughput (items completed per day/week),
- **W** = lead time (average time an item spends in the queue).

Show your numbers and the arithmetic (`W = L / λ`, or `L = λW`, etc.). Then sanity-check the
derived value against your gut — does it match what people *feel* the wait is?

> _Your measurement + derivation:_

---

### Exercise 13.2 — Identify the constraint

Map your delivery process as a sequence of steps (idea → code → review → test → deploy → done).
For each step, estimate its capacity (how many items/day it can clear). Then:
- **Identify** the constraint — the single slowest step where work piles up.
- Confirm it: is there a visible queue (a stock) growing in front of it?
- Apply the next steps: how would you **exploit** it (get more from existing capacity before
  spending money), what would you **subordinate** to it, and how might you **elevate** it?

> _Your answer:_

---

### Exercise 13.3 — WIP-limit thought experiment

Take the constraint from 13.2. Using Little's Law, predict what happens to **lead time** if you:
- **halve** the WIP feeding it (cut items-in-progress in half, hold throughput), then
- **double** the WIP.

Show the predicted lead times. Then argue, in a few sentences, why capping WIP is a leverage
point (Module 08) even though nobody is working faster — what does the cap force the system to do?

> _Your answer:_

---

### Exercise 13.4 — Batch size and feedback delay

Find one place in your pipeline where **batch size is large** (big releases, long-lived
branches, weekly deploys, giant PRs). Describe:
- how the large batch lengthens the queue's residence time,
- how it delays feedback (and which loop from earlier modules that delay lives in),
- what a smaller batch would cost and what it would buy.

> _Your answer:_
