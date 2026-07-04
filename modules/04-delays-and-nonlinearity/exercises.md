# Module 04 — Exercises

Work these after the readings. Simulating a delay in [LOOPY](https://ncase.me/loopy/) or
[Insight Maker](https://insightmaker.com/) makes the oscillation visceral — do it if you can,
then keep the sketch or link here.

---

### Exercise 4.1 — Add a delay, watch it oscillate

Take a balancing loop (a thermostat, an autoscaler, restocking inventory, hiring to a target
headcount). First describe how it behaves with an *instant* response. Then insert a delay
between the corrective action and its effect. Sketch both BOTGs.

> _Behavior with no delay:_
>
> _Behavior with a delay (shape of the oscillation):_
>
> _Sketch / link:_

---

### Exercise 4.2 — Trace a bullwhip

Pick a chain you know (autoscaling reacting to lagged metrics, a hiring pipeline, an ordering
chain, alert-driven remediation). Walk one small change at the "customer" end through the
chain and describe how the delay amplifies it at each stage.

> _The chain:_
>
> _The small initial change:_
>
> _How it gets amplified downstream:_

---

### Exercise 4.3 — Overshoot-and-collapse vs. S-curve

Sketch two BOTGs for the same growing quantity: one where it overshoots a limit and
collapses, one where it bends into an S-curve and plateaus. What structural difference
(delay in perceiving the limit? erodible vs. fixed limit?) decides which one happens?

> _Sketch / link:_
>
> _What decides collapse vs. plateau:_

---

### Exercise 4.4 — Find a nonlinearity

Name a real relationship in your systems that is clearly **nonlinear** — a response with a
knee, a threshold, or a cliff (queue latency vs. utilization, retries vs. load, on-call
fatigue vs. page count). Describe where the linear intuition breaks and what the curve
actually does past the knee.

> _The relationship:_
>
> _Where linear intuition breaks:_
>
> _What the curve really does:_
