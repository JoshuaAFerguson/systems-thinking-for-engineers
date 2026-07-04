# Module 14 — Conway's Law

**Phase 4 · Sociotechnical applications**

You've spent the earlier modules treating the *technical* system as the thing under study.
This phase flips the boundary outward: the organization that builds the system is *itself* a
system, and it leaves fingerprints all over the architecture. Conway's Law is the hinge.
Once you see it, you can't unsee it — and you can start using it on purpose.

## Objectives

By the end of this module you should be able to:

1. State **Conway's Law** precisely and explain *why* it holds — the mechanism, not just the
   slogan.
2. Find the **homomorphism** between a real org's communication structure and its
   architecture: which team boundary produced which interface.
3. Diagnose a concrete **mismatch** where the org shape and the desired architecture fight
   each other, and describe the friction it causes.
4. Propose an **Inverse Conway Maneuver** — a team-boundary change designed to produce the
   architecture you want — and use the **Team Topologies** vocabulary to describe it.

## Key concepts

- **Conway's Law (1968).** *"Any organization that designs a system... will produce a design
  whose structure is a copy of the organization's communication structure."* The system is a
  mirror. Two modules talk to each other cleanly only if the people who own them talk to each
  other cleanly. The interface *is* the communication path, frozen into code.
- **Why it holds.** An interface between two components requires negotiation and agreement.
  Negotiation happens along communication paths. Where two groups rarely communicate, they
  will avoid building a rich shared interface — they'll build a wall, a queue, a thin API, or
  a duplicated copy instead. The architecture takes the path of least *organizational*
  resistance. This is a feedback structure, not a coincidence.
- **The org is a system that shapes a system.** Reorgs are architecture decisions in
  disguise. A merged team tends to merge its services; a split team tends to split them
  (eventually). The delay between the org change and the architectural change is exactly the
  kind of lag you learned to watch for in Module 04.
- **The Inverse Conway Maneuver.** If systems mirror orgs, then to *get* a target
  architecture, first shape the org to match it. Design the teams and their communication
  paths deliberately, and let the desired architecture grow along those seams. This is a
  **leverage-point** move (Module 08): you're intervening in structure, not tuning a
  parameter.
- **Team Topologies — four team types.**
  - **Stream-aligned:** owns a flow of value end-to-end (a product, a user journey). The
    default and most common type; everything else exists to support these.
  - **Platform:** provides internal services/tools that reduce the cognitive load of
    stream-aligned teams. Treated as a product with users.
  - **Enabling:** a coaching/consulting team that helps others adopt a capability, then
    steps away. Temporary by design.
  - **Complicated-subsystem:** owns a part that needs deep specialist knowledge (a physics
    engine, a codec, a risk model) so others don't have to carry it.
- **Three interaction modes.** *Collaboration* (two teams work closely for a time — high
  bandwidth, high cost), *X-as-a-Service* (one team consumes another's offering over a clean
  boundary — low bandwidth, low friction), and *Facilitating* (one team helps another for a
  period). The mode you choose *is* a Conway decision: it sets which interfaces will form.
- **Team cognitive load.** A team can only hold so much in its head. Overload a team with too
  many unrelated domains and the architecture it produces gets muddy at exactly the seams it
  can't attend to. Bounded, well-sized teams produce bounded, well-shaped services.
- **Team APIs.** A team has an interface too: its code, its docs, its runbooks, its ways of
  being contacted, its promises. Designing the *team's* API is designing the system's future
  interfaces.

## Assigned readings

- Melvin Conway, **"How Do Committees Invent?"** (1968) — the original. Short. Read the actual
  paper, not a paraphrase; the argument is tighter than the slogan.
- Skelton & Pais, **_Team Topologies_** (2019) — the four team types, three interaction
  modes, cognitive load, and the Inverse Conway Maneuver. Read the framing chapters plus the
  team-types and interaction-modes chapters.
- *(Optional)* Revisit Meadows on **leverage points** (Module 08): the Inverse Conway
  Maneuver is a structure-level intervention, and it helps to place it on the leverage
  ladder.

See [reading-list.md](../../resources/reading-list.md) for full references.

## Work this module in order

1. Read the assigned readings.
2. Do the [exercises](exercises.md).
3. Work the [case study](case-study.md) against a real org-to-architecture coupling.
4. Answer the [self-check](self-check.md) from memory.
5. Write up your [notes](notes.md) in your own words.
6. Tick this module off in the [progress tracker](../../README.md#progress).
