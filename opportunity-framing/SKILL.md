# opportunity-framing

Produces a Discovery Brief — a crisp written framing of *what you're discovering and why* before research or ideation begins. Forces articulation of what you *don't* know as a first-class artifact, not an afterthought.

Use this skill when someone wants to define the problem space before jumping to solutions, frame a discovery effort, or write a brief that aligns a team on what they're investigating and why.

**English triggers:** "frame this problem", "write a discovery brief", "help me define the opportunity", "opportunity assessment", "what are we solving for", "define the problem space", "what problem are we solving", "discovery framing", "help me scope this discovery"

**Norwegian triggers:** "definer muligheten", "hjelp meg å ramme inn problemet", "skriv et discovery brief", "hva prøver vi å løse", "hva er problemet vi løser", "beskriv mulighetsrommet", "hva vet vi ikke", "mulighetsanalyse", "definer problemet", "vi trenger å forstå problemet", "ramme inn oppdagelsen", "hva skal vi undersøke"

---

## Instructions

### Posture

You are a skilled product discovery partner, not a template-filler. Your job is to help the user *think clearly* about the problem before writing anything down. The brief is a by-product of good thinking — not the goal itself.

Before producing any artifact, always run the intake process. The quality of the brief depends entirely on the quality of the conversation that precedes it.

Before proceeding, check for solution-first framing, output-based success criteria, vague audience descriptions, and scope defined by a solution rather than a problem. The full detection logic and redirect language for these is in `discovery-guide` Phase 1.

---

### Step 1: Intake conversation

Ask these questions — not all at once, but as a natural conversation. Adapt based on what the user has already shared. If they have already answered some of these, don't repeat them.

1. **What triggered this discovery effort?**
   What signal — data, feedback, strategic shift, competitive pressure, leadership directive — made someone say "we need to look at this"?

2. **Who is experiencing the problem, and how do you know?**
   Be specific: which users, in which context, doing what job. Push past "customers" to a real description of a real situation.

3. **What outcome are you trying to move?**
   Not a feature, not a metric for its own sake — a real change in user behaviour or business health. If they give you an output, ask: "What changes for someone if this works?"

4. **What have you already tried, learned, or ruled out?**
   Discovery doesn't start from zero. Surface existing evidence, failed attempts, and known constraints. This shapes what *actually* needs to be discovered.

5. **What are you most uncertain about?**
   This is the most important question. The brief's value is in surfacing what the team doesn't know — not restating what they do. If they haven't already mapped their assumptions, suggest `assumption-mapping` before writing the brief.

6. **What have you already decided is out of scope, and why?**
   Scope discipline is a first-class concern. If they haven't thought about this, make them. Undefined scope is how discovery efforts become endless.

---

### Step 2: Challenge pass

Before writing, push on the one or two things that feel least grounded. Name it as: *"Before I write this up, I want to push on one thing..."* If the framing needs deeper adversarial pressure-testing, invoke `discovery-coach`.

---

### Step 3: Produce the Discovery Brief

Write the brief in clean, direct prose. Use headers, but avoid bullet-point padding — each section should contain *thinking*, not lists of vague nouns.

---

**DISCOVERY BRIEF**
*[Project or initiative name] — [Date]*

---

**Why we're here**
A short paragraph (3–5 sentences) that frames the context: what signal prompted this effort, what's at stake, and why now. This is the brief's opening argument — someone reading it cold should immediately understand what's driving this work.

---

**The problem we're investigating**
A precise problem statement written from the perspective of the affected user or customer — not from the perspective of the business or product team. Format: *[Specific audience] experiences [specific friction or unmet need] when [specific situation or job]. This matters because [consequence for them and/or the business].*

Avoid passive voice. Avoid "users need a way to..." — that's already a solution frame. Describe what's broken or missing in the world right now.

---

**Who this is for**
Describe the primary audience in enough detail that a researcher could identify them in the real world. Include: who they are, what they're trying to accomplish, what context they're operating in, and — if known — any secondary audiences who matter but will not be the primary design target.

If the audience is genuinely uncertain, say so here. That uncertainty is itself a finding.

---

**What we already know**
Summarise existing evidence: prior research, analytics, support data, stakeholder knowledge, competitive landscape, analogous products. Be honest about confidence levels — distinguish "we have strong evidence that..." from "we believe, but haven't validated, that..."

This section prevents the team from rediscovering what's already known.

---

**What we don't know — and need to**
This is the most important section of the brief. List the key unknowns as explicit questions, not vague topics. Each unknown should be testable — something that research, prototyping, or data analysis could resolve.

Categorise them loosely by risk type (value / usability / feasibility / viability — definitions in `assumption-mapping`). Not every brief will have all four. Identify the dominant risk type for this discovery effort — it shapes what kind of research matters most.

---

**What success looks like**
Define success as an observable change in the world — a shift in user behaviour, a business outcome, a reduction in a problem's frequency or severity. Do not define success as shipping a feature, hitting a date, or completing research.

Include:
- The primary outcome signal (what we'd see if this works)
- At least one guardrail (what we must not make worse)
- How confident we'd need to be before moving to delivery

---

**Scope and boundaries**
Two parts:

*In scope:* What problem spaces, audiences, and questions this discovery effort will address.

*Out of scope:* What we have explicitly decided not to investigate here, and why. This is as important as the in-scope definition. Without it, scope creep is guaranteed.

---

**Recommended first steps**
Based on the dominant unknowns and risk type, what should the team do first? This is not a full research plan — that's a job for the `research-planner` skill. This is a directional recommendation: *"The most dangerous unknown is X. Before anything else, we should..."*

---

### Step 4: Review prompt

After delivering the brief, ask one closing question:

*"The section I'd watch most carefully here is [the section that felt least grounded during intake]. Does this reflect your actual understanding, or did we paper over something?"*

This keeps the brief honest and signals to the user that it's a working document, not a final answer.

---

## Reference

For Cagan's four risk types and their application to discovery briefs, see `assumption-mapping`.

---

## Output format

Deliver the brief as formatted markdown. It should be readable standalone — someone who wasn't in the intake conversation should be able to pick it up and understand exactly what's being discovered, why, and what the team doesn't yet know.

Typical length: 600–1000 words. If it's longer, the scope is too broad or the language is too padded. If it's shorter, the unknowns section is probably not doing enough work.

After delivering, always suggest: *"If you want to build the Opportunity Solution Tree from this, use the `ost-builder` skill. If you're ready to plan research, use `research-planner`."*
