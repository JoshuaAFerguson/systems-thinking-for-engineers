# Module 07 — System Archetypes

**Phase 2 · Tools & Patterns**

Certain feedback structures show up over and over, in wildly different domains, producing the
same frustrating behavior each time. These recurring structures are the **system archetypes** —
a small vocabulary of "stories the structure tells." Learn them and you stop re-diagnosing the
same trap from scratch; you recognize it, and you already know where its leverage lives.

## Objectives

By the end of this module you should be able to:

1. Recognize the common archetypes by their **feedback structure**, not just by their symptoms.
2. Sketch the loop diagram for at least three archetypes from memory.
3. For each archetype, name its characteristic **behavior over time** and its **way out** — the
   intervention that actually relieves it rather than feeding it.
4. Diagnose a real situation in your org or product by naming the archetype operating inside it.

## Key concepts

An archetype is not a problem — it's a *structure* that generates a class of problems. Each one is
a specific arrangement of reinforcing (R) and balancing (B) loops, usually with a **delay** doing
the damage. The nine below are the ones you'll meet most as an engineer.

- **Fixes that Fail.** A quick fix relieves the symptom now, but a delayed reinforcing
  consequence makes the underlying problem worse later. (Add a cache to hide slow queries → the
  slow queries proliferate because nobody feels the pain.) *Way out:* address the root cause;
  treat the fix as buying time, not solving.
- **Shifting the Burden** (and its addiction variant). A symptomatic solution is so convenient
  that it atrophies the fundamental solution; over time you become *dependent* on the crutch and
  the real capability withers. (Always paging a hero on-call instead of fixing the system.)
  *Way out:* strengthen the fundamental response even while it's slower; wean off the symptomatic
  one.
- **Limits to Growth.** A reinforcing engine of growth eventually runs into a balancing
  constraint (a limit), and growth stalls or reverses. Pushing harder on the engine does nothing.
  *Way out:* find and ease the limiting factor, not the growth driver.
- **Tragedy of the Commons.** Individually rational use of a shared, limited resource degrades it
  for everyone; each actor's gain is private, the cost is shared and delayed. (Everyone adds "just
  one more" job to the shared CI runners.) *Way out:* make the shared cost visible and feedback
  it to users — quota, pricing, or governance of the commons.
- **Escalation.** Two parties each respond to the other's advance by advancing further; two
  balancing loops couple into one reinforcing arms race. (Competing teams over-provisioning to
  out-headroom each other.) *Way out:* one side unilaterally de-escalates, or a shared goal is
  negotiated above both.
- **Success to the Successful.** Two activities compete for a shared resource; early success
  earns more resource, which produces more success — the winner is locked in regardless of
  intrinsic merit. (The project that got staffed gets the wins that justify more staffing.)
  *Way out:* decouple them from the shared resource, or reset the allocation by a rule other than
  past success.
- **Drift to Low Performance.** A goal that floats to track *actual* performance slides downward:
  a bad result lowers the standard, the lower standard permits worse results. (Letting the SLO
  quietly follow the outage rate.) *Way out:* anchor the goal to an absolute external reference,
  not to recent performance.
- **Policy Resistance.** Multiple actors pull a system stock toward different goals; any push by
  one is countered by the others, so the system stays stuck and effort is wasted. *Way out:*
  align the goals (find the shared one worth pulling toward) rather than pulling harder.
- **Seeking the Wrong Goal.** The system faithfully optimizes exactly what you told it to — but
  the metric was a poor proxy for what you actually wanted. (Optimizing tickets-closed, getting
  reopened tickets.) *Way out:* fix the goal/indicator, not the behavior; this is the archetype
  behind Goodhart's Law.

The payoff: archetypes tell you **where the leverage is**. The obvious push (do more of the quick
fix, push harder on growth, allocate more to the winner) almost always makes the trap worse. The
escape is usually somewhere less obvious and higher up — a goal, a rule, an information flow.

## Assigned readings

- Meadows, *Thinking in Systems* — **Chapter 5, "System Traps — and Opportunities."** The core
  reading; her "traps" are these archetypes with the escapes spelled out.
- Senge, *The Fifth Discipline* — the **systems archetypes appendix** (and the "Laws of the Fifth
  Discipline"). The original engineering-adjacent naming of the archetypes.
- Daniel H. Kim, **"Systems Archetypes I–III"** — compact reference cards for each archetype's
  loop structure. Good to keep beside you while diagramming.

See [reading-list.md](../../resources/reading-list.md) for full references.

## Work this module in order

1. Read the assigned readings.
2. Do the [exercises](exercises.md).
3. Work the [case study](case-study.md) against a real system you've seen.
4. Answer the [self-check](self-check.md) from memory.
5. Write up your [notes](notes.md) in your own words.
6. Tick this module off in the [progress tracker](../../README.md#progress).
