# Module 14 — Exercises

Work these after the readings. Keep answers here (or link out) so the trail is visible.

---

### Exercise 14.1 — Map the org, map the architecture

Pick a system you know well. Draw two diagrams side by side:

- **The org graph:** teams as nodes, communication paths as edges. Draw an edge where two
  teams actually talk regularly (standups, shared channels, joint on-call), not where an org
  chart *says* they should.
- **The architecture graph:** services/modules as nodes, interfaces/calls as edges.

Now line them up. For each architectural edge, name the org edge that produced it.

> _Your two diagrams (link an image, a LOOPY/Excalidraw file, or describe them):_
>
> _The mapping (architecture edge → org edge):_

---

### Exercise 14.2 — Find the homomorphism (and the leaks)

Conway's Law predicts a structural match between the two graphs above. Where does the match
hold cleanly, and where does it *leak*?

- Name one interface that is a faithful copy of a team boundary (clean mirror).
- Name one place where the architecture has a seam the org doesn't — or the org has a
  boundary the architecture ignores (a shared "god" module two teams both edit, a service no
  team clearly owns).

> _Clean mirror:_
>
> _Leak:_

---

### Exercise 14.3 — Locate a mismatch causing friction

Find one spot where the org shape and the *desired* architecture are fighting. Symptoms to
look for: an interface that needs constant cross-team meetings; a change that always requires
three teams; a module everyone touches and no one owns; duplicated logic in two services
because the teams don't talk.

Write:
- the friction you observe,
- the communication structure producing it,
- what a **CLD** (Module 03) of the reinforcing loop looks like (e.g., low bandwidth →
  duplicated code → more surface to coordinate → less bandwidth).

> _The friction:_
>
> _The communication structure behind it:_
>
> _The loop:_

---

### Exercise 14.4 — Propose an Inverse Conway Maneuver

Take the mismatch from 14.3 and design a **team-boundary change** to fix it at the source.
Use the Team Topologies vocabulary:

- Which team **type** should own each piece (stream-aligned, platform, enabling,
  complicated-subsystem)?
- What **interaction mode** connects them (collaboration, X-as-a-Service, facilitating)?
- What is each team's **API** — what does it promise and how is it consumed?
- What **cognitive load** does the change add or remove?

Then predict: what architecture will grow along these new seams, and how long is the delay?

> _The maneuver:_
>
> _Predicted architecture + expected lag:_

---

### Exercise 14.5 — Where is this a leverage point?

Place the Inverse Conway Maneuver on Meadows' leverage ladder (Module 08). Is reshaping teams
a parameter change, a structure change, a goal change, or a paradigm change? Contrast it with
the *low-leverage* alternative someone might reach for instead (e.g., "add a coordination
meeting," "write a stricter API doc").

> _Your answer:_
