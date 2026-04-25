Hybrid behavioural engine for Edenshell

A compact spec in markdown, treating Edenshell as a modern core + ancient drive system.

---

1. High‑level architecture

`text
[ Ancient Lineage Layer ]
    Deep-Sea / Mineral / Mycelial / Cosmological

[ Behaviour Engine Layer ]
    ABM + FSM + CA + Behaviour Trees + Prediction + Fractal Texture

[ Modern Core Runtime ]
    IoT APIs, safety logic, schedules, device control

[ Sensor Mesh ]
    cameras, motion, vibration, temp, humidity, contact, etc.

[ Actuator Layer ]
    lights, speakers, locks, HVAC, notifications

[ Physical House ]
    humans, pets, routines, environment
`

---

2. Core components

2.1 Agent‑based organism logic

- Role: Defines how “the organism” (Edenshell) responds to the environment.  
- Inputs: Normalised sensor events, household context, time.  
- Outputs: Intent signals (observe, warn, intervene, ignore).  
- Lineage specialisation:  
  - Deep‑Sea: pressure gradients, calm correction.  
  - Mineral: structural stress, boundary integrity.  
  - Mycelial: network continuity, pattern shifts.  
  - Cosmological: timing drift, orbital anomalies.

2.2 State layer (FSM)

- Global states: Idle, Attentive, Concerned, Intervening, Escalating.  
- Transitions: Triggered by thresholds, patterns, or lineage‑specific cues.  
- Guarantee: No direct jump from Idle → Escalating without passing through intermediate states.

2.3 Sensitivity grid (cellular automata)

- Grid: Logical map of the house (zones, rooms, boundaries).  
- Cells: Each zone has a state (quiet, active, anomalous, unknown).  
- Update rule:  
  - Local sensor changes + neighbour influence → new cell state.  
- Lineage flavour:  
  - Deep‑Sea: pressure‑like diffusion.  
  - Mineral: crack/strain propagation.  
  - Mycelial: signal spreading through a network.  
  - Cosmological: slow drift and phase shifts.

2.4 Decision hierarchy (behaviour trees)

- Top‑level branches:  
  - Safety → fire, gas, intrusion, escape.  
  - Integrity → doors, windows, leaks, fences.  
  - Comfort → temperature, light, noise.  
  - Courtesy → notifications, timing, non‑intrusiveness.  
- Execution:  
  - Evaluate highest‑priority branch first.  
  - Fall back gracefully if conditions not met.  
  - Always respect safety and user preferences.

2.5 Prediction layer (lightweight physics / modelling)

- Purpose: Anticipate near‑future states.  
- Examples:  
  - Door likely to slam?  
  - Pet likely to exit boundary?  
  - Window likely to rattle open?  
- Method: Simple models + historical patterns, not heavy ML.

2.6 Fractal texture (ancient feel)

- Scope: Micro‑timing, micro‑variation, ambient behaviour.  
- Used for:  
  - Slightly irregular polling intervals.  
  - Non‑repeating notification timing (within bounds).  
  - Subtle environmental adjustments (light, sound).  
- Rule: Never drives decisions, only texture.

---

3. Data flow

1. Sense:  
   Raw IoT events → normalised sensor stream.

2. Map:  
   Sensor stream → sensitivity grid (CA) + context.

3. Interpret:  
   Grid + context → organism logic (ABM) → intent.

4. Stabilise:  
   Intent → state layer (FSM) → current global state.

5. Decide:  
   State + intent → behaviour tree → chosen action.

6. Shape:  
   Action timing/texture → fractal layer → final action profile.

7. Act:  
   Final action → modern core → devices/notifications.

8. Learn (lightweight):  
   Outcomes → update thresholds, patterns, comfort preferences.

---

4. Lineage plug‑in points

Each ancient lineage modifies:

- Agent rules: what counts as “pressure”, “stress”, “network break”, “orbital drift”.  
- Grid rules: how anomalies spread across zones.  
- State thresholds: how quickly it moves from Attentive → Concerned → Intervening.  
- Behaviour tree priorities: e.g. Mineral boosts boundary checks, Mycelial boosts pattern continuity.  
- Fractal parameters: rhythm, softness, “feel” of the organism.

The modern core and safety guarantees stay identical across all lineages.

---

5. Safety and constraints

- Hard constraints:  
  - Never disable safety devices.  
  - Never lock humans out.  
  - Never escalate without clear cause.  
- Soft constraints:  
  - Minimise noise (alerts, pings).  
  - Preserve domestic calm.  
  - Respect user schedules and modes (sleep, away, focus).

---

6. One‑line summary

The hybrid behavioural engine is a layered system that fuses agent‑based logic, state machines, cellular automata, behaviour trees, prediction, and fractal texture—then lets an ancient lineage plug into those layers to decide how the house feels and responds, without ever changing the underlying safety or IoT core.