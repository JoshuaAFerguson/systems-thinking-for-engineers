# Module 10 — Exercises

Work these after the readings. Commit any diagram (LOOPY link, image, or `.mmd`) alongside your
answers so the trail is visible.

---

### Exercise 10.1 — Behavior over time first

Take this supplied scenario:

> A team adds a mandatory review step to improve quality. Review latency grows, so work-in-progress
> piles up, so people batch bigger changes to "make the review worth it," which makes each review
> slower still. Quality is uneven and morale drops.

Draw the **reference behavior graph**: which quantities are rising or falling over time, and over
what horizon? (A rough sketch of curves is enough.)

> _Your behavior-over-time sketch:_

---

### Exercise 10.2 — Inventory the variables

List the changing quantities and rates in the scenario as **neutral, measurable** nouns. Avoid
events and loaded words.

> _Variables:_

---

### Exercise 10.3 — Assign polarity

For each pair, mark the link `+` (same direction) or `−` (opposite direction), and justify it in a
few words.

| From → To | Polarity (+/−) | Why |
|-----------|----------------|-----|
| review latency → WIP | | |
| WIP → batch size | | |
| batch size → review latency | | |
| review latency → morale | | |
| review thoroughness → defects shipped | | |

> _Your answers:_

---

### Exercise 10.4 — Find and label the loops

Trace the closed loops in your map. For each, count the negative links, decide **R or B** (even
number of `−` = R; odd = B), and give it a short story-name.

| Loop (variables in the cycle) | # of − links | R or B | Name |
|-------------------------------|--------------|--------|------|
| | | | |
| | | | |

> _Which loop dominates the behavior, and does the structure match an archetype from Module 07?_

---

### Exercise 10.5 — Locate leverage

Using Module 08's ladder, name one **low-leverage** fix someone would try here and one
**higher-leverage** intervention the map points to. Say which loop each one acts on.

> _Low-leverage:_
>
> _Higher-leverage:_
