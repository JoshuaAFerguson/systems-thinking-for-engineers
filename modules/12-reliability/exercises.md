# Module 12 — Exercises

Work these after the readings. Keep answers here (or link out) so the trail is visible. Use the
reinforcing/balancing-loop notation from Module 03 and name archetypes from Module 07 where they
fit.

---

### Exercise 12.1 — Draw the cascading-failure loop

Take a distributed system you know (microservices, a job queue, a data pipeline). Draw the
**reinforcing loop** by which one node's overload becomes many nodes' overload. Label:
- the initial perturbation (what nudged the first node),
- the mechanism that passes load to neighbors (shared pool, synchronous call, retry, queue),
- why the loop reinforces rather than settling.

> _Your diagram:_

---

### Exercise 12.2 — Model a retry storm and its brake

Draw the retry-storm loop explicitly:

> _dependency slows → callers time out → callers retry → load on dependency rises → dependency
> slows further_

Name it as the archetype it is (from Module 07). Then add the **balancing loop** that tames it —
a circuit breaker, exponential backoff with jitter, a token-bucket rate limit, or load shedding.
For your chosen brake, state:
- what it senses,
- what it does when the sense crosses a threshold,
- the **delay** between "things go bad" and "brake engages," and what happens if that delay is
  too long.

> _Your answer:_

---

### Exercise 12.3 — Find the missing balancing loop

Pick a real system you operate or use. Find one **amplifying loop with no brake** — a place
where a small failure can run away because no circuit breaker, backpressure, rate limit, or load
shedder is present. Describe:
- the amplifying loop,
- what a small trigger would do today,
- the specific balancing loop you'd add, where you'd wire it, and its setpoint.

> _Your answer:_

---

### Exercise 12.4 — Reframe a "root cause" as structure

Take one incident with a known "root cause" writeup (yours or a public postmortem). Rewrite its
cause **as a structure**, per Cook and STAMP:
- the latent conditions already present (degraded mode of normal operation),
- the several small failures that aligned,
- the **control** that was missing, slow, or unenforced (which constraint went unchecked?).

Contrast: what does the structural view suggest fixing that the single-root-cause view didn't?

> _Your answer:_
