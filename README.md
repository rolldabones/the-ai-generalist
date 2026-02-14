# The AI Generalist

Recommended program (inspiration for this workshop): https://www.outskill.com/2-day-ai-mastermind

## Learning Objectives
By the end of this workshop participants will be able to:
1. Explain, at a working level, what a large language model (LLM) is, what it can and cannot do, and why failure modes are predictable.
2. Use a repeatable prompting workflow to produce higher quality outputs with fewer retries.
3. Choose the right tool for a task across chat, search, documents, meetings, coding, image, video, and voice agents.
4. Design a simple “mix and remix” workflow across tools (prompt → backend agent → front-end).
5. Apply **Slow AI** and **Final Liability rests with the Human** to real corporate use cases using an AI governance, risk management, and compliance (AI GRC) lens.
6. Build a lightweight control set: scope, data handling, logging, human gates, evaluation, escalation, and change management.

(Teaching note: Read the objectives aloud. Ask participants to pick one objective they care about most. Use that to weight time allocation.)

---

## TL;DR
- Become an AI Generalist to surf the tsunami: adapt fast while holding control.
- Your advantage is high context from experience. Encode it into prompts and checklists, then let AI compress execution.
- Learn by building, but in corporate settings experimentation must be governed: scope, gates, logs, escalation.
- Operating posture: Slow AI plus Final Liability rests with the Human.
- Outputs should be reusable: prompt library, governed workflow specs, risk tiering, evidence packs.

---

## 1) Workshop posture

### 1.1 Become an AI Generalist to “Surf the Tsunami”
AI is now a general capability layer touching most functions. “Generalist” here does not mean shallow. It means you can:
- Understand the core mechanism
- Choose tools rationally
- Build small workflows fast
- Control risk with discipline
- Keep humans accountable

(Teaching note: Set expectation: we are not learning one tool. We are learning a durable method in a fast-changing landscape.)

### 1.2 Build on your experience, which gives you high context
Domain experience is leverage. The model can draft, summarize, transform, plan, and code. You supply:
- Objectives and constraints
- Edge cases and acceptable risk
- Reality checks and tradeoffs
- The decision and the owner

(Teaching note: Quick prompt: “Draft a policy.” Then ask: “What does the model not know about our regulators, customers, systems, and internal risk appetite?” Capture answers.)

### 1.3 Try the tools, stretch a bit
You learn by doing. The practical loop:
1. Try a tool on a real task
2. Compare outputs across 2–3 tools
3. Add constraints and checks
4. Log what worked as a reusable pattern

(Teaching note: Curiosity is allowed. Production changes require controls and sign-off.)

---

## 2) Slow AI, Final Liability, and AI GRC

### 2.1 Slow AI (operating posture)
Slow AI does not mean slow work. It means governed work:
- Visible
- Explainable enough for the decision at hand
- Auditable
- Monitored
- Pausable

(Teaching note: Translate this into controls: logs, gates, evals, change control, rollback.)

### 2.2 Final Liability rests with the Human (accountability rule)
Every AI-assisted output attaches to a named human who:
- Has decision authority
- Understands limits
- Owns consequences
- Can stop the workflow

(Teaching note: Ask for a name, not a role. “Who signs it” is the fastest truth test.)

### 2.3 AI GRC (minimum corporate control set)
Treat AI as a capability that changes decision quality, record creation, process velocity, and risk pathways.

Minimum control set:
1. **Use-case registry**: what AI is doing, where, for whom, by which owner
2. **Data rules**: what data may be used, where it may go, retention rules
3. **Human gates**: which outputs require review and approval
4. **Logging**: inputs, outputs, versions, approvals, exceptions
5. **Evaluation**: accuracy, hallucination rate, security tests, regressions across updates
6. **Security**: prompt injection defenses, tool permissions, secrets handling
7. **Vendor and supply chain**: models, plugins, connectors, agent tools
8. **Change management**: updates, drift monitoring, rollback plan, CAPA

