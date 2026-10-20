# The AI Generalist: Facilitator Guide

Son-U Michael Paik · CEO, GRC Solutions Korea

**v2.0.2 · 20 October 2026 (KST)**

The runbook for the one-day workshop. Participants read [participant-handout.md](participant-handout.md); the tool map is [tool-map.md](tool-map.md); the learning objectives, currency note and citation are in [README.md](README.md). The control set is stated once, in the handout's section 2.4, and nothing here varies it.

## Agenda: one day, 8 hours including breaks

Times are shown for a 09:00 start; shift them as a block. Handout sections are cited by number.

| Block | Duration | Purpose | Facilitation steps with timings | Exercise | Expected artifact |
|---|---|---|---|---|---|
| 1. Contract and posture (09:00) | 90 min | Agree how the day works and why experience and context are the participant's leverage (handout 0 to 2) | Objectives read aloud and weighted by the room (10); workshop contract and Definition of Done (15); posture and the missing-context drill (25); the three doctrines and the eight controls of 2.4 (30); questions (10) | Missing-context drill (1.2); name, not role, for one live use case (2.3) | Weighted objectives list; one named owner per use case raised |
| Break (10:30) | 15 min | | | | |
| 2. Foundations and prompting (10:45) | 90 min | What an LLM is, why its failure modes are predictable and how to prompt as a professional (handout 3 to 5) | Stack map and pipeline (15); 3.3 implications including context window, RAG, agents and thinking models (15); Magic Prompt and the 4-pass workflow (20); Module 1 (30); debrief with bad prompt against improved prompt (10) | Module 1: Prompt upgrade | One Magic Prompt template per participant, stored in the agreed format |
| Lunch (12:15) | 45 min | | | | |
| 3. Tools and workflows (13:00) | 90 min | Recognize tool categories, compose governed workflows (handout 6 and 7, tool-map.md, 9 and 10) | Categories assigned to groups (10); Module 2 under the exercise data rule (35); group report-backs (15); the four mix-and-remix patterns (20); diffusion and vibe coding rules (10) | Module 2: Tool bake-off | Default-tool-by-task scorecard; one pattern chosen per group |
| Break (14:30) | 15 min | | | | |
| 4. Safe agentic work and the Tiny Servant (14:45) | 90 min | MCP, prompt injection and tool risk, then one small working workflow spec (handout 8, Modules 3 and 5) | MCP as the port and the draft-not-send rule (15); threat literacy (10); Module 3 on the ten-line template (40); Module 5 on the same spec (20); read-outs (5) | Module 3: Tiny Servant spec; Module 5: MCP threat modeling | Ten-line Tiny Servant spec with gate, logging line and named owner; top abuse cases and mitigations |
| 5. Use cases and operating plan (16:15) | 45 min | Convert the day into an operating plan (handout 11, section 13 of this guide, closing rule set) | Two or three use cases chosen for the audience (10); operating checklist worked as a group (25); closing rule set and commitments (10) | Operating checklist (section 13) | Operating plan: three use cases, named owners, allowed and forbidden data, gates, logging and evaluation |

Modules 4 (voice agent tabletop) and 5 may swap; Module 4 fits a room with intake or helpdesk work. Total 480 minutes.

## Materials and prerequisites

