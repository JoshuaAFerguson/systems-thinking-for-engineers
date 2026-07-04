# Module 12 — Case Study

> **Your work.** Take one real incident you lived through (or a public postmortem you know well)
> and analyze it as **structure** — loops, delays, and missing controls — instead of a linear
> root-cause chain. The goal isn't to assign blame; it's to see the system that made the outage
> possible. Use the loop notation from Module 03, the archetypes from Module 07, and Cook/STAMP.

## The incident

_Name the incident in a sentence: what degraded, for how long, and who felt it._

## The linear story

_Write the single-root-cause version first — the "X broke, so we fixed X" narrative that a quick
postmortem would produce._

## The latent conditions

_Per Cook: what was already true before the incident? What degraded-but-normal conditions and
latent faults were present that nobody was paging on?_

## The amplifying structure

_Draw the reinforcing loop(s) that turned a small trigger into an outage — cascade, retry storm,
thundering herd. What aligned? Name the archetype if one fits._

## The missing or slow control

_Per STAMP: which balancing loop or control was absent, too slow, or unenforced? Which safety
constraint went unchecked? Where were the damaging delays?_

## What structure suggests fixing

_What does the systemic view tell you to change that the single-root-cause view missed? Two or
three sentences on what you saw once you stopped looking for one broken part._