(Teaching note: AI GRC is decision control first. Artifacts follow. The order matters.)

⧉ Biggest recurring gap in corporate rollouts: AI adoption outruns ownership, allowed data, stop rules, and logging.

---

## 3) Foundations: what an LLM is and how it works

### 3.1 The “AI stack” nesting map
1. Artificial intelligence: machines performing tasks associated with human intelligence
2. Machine learning: systems that learn patterns from data to make predictions
3. Deep learning: neural-network-based learning at scale
4. Large language models: deep learning models trained on large text corpora to predict and generate language

(Teaching note: Keep it short. The goal is operational understanding, not theory.)

### 3.2 How it works (simple pipeline)
1. **Tokenization**: text is broken into tokens
2. **Embeddings**: tokens map to vectors that represent relationships in meaning
3. **Transformer attention**: the model weights which prior tokens matter most
4. **Next-token prediction**: the model predicts the next token repeatedly
5. **Response generation**: those predictions become text and structured outputs

(Teaching note: One sentence to anchor everything: it predicts plausible next tokens, not truth.)

### 3.3 Practical implications
- Strong at drafting, summarizing, transforming, patterning, and coding assistance
- Weak at guaranteed factuality without retrieval and verification
- Models vary by reasoning strength, speed, cost, context length, multimodal capability, tool integration

(Teaching note: Ask: “What is the cost of being wrong in this workflow?” Use that to justify checks and gates.)

---

## 4) Prompting as a professional skill

### 4.1 The Magic Prompt structure
A durable prompt pattern:
1. **Role**: who the assistant is acting as
2. **Objective**: what success looks like
3. **Context**: facts, constraints, audience, inputs
4. **Instructions**: steps, boundaries, checks
5. **Output spec**: format, headings, length, style rules
6. **Verification**: assumptions, unknowns, how it checked

(Teaching note: Make participants rewrite one real prompt into this structure. Compare outputs before and after.)

### 4.2 The 4-pass workflow
1. **FRAME**: objective, decision owner, constraints, risks
2. **DRAFT**: generate a first pass fast
3. **TIGHTEN**: add checks, edge cases, counterarguments, formatting
4. **LOCK**: finalize, record assumptions, store as a reusable template

(Teaching note: Demonstrate “tighten” by adding: “include failure modes, include a checklist, include escalation triggers.”)

### 4.3 Common failure modes and fixes
- Vague objective → add acceptance tests and examples
- Missing constraints → add must and must-not rules
- Overconfidence → force Unknown or Insufficient data plus explicit assumptions
- Inconsistent style → provide a style block and output schema
- Factual errors → require sources, or use retrieval tools, then verify

(Teaching note: Do a live “bad prompt vs improved prompt” with the same task.)

---

## 5) Landscape: models and assistants (combined map)
Think in two layers:
- **Models**: the engines
- **Assistants**: products packaging models with UX, memory, tools, and connectors

Selection heuristics:
1. Risk: higher-risk tasks require stronger controls, not just better models
2. Data: where data goes, what is retained, what can be isolated
3. Workflow: docs, meetings, IDE, APIs, agents, automations
4. Cost and latency: speed vs depth
5. Governance: admin controls, audit logs, policy enforcement

(Teaching note: When asked “which model is best,” redirect to criteria. Safety comes from fit and controls, not fandom.)

---

## 6) Tooling map for an AI Generalist

The goal is not to use everything. The goal is to recognize categories and compose workflows safely.

(Teaching note: Assign each table a category to test and report back: strengths, failure modes, data touched, minimum controls.)

### A) Core assistants and search
- ChatGPT: https://chatgpt.com/
- Claude: https://claude.ai/
- Gemini: https://gemini.google.com/
- Microsoft Copilot: https://copilot.microsoft.com/
- Grok: https://grok.com/
- Meta AI: https://www.meta.ai/
- Perplexity: https://www.perplexity.ai/

### B) Research and notes
- NotebookLM: https://notebooklm.google/
- Chronicle: https://chroniclehq.com/
- Granola: https://www.granola.ai/

