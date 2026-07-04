# Module 11 — Exercises

Work these after the readings. Keep answers here (or link out) so the trail is visible. Reuse
the stock-and-flow notation from Module 02 and the causal-loop notation from Module 03.

---

### Exercise 11.1 — Draw the tech-debt stock and flow

Pick a codebase you work in. Draw technical debt as a **stock** with:
- an **inflow** of shortcuts (name the actual sources — deadline hacks, skipped tests,
  copy-paste, undeleted dead code),
- an **outflow** of paydown (name the actual mechanisms — refactoring, deletion, test-backfill),
- the current *rate* of each flow (roughly: is inflow or outflow winning right now?).

Then answer: with today's flows, is the stock rising, falling, or flat? What would it take to
make the outflow exceed the inflow?

> _Your diagram + answer:_

---

### Exercise 11.2 — Map the coupling

Take one part of that codebase — a service, a package, a set of modules. Draw it as a system of
**interconnections**, not a list of files. For each edge, note *what flows across it* (a call, a
shared database table, an event, a config value, an implicit ordering assumption).

Then find the node with the highest interconnection density (most edges). Answer:
- What happens to change effort when *that* node changes?
- Is its density essential to the problem, or accidental (could be reduced by an interface,
  an event, or a boundary)?

> _Your map + answer:_

---

### Exercise 11.3 — Find the reinforcing decay loop, then design the brake

Identify one **reinforcing loop of decay** in this codebase and write it as a loop:

> _harder to change → more shortcuts taken → ______ → harder to change_

Fill in the middle links with specifics from your system. Then design a **balancing loop** that
could counter it — a concrete mechanism (a refactor budget, a complexity check in CI, a
merge-blocking fitness function, an on-call-owns-cleanup rule). Describe:
- what it measures,
- what it pushes back toward,
- the delay before it takes effect (balancing loops with long delays overshoot — see Module 04).

> _Loop + brake:_

---

### Exercise 11.4 — Emergence spotting

Name one instance of **emergent complexity** in your system: a painful behavior that no single
module is responsible for, that only appears from the *interaction* of several. Describe where
someone reviewing any one file would miss it, and what view (a dependency graph, a trace, a
sequence diagram) would make it visible.

> _Your answer:_
