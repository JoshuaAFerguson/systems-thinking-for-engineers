# Module 15 — Incentives & Metrics

**Phase 4 · Sociotechnical applications**

Every metric you put on a dashboard is a feedback signal wired into a system full of people
who will respond to it. That's the point — and it's also the danger. This module is about
what happens *after* you start measuring: the goal you actually installed, the behavior it
actually rewards, and the gap between the two. Meadows warned that information flows are a
high-leverage place to intervene *and* that "seeking the wrong goal" is one of the deepest
system traps. Both are true at once, and metrics live exactly at that intersection.

## Objectives

By the end of this module you should be able to:

1. Explain why a metric is a **feedback signal** — and why installing one changes the system
   you were trying to observe.
2. State **Goodhart's Law** and **Campbell's Law**, and tell them apart from the everyday
   "the metric is wrong" complaint.
3. Trace a **perverse incentive** (the cobra effect) from proxy metric to gamed behavior to
   damaged system goal.
4. Distinguish **local optimization** (a metric improving while the whole system degrades)
   from genuine improvement.
5. Redesign a metric — or, more often, **pair it with a balancing measure** — so the reward
   points back at the real goal.

## Key concepts

- **Metrics are feedback signals.** A measure that's watched, rewarded, or funded becomes an
  input to behavior. You didn't just add a number; you added a **feedback loop** (Module 03)
  and set a **goal** for it (Module 08). People and teams will steer toward the number.
- **Goodhart's Law.** *"When a measure becomes a target, it ceases to be a good measure."*
  (Strathern's crisp phrasing of Goodhart's observation.) The moment a proxy is optimized,
  the correlation you relied on decays — because effort flows to the *proxy*, not the thing
  it stood for.
- **Campbell's Law.** The social-science sibling: the more a quantitative indicator is used
  for decision-making, the more it distorts and corrupts the process it was meant to monitor.
  Same phenomenon, stated from the measurement side.
- **The proxy trap.** You want quality; you measure test count. You want productivity; you
  measure lines of code or tickets closed. You want reliability; you measure uptime on a
  dashboard nobody bleeds into user pain. The proxy is *cheap to measure and easy to game*,
  and it drifts away from the goal the instant it becomes the target.
- **The cobra effect / perverse incentives.** The parable: a bounty on dead cobras led people
  to *breed* cobras. The metric ("cobras killed") got maximized; the goal ("fewer cobras")
  got worse. Engineering versions: rewarding closed tickets breeds trivial tickets; rewarding
  bug-fix counts breeds bugs; rewarding code review speed breeds rubber-stamp approvals.
- **Local optimization harming the global system.** A team maximizes its own metric —
  velocity, its service's latency, its own on-call quiet — by pushing cost onto a neighbor:
  tech debt, a noisy dependency, a queue that backs up downstream. The local number goes
  green; the system gets worse. This is the archetype work of Module 07 wearing a
  scoreboard.
- **Balancing measures.** The cheapest defense: never ship a target metric alone. Pair every
  "go faster" metric with a "don't break things" metric (throughput *and* change-fail rate;
  tickets closed *and* reopen rate; coverage *and* escaped-defect rate). The pair makes the
  gaming visible, because you can't win both by cheating one.
- **The audit question.** Before shipping a metric, ask the load-bearing question: *"What is
  the cheapest way to make this number look good — and would that behavior actually serve the
  goal?"* If the cheapest path is gaming, you've designed an exploit, not a measurement.

## Assigned readings

- **Goodhart / Strathern on Goodhart's Law.** Strathern's 1997 paper ("'Improving ratings':
  audit in the British university system") for the sharp phrasing; Goodhart's original for
  the monetary-policy root. Short.
- Meadows, **_Thinking in Systems_** — the **information flows** leverage point (giving a
  system a missing feedback loop) *and* the **"seeking the wrong goal"** system trap. Read
  them together; metrics sit precisely between them.
- *(Optional)* Revisit the **archetypes** module (Module 07): "Success to the Successful,"
  "Shifting the Burden," and "Eroding Goals" all show up wherever metrics drive behavior.

See [reading-list.md](../../resources/reading-list.md) for full references.

## Work this module in order

1. Read the assigned readings.
2. Do the [exercises](exercises.md).
3. Work the [case study](case-study.md) against a real metric in your world.
4. Answer the [self-check](self-check.md) from memory.
5. Write up your [notes](notes.md) in your own words.
6. Tick this module off in the [progress tracker](../../README.md#progress).