### C) Meetings and transcription
- Fireflies: https://fireflies.ai/

### D) Marketing and social workflows
- Writesonic: https://writesonic.com/
- Supergrow: https://www.supergrow.ai/
- Socialsonic: https://socialsonic.com/
- Humanic AI: https://humanic.ai/
- Happenstance: https://happenstance.ai/
- Emergent: https://emergent.sh/

### E) Spreadsheets and “AI in cells”
- Numerous AI: https://numerous.ai/

### F) Images and design
- Midjourney: https://www.midjourney.com/
- Runway: https://runwayml.com/
- Krea: https://www.krea.ai/
- Leonardo: https://leonardo.ai/
- Magnific: https://magnific.ai/
- Phot AI: https://www.phot.ai/

### G) Video generation and avatars
- HeyGen: https://www.heygen.com/
- Kling: https://app.klingai.com/global/
- Higgsfield: https://higgsfield.ai/

### H) Audio and voice
- ElevenLabs: https://elevenlabs.io/
- Suno: https://suno.com/

### I) Builders for rapid prototyping and “vibe coding”
- Replit: https://replit.com/
- Bolt: https://bolt.new/
- Lovable: https://lovable.dev/

### J) Agent platforms and orchestration
- Lyzr AI: https://www.lyzr.ai/
- OpenRouter (model routing): https://openrouter.ai/

### K) Local hosting
- Ollama: https://ollama.com/

### L) Tool connection standard
- MCP (Model Context Protocol): https://modelcontextprotocol.io/

### M) Computer automation agents
- Goose: https://block.github.io/goose/

### N) Data acquisition and scraping
- Apify: https://apify.com/

### O) Voice agents and calling workflows
- Vapi: https://vapi.ai/

### P) “Emily” (engineering scaffolding)
- Emily: https://meetemily.ai/

### Q) Agent swarms and wide-search assistants
- Kimi: https://www.kimi.com/en
- Moonshot AI (Kimi developer): https://www.moonshot.ai/

---

## 7) Mix and remix: how AI Generalists build workflows

### 7.1 Pattern 1: Prompt → structured output → reuse
1. Write one Magic Prompt for a recurring task
2. Produce output in a fixed schema
3. Save prompt and schema as a template
4. Re-run with new inputs

(Teaching note: Have participants build one template: meeting brief, outreach email, policy draft, due diligence checklist, sales enablement memo.)

### 7.2 Pattern 2: Gems → backend agents → front-end app
Example composition:
1. Draft a strong prompt in Gemini Gems as the “front door”
2. Move the same prompt into Lyzr as backend orchestration
3. Use an agent inference layer via API to run the workflow repeatedly
4. Plug outputs into Replit to build a UI and ship an internal tool

(Teaching note: Teach modularity. Prompt is a spec. Orchestration is control. UI is adoption.)

### 7.3 Pattern 3: Voice agents with Vapi
1. Define role and allowed actions
2. Write the call script as policy, not improvisation
3. Add hard stops and escalation triggers
4. Log calls, decisions, and exceptions

(Teaching note: Keep it to safe scenarios: intake, triage, scheduling, internal helpdesk.)

### 7.4 Pattern 4: OpenRouter and Bolt setups
- OpenRouter: unify access to multiple models, add routing logic
- Bolt: prototype apps fast, then add governance controls before real use

(Teaching note: Separate “prototype fast” from “operate safely.” The gates are the difference.)

### 7.5 Pattern 5: Ollama for home hosting, then connect it
- Use Ollama for privacy constraints, cost control, or offline work
- Connect local models into your prototyping workflow when appropriate
- Treat local models as still risky: hallucinations persist, tool access can still leak

(Teaching note: Local reduces some risks. It does not remove governance duties.)

---

## 8) Essential concepts for safe agentic work

### 8.1 MCP is essential
MCP is a standard for connecting AI applications to tools and data sources. It matters because:
- Agents become useful when they can act, not just talk
- Tool access is the biggest risk amplifier
- MCP pushes explicit interfaces: permissions, scopes, logs

