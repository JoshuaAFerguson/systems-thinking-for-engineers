# Module 10 — Mapping Practice

**Phase 2 · Tools & Patterns**

This is the capstone of Phase 2: the full causal-loop-diagramming (CLD) workflow, applied end to
end to one real, messy problem. Earlier modules gave you the pieces — feedback, loops, archetypes,
leverage. Here you run them as a single repeatable process, from "something is wrong" to "here's
the structure driving it, and here's where the leverage is."

## Objectives

By the end of this module you should be able to:

1. Run the six-step mapping workflow on a real problem without getting lost.
2. Assign **polarity** to a causal link correctly (same-direction `+` vs. opposite-direction `−`).
3. Find the loops in a tangle of variables and label each **R** (reinforcing) or **B** (balancing).
4. Read the **story** the structure tells and locate a leverage point in it — connecting this
   module back to archetypes (07) and leverage points (08).

## Key concepts

The workflow — six steps, in order:

1. **State the problem as a behavior over time.** Not "the deploys are bad" but a graph: *deploy
   frequency fell steadily over two quarters while incident count rose.* A reference behavior graph
   keeps the map honest and bounds the scope.
2. **Inventory the variables.** List the things that change — quantities and rates, not events.
   Prefer neutral, measurable nouns ("review latency," "WIP," "confidence") over loaded ones.
3. **Connect them with polarity.** Draw a causal arrow only where one variable genuinely drives
   another. Mark each `+` (they move the *same* direction — more cause, more effect) or `−` (they
   move *opposite* — more cause, less effect). Get the polarity right and the loops fall out
   almost mechanically.
4. **Find and label the loops.** Trace closed paths. Count the negative links: an **even** number
   (including zero) of `−` links is **reinforcing (R)**; an **odd** number is **balancing (B)**.
   Name each loop for the story it tells ("the rework spiral," "the trust rebuild").
5. **Find the story the structure tells.** Which loop dominates now? Where are the delays? Does the
   shape match a known **archetype** from Module 07? The map is a hypothesis about *why* the
   behavior-over-time looks the way it does.
6. **Locate leverage.** Using Module 08's ladder, ask where a small change reshapes the dominant
   loops — an information flow, a rule, a goal — rather than the parameter you'd reach for first.

Discipline notes that separate a useful CLD from a hairball: keep variables *neutral and
measurable*; make polarity explicit on every link; don't map events, map the things that
accumulate and rate; and stop adding variables once the loops that explain your reference behavior
are closed. A CLD is a communication and hypothesis tool — completeness is not the goal, *insight
into the behavior* is.

## Assigned readings

- Meadows, *Thinking in Systems* — the **feedback-loop** material (Ch. 1–2) and **Chapter 6** on
  leverage points, reused here as the vocabulary for reading a finished map.
- Daniel H. Kim — his writing on **causal loop diagramming practice** (the *Systems Archetypes*
  and *Systems Thinking Tools* material): how to choose variables, assign polarity, and read loops.

See [reading-list.md](../../resources/reading-list.md) for full references.

## Tools (pick one)

- **[LOOPY](https://ncase.me/loopy/)** — browser tool for quick, *animated* causal loop diagrams.
  The fastest way to see whether a loop reinforces or balances. No install; exportable.
- **Excalidraw / draw.io** — for a cleaner static diagram you commit as an image.
- **Mermaid** — commit the diagram as a `.mmd` file (or a fenced ```mermaid``` block) so it lives
  in the repo as text and renders on the web.

Commit your final map into the module as an image, a LOOPY link, or a `.mmd` file.

See [reading-list.md](../../resources/reading-list.md) for full references.

## Work this module in order

1. Read the assigned readings.
2. Do the [exercises](exercises.md) — practice polarity and loop-labeling on a small scenario.
3. Work the [case study](case-study.md): a full CLD of a real problem, committed as an artifact.
4. Answer the [self-check](self-check.md) from memory.
5. Write up your [notes](notes.md) in your own words.
6. Tick this module off in the [progress tracker](../../README.md#progress).
