# Module 16 — Learning Organizations

**Phase 4 · Sociotechnical applications**

Some teams get hit by an incident, learn something real, and never repeat it. Others get hit
by the *same* incident every quarter, write the *same* postmortem, and change nothing. The
difference isn't intelligence or effort — it's whether the organization has a working
**learning loop**. This module names the disciplines that make a team able to learn, and the
crucial distinction between fixing the symptom and fixing the *rules that produced* the
symptom. Systems thinking is the thread that ties them together — Senge called it the *fifth
discipline* for exactly that reason.

## Objectives

By the end of this module you should be able to:

1. Name Senge's **five disciplines** and explain why systems thinking is the one that
   integrates the other four.
2. Distinguish **single-loop** from **double-loop** learning (Argyris) and classify a real
   fix as one or the other.
3. Diagnose a **broken learning loop** — an org that keeps repeating the same failure — and
   name where the loop is severed.
4. Explain why a **blameless postmortem** is a learning-loop design choice, not just a
   courtesy, and what makes one actually change behavior.

## Key concepts

- **Senge's five disciplines.** The practices of an organization that can learn:
  - **Personal mastery** — individuals committed to their own growth and to seeing reality
    clearly.
  - **Mental models** — surfacing and testing the assumptions each person carries (connects
    straight back to the Module 00 idea that where you draw the boundary changes the answer).
  - **Shared vision** — a genuine common goal people are pulled toward, not a poster on a
    wall.
  - **Team learning** — the capacity to think and learn together, faster than members can
    alone (dialogue over debate).
  - **Systems thinking** — the *fifth discipline*, the one that integrates the other four.
    Without it the disciplines stay a pile of parts; with it they become a system for
    learning. (Recall Module 00: a system is more than its parts.)
- **Single-loop learning (Argyris).** You detect an error and correct your **action**, while
  leaving the governing goals, assumptions, and rules untouched. The thermostat model: too
  cold → turn on the heat. Useful, fast, and often exactly right — but it never asks whether
  the setpoint itself is wrong.
- **Double-loop learning.** You detect an error and question the **governing variables** — the
  goals, the incentives, the mental models, the "way we do things" — that made the error
  likely. Not "turn on the heat" but "why is the setpoint 30°C, and who decided that?" This
  is where structural change (Module 08 leverage points) lives. Single-loop treats
  parameters; double-loop treats structure and goals.
- **Applied to engineering: the incident loop.** A postmortem is a designed feedback loop.
  For it to *learn*, the loop has to close: signal (what happened) → analysis (why, at the
  structural level) → change (an action that alters future behavior) → verification (did the
  change hold?). Break any link and the org stops learning.
- **Blameless postmortems as loop design.** Blame severs the analysis link: if naming the
  real cause gets someone punished, people route around the truth and the loop learns a
  fiction. Blamelessness isn't softness — it's what keeps the *information flow* (Module 15)
  honest enough to act on. The goal is to find the conditions that made a competent person's
  action reasonable, then change the conditions.
- **Why some orgs keep repeating the same incident.** Almost always a broken loop, and
  usually single-loop-only learning: the team fixes *this* null pointer but never asks why
  the architecture keeps producing that class of bug; adds *this* runbook step but never
  questions the goal that keeps the system fragile. The action items close; the governing
  variables never move; the incident returns. This is the "fixes that fail" and "shifting the
  burden" territory from Module 07, wearing an on-call pager.
- **The double-loop test.** After any fix, ask: *did we change an action, or did we change a
  rule that generates actions?* If every postmortem in a year produced only single-loop fixes,
  the org is patching, not learning.

## Assigned readings

- Senge, **_The Fifth Discipline_** (1990/2006) — the five disciplines and why systems
  thinking integrates them. Read the framing and the chapters introducing each discipline.
- **Chris Argyris on single-loop vs. double-loop learning** — "Teaching Smart People How to
  Learn" (HBR, 1991) is the compact entry point; the governing-variables framing is the core.
- *(Optional)* Revisit **archetypes** (Module 07) — "Fixes that Fail," "Shifting the Burden,"
  and "Eroding Goals" are what non-learning looks like from the outside — and **leverage
  points** (Module 08), since double-loop learning is a structure/goal-level intervention.

See [reading-list.md](../../resources/reading-list.md) for full references.

## Work this module in order

1. Read the assigned readings.
2. Do the [exercises](exercises.md).
3. Work the [case study](case-study.md) against a real learning (or non-learning) loop.
4. Answer the [self-check](self-check.md) from memory.
5. Write up your [notes](notes.md) in your own words.
6. Tick this module off in the [progress tracker](../../README.md#progress).