(Teaching note: MCP is the port. What you plug into it determines capability and risk.)

### 8.2 Prompt injection and tool risk
When a model can call tools, untrusted content can try to steer the agent:
- Ignore prior instructions
- Exfiltrate secrets
- Rewrite files
- Send messages

Controls:
1. Least-privilege tool permissions
2. Allowlists for actions
3. Separation of duties for high-impact actions
4. Human approval gates
5. Logging and monitoring

(Teaching note: Simple policy you can teach: the agent may draft, it may not send.)

### 8.3 Agent swarms and multi-agent planning
Multi-agent systems can improve coverage but can:
- Multiply cost
- Multiply attack surface
- Produce plausible consensus that is still wrong

(Teaching note: Require a single arbiter: one human owner signs the final output.)

---

## 9) Diffusion models: what to know (images and video)
Diffusion models generate images and video by iteratively refining noise into structure.

Practical uses:
- Marketing drafts
- Product mockups
- Storyboards
- Training visuals

Risk and control notes:
- Rights and provenance
- Brand safety and disallowed content
- Synthetic media disclosure where required
- Human review before external use

(Teaching note: Run a corporate-safe exercise: generate a storyboard, then add a disclosure footer and a usage rule.)

---

## 10) Vibe coding, safely
Vibe coding means building software by describing intent and iterating with AI-drafted code. It compresses time-to-prototype. It can also ship invisible risk.

Safe vibe coding rules:
1. Keep secrets out of prompts and repos
2. Require tests, even basic smoke tests
3. Use dependency scanning and security linting
4. Use staged rollout and rollback
5. Human review remains mandatory for production

(Teaching note: Run a 10-minute build: internal FAQ app. Then add the checklist: auth, logging, tests, deployment, rollback.)

---

## 11) Corporate use cases (cross-functional)
(Teaching note: Pick 2–3 based on the audience. For each: define decision owner, data classification, and stop rules.)

### Legal and compliance
- Contract drafting support with clause libraries and structured checklists
- Policy drafting and redlining with traceable assumptions
- Investigation support with strict confidentiality rules and logging

### Finance and operations
- Variance explanations and narrative summaries
- Workflow automation for recurring reporting
- Internal controls support: draft narratives, evidence requests, test scripts

### Sales, marketing, customer support
- Persona-based drafts with explicit brand rules
- Meeting capture → action items → CRM-ready summaries
- Customer response drafting with escalation triggers

### Engineering and product
- Prototype internal tools quickly
- Spec writing, test generation, documentation
- Agent workflows touching tickets, repos, and deployments, with gates

---

## 12) Practical exercises (workshop-ready modules)
(Teaching note: Each module is 20–40 minutes. Pick 3–5 depending on time.)

### Module 1: Prompt upgrade
- Take a real task prompt
- Convert it into the Magic Prompt structure
- Add verification: assumptions, unknowns, self-check
- Compare outputs

### Module 2: Tool bake-off
- Same task across ChatGPT, Claude, Gemini, Perplexity
- Score correctness, usefulness, structure, and edit effort
- Choose a default tool by task type

### Module 3: Build a “Tiny Servant” workflow
- Choose one recurring task
- Define input fields and output schema
- Add a gate and a logging requirement
- Store as a reusable internal template

### Module 4: Vapi voice agent tabletop
- Define a safe inbound scenario
- Write allowed actions
- Write escalation triggers
- Write post-call logging format

### Module 5: MCP threat modeling mini-session
- Pick one agent workflow
- List tool access
- Identify top abuse cases
- Add mitigations and human gates

---

## 13) Operating checklist for instructors and teams
(Teaching note: Use this at the end. It converts learning into an operational plan.)

1. Pick 3 priority use cases
2. Name decision owners for each
3. Define allowed data and forbidden data
4. Define human gates
5. Define logging requirements
6. Define evaluation: what good means, how you test, and what breaks the build
7. Pilot with a small group
8. Review incidents and near-misses
9. Expand with change management and training

