# Module 12 — Reliability

**Phase 3 · Technical applications**

Incidents are system behavior, not single "root causes." This module reframes outages as the
output of a *structure* — reinforcing loops that amplify failure, balancing loops that should
have contained it, and control loops that were meant to catch it. The archetypes from Module 07
and the loop vocabulary from Module 03 do most of the work here.

## Objectives

By the end of this module you should be able to:

1. Explain why a major incident rarely has a single **root cause**, and reframe it as a
   *structure* of interacting conditions.
2. Draw **cascading failure** as a reinforcing loop, and **retry storms / thundering herds** as
   amplifying loops that turn a small perturbation into an outage.
3. Recognize the **balancing loops** engineered to contain failure — circuit breakers,
   backpressure, load shedding, rate limits, error budgets — and reason about their delays.
4. Describe reliability as a **control problem**: the SRE loop (monitor → alert → respond) and
   Leveson's **STAMP** view of safety as inadequate control, not just component failure.

## Key concepts

- **"Root cause" is a linear story.** The linear view (Module 00) wants one broken part and one
  fix. Cook's *How Complex Systems Fail* says the opposite: complex systems run in a degraded
  mode as normal, always contain latent faults, and fail only when *several* small failures line
  up. There is no root cause — there is a structure that permitted the alignment.
- **Cascading failure is a reinforcing loop.** One overloaded node sheds its work onto its
  neighbors, which overload and shed onto theirs. Failure feeds failure: the R loop from
  Module 03, running in the wrong direction. Nothing "spreads" — the loop *amplifies*.
- **Retry storms and thundering herds are amplifying loops.** A slow dependency causes timeouts;
  timeouts trigger retries; retries multiply load on the already-slow dependency; it gets slower.
  This is the "Fixes that Fail" archetype from Module 07: the local fix (retry to recover) makes
  the global problem worse.
- **Circuit breakers, backpressure, and error budgets are balancing loops.** A circuit breaker
  opens to cut the amplifying loop; backpressure signals upstream to slow down; load shedding
  drops low-priority work to protect the core; an error budget converts reliability into a
  *goal-seeking* balancing loop that throttles release risk. Each pushes the system back toward a
  safe setpoint — and each has a **delay** (detection, propagation) that, if too long, lets the
  reinforcing loop win first.
- **SRE is a control loop.** Monitor → alert → respond → recover is exactly the balancing-loop
  structure from Module 03 wrapped around a service. Alert delay, human response delay, and
  rollback delay are the parameters that decide whether the control loop is fast enough.
- **STAMP: accidents are control failures.** Leveson reframes safety not as "which component
  broke" but as "which constraint went unenforced." Losses happen when the control structure —
  monitors, limits, human operators, automation — fails to keep the system inside safe bounds.
  Missing or slow control, not a faulty widget, is the systemic cause.

## Assigned readings

- Richard Cook, *How Complex Systems Fail* (2000) — the whole thing; it's short. Read points
  1–7 as a direct rebuttal to root-cause thinking.
- Nancy Leveson, *Engineering a Safer World* — the **STAMP** model: safety as a control problem,
  accidents as inadequate enforcement of constraints. (Chapters on the model; skim the formalism.)
- Google **SRE** material (*Site Reliability Engineering* / *The SRE Workbook*) — **error
  budgets**, and control-loop treatments of monitoring, alerting, and incident response.

See [reading-list.md](../../resources/reading-list.md) for full references.

## Work this module in order

1. Read the assigned readings.
2. Do the [exercises](exercises.md).
3. Work the [case study](case-study.md) against a real incident you lived through.
4. Answer the [self-check](self-check.md) from memory.
5. Write up your [notes](notes.md) in your own words.
6. Tick this module off in the [progress tracker](../../README.md#progress).
