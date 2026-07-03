# Discovery Bundle — Reference

This file is the canonical reference for concepts shared across all skills in the discovery bundle. Individual skills point here rather than re-defining shared frameworks.

---

## Bundle skills and routing

Use `discovery-guide` as the entry point for any discovery effort. It will orient you and route to the right skill.

| Where you are | Skill to use |
|---|---|
| No clear problem or outcome yet | `opportunity-framing` |
| Problem framed but no OST or strategic structure | `ost-builder` |
| Outcome unclear or defined in output terms | `outcome-framing` |
| Problem clear, need to plan research | `research-planner` |
| Research done, need to make sense of it | `research-synthesis` |
| Direction emerging, assumptions not mapped | `assumption-mapping` |
| Assumptions mapped, need solution directions | `solution-exploration` |
| Direction set, need to communicate findings | `stakeholder-communication` |
| Thinking needs to be challenged before proceeding | `discovery-coach` |
| Team isn't sure they're doing discovery at all | `discovery-coach` first |

---

## Cagan's four risk types

*Source: Marty Cagan — Inspired*

Every product direction carries four types of risk. The purpose of discovery is to eliminate them cheaply before building.

**Value risk** — Do users actually have this problem? Is it painful or frequent enough that they would change their behaviour to solve it? Is our solution one they would recognize as solving it?

**Usability risk** — Can users understand and use what we build? Will it fit how they actually work, without training or excessive behaviour change?

**Feasibility risk** — Can the team actually build this, at the quality and pace required, given current capabilities, dependencies, and technical debt?

**Viability risk** — Does solving this work for the business? Does the monetization model hold, the legal and regulatory context allow it, the economics work at scale?

The full assumption lists per risk type live in `assumption-mapping`. Every other skill refers to these types by name only.

---

## Validation theater

*Canonical anti-pattern name used across the bundle*

Validation theater is research or experimentation designed to confirm a decision already made, rather than to reduce genuine uncertainty. The output of validation theater is activity — sessions run, interviews completed, experiments shipped — not learning.

Signs you are in validation theater:
- You could describe what you'd conclude before running the study
- A negative result would not change the direction
- The research is being used to pre-sell a solution, not to stress-test it
- The team would run it regardless of what you find

If you detect validation theater, name it directly: *"This looks like validation theater — research designed to confirm a decision already made. Do you want to redesign this as genuine learning, or do you need help communicating a direction that's already set?"*

Defined canonically here; introduced in `discovery-coach`. Referenced in `research-planner` and `stakeholder-communication`.

---

## Evidence log and confidence scoring

*Canonical format used across the bundle — owned by `assumption-mapping`*

```
Assumption: [statement]
Before confidence: [1–5]
After confidence: [1–5]
Key finding: [one sentence — what was observed, not what was inferred]
Implication: [what this means for the direction]
Decision: [proceed / pivot / stop / run follow-up]
```

**Confidence scale:**

| Grade | Meaning |
|---|---|
| 1 | Single source, self-reported, no corroboration |
| 2 | 2–3 sources with similar signal, still self-reported |
| 3 | Pattern across multiple participants, at least partially observed |
| 4 | Strong pattern, directly observed behaviour, corroborated across source types |
| 5 | Repeatedly observed behaviour across diverse contexts, corroborated by quantitative signal |

Self-reported data caps at 3 unless supported by observed behaviour.

---

## JTBD forces diagram

*Source: Bob Moesta and Clayton Christensen — Jobs to Be Done*

*Canonical description — owned by `research-planner`. Referenced in `research-synthesis`.*

People "hire" products to make progress in specific circumstances. A switch interview reconstructs the timeline of a real decision or behaviour change to reveal four forces:

- **Push** — the struggle with the current situation that makes continuing with it costly
- **Pull** — the attraction of the new solution and the progress it promises
- **Anxiety** — the fear or uncertainty that slows adoption of something new
- **Habits** — the inertia of the current situation and existing behaviour patterns

The opportunity lives where push and pull are high and anxiety can be reduced. Reconstruct all four forces from a real event; do not solicit opinions.

---

## Core source texts

All skills in this bundle draw on these four texts. Individual skills cite specific concepts inline rather than re-listing the full bibliography.

- **Marty Cagan** — *Inspired* and *Empowered*: Four risk types; empowered teams; discovery as risk elimination; the purpose of prototypes
- **Melissa Perri** — *Escaping the Build Trap*: Output vs. outcome orientation; the product kata; the build trap mechanism; communicating in outcome terms
- **Teresa Torres** — *Continuous Discovery Habits*: The Opportunity Solution Tree; continuous discovery as a practice; assumption mapping and experiment design
- **Dan Brown** — *Practical Design Discovery*: Discovery briefs; naming unknowns as first-class artifacts; synthesis methods; design principles as constraints; analogue research