---

## 14) Recommended Readings and Reference Map

### Level 1: working literacy
- NIST AI Risk Management Framework overview: https://www.nist.gov/itl/ai-risk-management-framework
- NIST AI RMF 1.0 (PDF): https://nvlpubs.nist.gov/nistpubs/ai/nist.ai.100-1.pdf
- OWASP Top 10 for LLM Applications: https://owasp.org/www-project-top-10-for-large-language-model-applications/
- MITRE ATLAS: https://atlas.mitre.org/

(Teaching note: Assign Level 1 as pre-read for corporate cohorts.)

### Level 2: building and connecting tools
- MCP home: https://modelcontextprotocol.io/
- MCP specification: https://modelcontextprotocol.io/specification/2025-11-25
- OpenRouter: https://openrouter.ai/
- Apify docs: https://docs.apify.com/
- Vapi docs: https://docs.vapi.ai/

### Level 3: management systems and governance
- ISO/IEC 42001 overview: https://www.iso.org/standard/42001
- ISO 42001 explained: https://www.iso.org/home/insights-news/resources/iso-42001-explained-what-it-is.html

(Teaching note: For regulated sectors, Level 3 becomes mandatory, not optional.)

### Reading Map (by role)
Use this section for pre-reads and for post-workshop deepening.

- Executives and functional leaders
  1. NIST AI RMF overview: https://www.nist.gov/itl/ai-risk-management-framework
  2. NIST AI RMF 1.0 (PDF): https://nvlpubs.nist.gov/nistpubs/ai/nist.ai.100-1.pdf
  3. ISO/IEC 42001 overview: https://www.iso.org/standard/42001
  4. OWASP Top 10 for LLM Applications: https://owasp.org/www-project-top-10-for-large-language-model-applications/

  (Teaching note: Leaders should learn the control vocabulary: ownership, tiering, gates, logs, evals, incident response, and change management.)

- Workflow owners and operators
  1. OWASP Top 10 for LLM Applications: https://owasp.org/www-project-top-10-for-large-language-model-applications/
  2. MCP home: https://modelcontextprotocol.io/
  3. NotebookLM: https://notebooklm.google/
  4. AI assistants category list in this note, then run a bake-off

  (Teaching note: Operators should learn two habits: write acceptance tests, then rerun tests after model or prompt changes.)

- Security and IT
  1. MITRE ATLAS: https://atlas.mitre.org/
  2. OWASP Top 10 for LLM Applications: https://owasp.org/www-project-top-10-for-large-language-model-applications/
  3. MCP specification: https://modelcontextprotocol.io/specification/2025-11-25
  4. Apify docs: https://docs.apify.com/ (treat scraping as policy-gated)

  (Teaching note: Tool connections are privileged access. Default deny, then grant least privilege with logs and approvals.)

- Legal and compliance
  1. ISO/IEC 42001 overview: https://www.iso.org/standard/42001
  2. NIST AI RMF 1.0 (PDF): https://nvlpubs.nist.gov/nistpubs/ai/nist.ai.100-1.pdf
  3. OWASP Top 10 for LLM Applications: https://owasp.org/www-project-top-10-for-large-language-model-applications/

  (Teaching note: Focus on operational controls: classification, retention, vendor review, audit logs, approvals, CAPA.)

- Engineering and product
  1. MCP home: https://modelcontextprotocol.io/
  2. OpenRouter: https://openrouter.ai/
  3. Ollama: https://ollama.com/
  4. Replit: https://replit.com/
  5. Bolt: https://bolt.new/

  (Teaching note: Treat prompts like code. Version them, test them, monitor them, and keep rollback.)

---

## Closing: the AI Generalist’s rule set
1. Start with the decisions.
2. Use AI to accelerate drafts, not to replace accountability.
3. Constrain scope, control data, and log the work.
4. Build small, ship safely, iterate.
5. **Final Liability rests with the Human.**