- Participants: a laptop, an account on at least two core assistants (tool-map.md, A) approved by their organization (Module 2 compares four; the facilitator demonstrates on screen the ones a participant has no account on) and one recurring task from their own work described in a sentence, with no Client or personal data in it.
- Facilitator: this guide, the handout printed or shared, the tool map with every link checked within the week, an account on each of the four assistants Module 2 compares, the Magic Prompt template as a fillable document, the ten-line Tiny Servant template as a fillable document and the operating checklist as a shared sheet.
- Room: projector or shared screen, a shared document for artifacts, timers visible to the facilitator.
- Pre-read, sent a week before: handout sections 0 to 2 and the learning objectives in README.md.
- Data rule for the day: synthetic inputs only in every exercise; nothing from a live matter, a Client or a person enters a tool.
- Prerequisite reading for the facilitator: [DOCTRINE.md](https://github.com/rolldabones/rolldabones/blob/main/DOCTRINE.md) sections 1 to 3 and 8, so the doctrines are taught in their stated forms.

## Teaching notes by handout section

Each note stood in the participant text at v1.1.4 as a parenthetical; the text is unchanged. Notes for the Learning Objectives refer to README.md; the others to the handout section named.

### Learning Objectives (README.md)
- Read the objectives aloud. Ask participants to pick one objective they care about most. Use that to weight time allocation.

### 1) Workshop posture
- 1.1 Become an AI Generalist to surf the tsunami: Make the promise explicit. This is a repeatable operating method, not hype.
- 1.2 Your leverage is experience and context: Run the “missing context” drill: “Draft a policy.” Then ask: “What does the model not know about our regulators, customers, systems and internal risk appetite?” Capture answers.
- 1.3 Learn by building, but govern the build: Curiosity is allowed. Production changes require controls and sign-off.

### 2) Slow AI, Informed Intent, Final Liability and AI governance, risk management and compliance (AI GRC)
- 2.2 Informed Intent (authorization gate): Informed Intent is the gate before the build. An authorization missing its exit is not an authorization. Slow AI is the condition the workflow must meet before the authorization issues and for as long as it runs. If nobody can produce the authorization, the workflow is ungoverned by definition.
- 2.3 Final Liability rests with the Human (accountability rule): Ask for a name, not a role. “Who signs it” is the fastest truth test.

### 3) Foundations: what an LLM is and why failure modes are predictable
- 3.1 The “AI stack” nesting map (operational, not academic): Keep this short. The goal is operational understanding.
- 3.3 Practical implications you can use immediately: Ask: “What is the cost of being wrong here?” Use that to justify checks and gates.

### 4) Prompting as a professional skill
- 4.2 The 4-pass workflow: Demonstrate “tighten” by adding: “include failure modes, include a checklist, include escalation triggers.”
- 4.3 Common failure modes and fixes: Run “bad prompt vs improved prompt” on the same task.

### 5) Landscape: models vs assistants
- When asked “which model is best,” redirect to criteria. Safety comes from fit plus controls.

### 6) Tooling map for an AI Generalist
- Assign each category to a group to test and report back: strengths, failure modes, data touched, minimum controls.

### 7) Mix and remix: how AI Generalists build workflows
- 7.1 Pattern 1: Prompt → structured output → reuse: Have participants build one template: meeting brief, outreach email, policy draft, due diligence checklist, sales enablement memo.
- 7.2 Pattern 2: Front door prompt → backend orchestration → UI: Modularity matters. Prompt is a spec. Orchestration is control. UI is adoption.
- 7.3 Pattern 3: Voice agents with Vapi: Keep it to safe scenarios: intake, triage, scheduling, internal helpdesk.

### 8) Essential concepts for safe agentic work
- 8.1 MCP is essential: MCP is the port. What you plug into it determines capability and risk.
- 8.2 Prompt injection and tool risk (the practical version): A simple rule that works: the agent may draft, it may not send.
- 8.3 Threat literacy you can actually use: Do not overcomplicate. One habit: list tools and data access, then design gates.

### 9) Diffusion models: what to know (images and video)
- Run a corporate-safe exercise: generate a storyboard, then add a disclosure footer and a usage rule.

### 10) Vibe coding, safely
- Prototype fast, then add controls before real users touch it.

### 11) Corporate use cases (cross-functional)
- Pick 2–3 based on audience. For each: define decision owner, data classification and stop rules.

## 12) Practical exercises (workshop-ready modules)
(Teaching note: Each module is 20–40 minutes. Pick 3–5 depending on time.)

### Module 1: Prompt upgrade
- Take a synthetic task prompt
- Convert it into the Magic Prompt structure
- Add verification: assumptions, unknowns, self-check
- Compare outputs

### Module 2: Tool bake-off
- Same task across ChatGPT, Claude, Gemini, Perplexity; participants run the assistants they have accounts on and the facilitator demonstrates the rest on screen
- Score correctness, usefulness, structure and edit effort
- Choose a default tool by task type
- Exercise data rule: synthetic inputs only; no Client data, no personal data and no confidential material enters any tool during the bake-off (control 2 of participant-handout.md section 2.4)

### Module 3: Build a “Tiny Servant” workflow spec
- Choose one recurring task
- Define input fields and output schema
- Add a gate and a logging requirement
- Store as a reusable internal template

**Tiny Servants** are narrow AI services with one purpose, clear boundaries and a named owner, which do one useful task well and then stop (first public use in [*Made to Hold*](https://redcaps.substack.com/p/made-to-hold), 28 July 2026). The spec a participant leaves with is ten lines:

| Line | Field | Write |
|---|---|---|
| 1 | Purpose | the one task, in one sentence |
| 2 | Inputs | the fields it receives and from where |
| 3 | Outputs | the schema it returns and to whom |
| 4 | Boundaries | data it may touch, actions it may take, thresholds it may not cross |
| 5 | Owner | a named human with decision rights, oversight and the power to intervene |
| 6 | Exit | how it is paused, rolled back and retired |
| 7 | Evidence | what is logged: inputs, outputs, versions, approvals, exceptions |
| 8 | Review | the human gate, who reviews which outputs and when |
| 9 | Tier | the risk tier and why |
| 10 | Done-when | the acceptance test the first run must pass |

### Module 4: Voice agent tabletop
- Define a safe inbound scenario
- Write allowed actions
- Write escalation triggers
- Write post-call logging format

### Module 5: MCP threat modeling mini-session
- Pick one agent workflow
- List tool access
- Identify top abuse cases
- Add mitigations and human gates

## 13) Operating checklist for instructors and teams
(Teaching note: Use this at the end. Converts learning into an operational plan.)

1. Pick 3 priority use cases
2. Name decision owners for each
3. Define allowed data and forbidden data
4. Define human gates
5. Define logging requirements
6. Define evaluation: what good means, how you test, what breaks the build
7. Pilot with a small group
8. Review incidents and near-misses
9. Expand with change management and training

The control set is stated once, in [participant-handout.md](participant-handout.md) section 2.4; this checklist converts it into an operating plan and adds nothing to it.

---

**Final Liability rests with the Human.**
