The AI Generalist

Recommended program (inspiration): https://www.outskill.com/2-day-ai-mastermind

Learning Objectives

By the end of this workshop participants will be able to:
	1.	Explain, at a working level, what a large language model (LLM) is, what it can and cannot do, and why failure modes are predictable.
	2.	Use a repeatable prompting workflow to produce higher quality outputs with fewer retries.
	3.	Choose the right tool for a task across chat, search, documents, meetings, coding, image, video, and voice agents.
	4.	Design a simple “mix and remix” workflow across tools (prompt → backend agent → front-end).
	5.	Apply Slow AI and Final Liability rests with the Human to real corporate use cases using an AI governance, risk management, and compliance (AI GRC) lens.
	6.	Build a lightweight control set: scope, data handling, logging, human gates, evaluation, escalation, and change management.

(Teaching note: Read the objectives aloud. Ask participants to pick one objective they care about most. Use that to weight time allocation.)

⸻

0) Workshop contract: how we work today

0.1 Mode
	•	This is not a “one tool” class.
	•	We are building a durable method that survives tool churn.

0.2 Outcome

Participants leave with:
	•	A reusable prompting workflow
	•	A tool selection map
	•	A minimum governance control set
	•	One small, working workflow spec they can reuse at work

0.3 Definition of Done

This note should be usable as:
	•	Participant primer
	•	Instructor runbook
	•	Reference map with live links

⸻

1) Workshop posture

1.1 Become an AI Generalist to surf the tsunami

AI is now a general capability layer across functions. “Generalist” does not mean shallow. It means you can:
	•	Understand the core mechanism
	•	Choose tools rationally
	•	Build small workflows fast
	•	Control risk with discipline
	•	Keep humans accountable

(Teaching note: Make the promise explicit. This is a repeatable operating method, not hype.)

1.2 Your leverage is experience and context

Models can draft, summarize, transform, plan, and assist with code. You supply:
	•	Objectives and constraints
	•	Edge cases and acceptable risk
	•	Reality checks and tradeoffs
	•	The decision and the owner

(Teaching note: Run the “missing context” drill: “Draft a policy.” Then ask: “What does the model not know about our regulators, customers, systems, and internal risk appetite?” Capture answers.)

1.3 Learn by building, but govern the build

Practical loop:
	1.	Try a tool on a real task
	2.	Compare outputs across 2–3 tools
	3.	Add constraints and checks
	4.	Log what worked as a reusable pattern

(Teaching note: Curiosity is allowed. Production changes require controls and sign-off.)

⸻

2) Slow AI, Final Liability, and AI GRC

2.1 Slow AI (operating posture)

Slow AI does not mean slow work. It means governed work:
	•	Visible
	•	Explainable enough for the decision at hand
	•	Auditable
	•	Monitored
	•	Pausable

Translate posture into controls:
	•	Versioning (prompt, model, tools)
	•	Logging (inputs, outputs, approvals, exceptions)
	•	Evaluation (before and after changes)
	•	Change control (roll forward, roll back)
	•	Stop rules (when the workflow must halt)

2.2 Final Liability rests with the Human (accountability rule)

Every AI-assisted output attaches to a named human who:
	•	Has decision authority
	•	Understands limits
	•	Owns consequences
	•	Can stop the workflow

(Teaching note: Ask for a name, not a role. “Who signs it” is the fastest truth test.)

2.3 AI GRC minimum control set

Treat AI as a capability that changes decision quality, record creation, process velocity, and risk pathways.

Minimum control set (workable in most organizations):
	1.	Use-case registry: what AI is doing, where, for whom, by which owner
	2.	Data rules: what data may be used, where it may go, retention rules
	3.	Human gates: which outputs require review and approval
	4.	Logging: inputs, outputs, versions, approvals, exceptions
	5.	Evaluation: accuracy, hallucination rate, regressions after updates
	6.	Security: prompt injection defenses, tool permissions, secrets handling
	7.	Vendor and supply chain: models, plugins, connectors, agent tools
	8.	Change management: updates, drift monitoring, rollback plan, CAPA (corrective and preventive action)

NIST AI RMF overview: https://www.nist.gov/itl/ai-risk-management-framework  ￼
NIST AI RMF 1.0 (PDF): https://nvlpubs.nist.gov/nistpubs/ai/nist.ai.100-1.pdf  ￼

⧉ Biggest recurring gap: adoption outruns ownership, allowed data, stop rules, and logging.

⸻

3) Foundations: what an LLM is and why failure modes are predictable

3.1 The “AI stack” nesting map (operational, not academic)
	1.	Artificial intelligence: machines doing tasks associated with human intelligence
	2.	Machine learning: systems learning patterns from data to make predictions
	3.	Deep learning: neural networks at scale
	4.	Large language models: deep learning models trained on large text corpora to predict and generate language

(Teaching note: Keep this short. The goal is operational understanding.)

3.2 How an LLM works (simple pipeline)
	1.	Tokenization: text is broken into tokens
	2.	Embeddings: tokens map to vectors capturing relationships in meaning
	3.	Transformer attention: model weights which prior tokens matter most
	4.	Next-token prediction: model predicts the next token repeatedly
	5.	Response generation: predictions become text, code, or structured outputs

Anchor sentence:
	•	An LLM predicts plausible next tokens, not truth.

3.3 Practical implications you can use immediately
	•	Strong at drafting, summarizing, transforming, patterning, and code assistance
	•	Weak at guaranteed factuality without retrieval and verification
	•	Output quality depends heavily on constraints, context, and evaluation

(Teaching note: Ask: “What is the cost of being wrong here?” Use that to justify checks and gates.)

⸻

4) Prompting as a professional skill

4.1 The Magic Prompt structure

A durable pattern:
	1.	Role: who the assistant is acting as
	2.	Objective: what success looks like
	3.	Context: facts, constraints, audience, inputs
	4.	Instructions: steps, boundaries, checks
	5.	Output spec: format, headings, length, style rules
	6.	Verification: assumptions, unknowns, how it checked

4.2 The 4-pass workflow
	1.	FRAME: objective, decision owner, constraints, risk tier, stop rules
	2.	DRAFT: generate a first pass fast
	3.	TIGHTEN: add checks, edge cases, counterarguments, formatting, tests
	4.	LOCK: finalize, record assumptions, store as a reusable template

(Teaching note: Demonstrate “tighten” by adding: “include failure modes, include a checklist, include escalation triggers.”)

4.3 Common failure modes and fixes
	•	Vague objective → add acceptance tests and examples
	•	Missing constraints → add must and must-not rules
	•	Overconfidence → force “Unknown/Insufficient data” plus explicit assumptions
	•	Inconsistent style → provide an output schema and style block
	•	Factual errors → require sources, or use retrieval, then verify

(Teaching note: Run “bad prompt vs improved prompt” on the same task.)

Helpful references:
	•	OpenAI prompt engineering guide: https://platform.openai.com/docs/guides/prompt-engineering
	•	OpenAI evals guide: https://platform.openai.com/docs/guides/evals

⸻

5) Landscape: models vs assistants

Think in two layers:
	•	Models: engines (capabilities, context length, latency, cost)
	•	Assistants: products packaging models with UX, memory, tools, and connectors

Selection heuristics:
	1.	Risk: higher-risk tasks require stronger controls, not just “better models”
	2.	Data: where data goes, what is retained, what can be isolated
	3.	Workflow: docs, meetings, IDE, APIs, agents, automations
	4.	Cost and latency: speed vs depth
	5.	Governance: admin controls, audit logs, policy enforcement

(Teaching note: When asked “which model is best,” redirect to criteria. Safety comes from fit plus controls.)

⸻

6) Tooling map for an AI Generalist

Goal: not to use everything. Goal: recognize categories and compose workflows safely.

(Teaching note: Assign each table a category to test and report back: strengths, failure modes, data touched, minimum controls.)

A) Core assistants and search
	•	ChatGPT: https://chatgpt.com/
	•	Claude: https://claude.ai/
	•	Gemini: https://gemini.google.com/
	•	Microsoft Copilot: https://copilot.microsoft.com/
	•	Grok: https://grok.com/
	•	Meta AI: https://www.meta.ai/
	•	Perplexity: https://www.perplexity.ai/

B) Research and notes
	•	NotebookLM: https://notebooklm.google/
	•	Chronicle: https://chroniclehq.com/
	•	Granola: https://www.granola.ai/

C) Meetings and transcription
	•	Fireflies: https://fireflies.ai/

D) Marketing and social workflows
	•	Writesonic: https://writesonic.com/
	•	Supergrow: https://www.supergrow.ai/
	•	Socialsonic: https://socialsonic.com/
	•	Humanic AI: https://humanic.ai/
	•	Happenstance: https://happenstance.ai/
	•	Emergent: https://emergent.sh/

E) Spreadsheets and “AI in cells”
	•	Numerous AI: https://numerous.ai/

F) Images and design
	•	Midjourney: https://www.midjourney.com/
	•	Runway: https://runwayml.com/
	•	Krea: https://www.krea.ai/
	•	Leonardo: https://leonardo.ai/
	•	Magnific: https://magnific.ai/
	•	Phot AI: https://www.phot.ai/

G) Video generation and avatars
	•	HeyGen: https://www.heygen.com/
	•	Kling: https://app.klingai.com/global/
	•	Higgsfield: https://higgsfield.ai/

H) Audio and voice
	•	ElevenLabs: https://elevenlabs.io/
	•	Suno: https://suno.com/

I) Builders for rapid prototyping and “vibe coding”
	•	Replit: https://replit.com/
	•	Bolt: https://bolt.new/
	•	Lovable: https://lovable.dev/

J) Agent platforms and orchestration
	•	Lyzr AI: https://www.lyzr.ai/
	•	OpenRouter: https://openrouter.ai/

K) Local hosting
	•	Ollama: https://ollama.com/

L) Tool connection standard
	•	MCP (Model Context Protocol): https://modelcontextprotocol.io/

M) Computer automation agents
	•	Goose: https://block.github.io/goose/

N) Data acquisition and scraping
	•	Apify: https://apify.com/
	•	Apify docs: https://docs.apify.com/

O) Voice agents and calling workflows
	•	Vapi: https://vapi.ai/
	•	Vapi docs: https://docs.vapi.ai/

P) “Emily” (engineering scaffolding)
	•	Emily: https://meetemily.ai/

Q) Agent swarms and wide-search assistants
	•	Kimi: https://www.kimi.com/en
	•	Moonshot AI: https://www.moonshot.ai/

⸻

7) Mix and remix: how AI Generalists build workflows

7.1 Pattern 1: Prompt → structured output → reuse
	1.	Write one Magic Prompt for a recurring task
	2.	Produce output in a fixed schema
	3.	Save prompt and schema as a template
	4.	Re-run with new inputs

(Teaching note: Have participants build one template: meeting brief, outreach email, policy draft, due diligence checklist, sales enablement memo.)

7.2 Pattern 2: Front door prompt → backend orchestration → UI

Example composition:
	1.	Draft a strong “front door” prompt (fixed inputs, fixed outputs)
	2.	Move the same prompt into an orchestration layer with tool permissions
	3.	Run the workflow repeatedly with logs and evaluations
	4.	Plug outputs into a simple UI for adoption

(Teaching note: Modularity matters. Prompt is a spec. Orchestration is control. UI is adoption.)

7.3 Pattern 3: Voice agents with Vapi
	1.	Define role and allowed actions
	2.	Write the call script as policy, not improvisation
	3.	Add hard stops and escalation triggers
	4.	Log calls, decisions, and exceptions

(Teaching note: Keep it to safe scenarios: intake, triage, scheduling, internal helpdesk.)

7.4 Pattern 4: Local hosting when privacy constraints are real
	•	Use local models for privacy, cost control, or offline work
	•	Treat local models as still risky: hallucinations persist, tool access can still leak
	•	Keep the same controls: gates, logs, evals, rollback

⸻

8) Essential concepts for safe agentic work

8.1 MCP is essential

MCP is a standard for connecting AI applications to tools and data sources.
	•	MCP home: https://modelcontextprotocol.io/
	•	MCP specification: https://modelcontextprotocol.io/specification/2025-11-25

(Teaching note: MCP is the port. What you plug into it determines capability and risk.)

8.2 Prompt injection and tool risk (the practical version)

When a model can call tools, untrusted content can try to:
	•	Exfiltrate secrets
	•	Rewrite files or records
	•	Trigger actions that look reasonable

Controls:
	1.	Least-privilege tool permissions
	2.	Allowlists for actions
	3.	Separation of duties for high-impact actions
	4.	Human approval gates
	5.	Logging and monitoring

(Teaching note: A simple rule that works: the agent may draft, it may not send.)

8.3 Threat literacy you can actually use

Two baseline references:
	•	OWASP Top 10 for LLM Applications: https://owasp.org/www-project-top-10-for-large-language-model-applications/
	•	MITRE ATLAS: https://atlas.mitre.org/  ￼

OWASP LLM Top 10 project repository (useful for tracking updates): https://github.com/OWASP/www-project-top-10-for-large-language-model-applications  ￼

(Teaching note: Do not overcomplicate. One habit: list tools and data access, then design gates.)

⸻

9) Diffusion models: what to know (images and video)

Diffusion models generate images and video by iteratively refining noise into structure.

Practical uses:
	•	Marketing drafts
	•	Product mockups
	•	Storyboards
	•	Training visuals

Risk and control notes:
	•	Rights and provenance
	•	Brand safety and disallowed content
	•	Synthetic media disclosure where required
	•	Human review before external use

(Teaching note: Run a corporate-safe exercise: generate a storyboard, then add a disclosure footer and a usage rule.)

⸻

10) Vibe coding, safely

Vibe coding compresses time-to-prototype. It can also ship invisible risk.

Safe rules:
	1.	Keep secrets out of prompts and repos
	2.	Require tests, even basic smoke tests
	3.	Use dependency scanning and security linting
	4.	Use staged rollout and rollback
	5.	Human review remains mandatory for production

(Teaching note: Prototype fast, then add controls before real users touch it.)

⸻

11) Corporate use cases (cross-functional)

(Teaching note: Pick 2–3 based on audience. For each: define decision owner, data classification, and stop rules.)

Legal and compliance
	•	Contract drafting support with clause libraries and structured checklists
	•	Policy drafting and redlining with traceable assumptions
	•	Investigation support with strict confidentiality rules and logging

Finance and operations
	•	Variance explanations and narrative summaries
	•	Workflow automation for recurring reporting
	•	Internal controls support: draft narratives, evidence requests, test scripts

Sales, marketing, customer support
	•	Persona-based drafts with explicit brand rules
	•	Meeting capture → action items → CRM-ready summaries
	•	Customer response drafting with escalation triggers

Engineering and product
	•	Prototype internal tools quickly
	•	Spec writing, test generation, documentation
	•	Agent workflows touching tickets, repos, and deployments, with gates

⸻

12) Practical exercises (workshop-ready modules)

(Teaching note: Each module is 20–40 minutes. Pick 3–5 depending on time.)

Module 1: Prompt upgrade
	•	Take a real task prompt
	•	Convert it into the Magic Prompt structure
	•	Add verification: assumptions, unknowns, self-check
	•	Compare outputs

Module 2: Tool bake-off
	•	Same task across ChatGPT, Claude, Gemini, Perplexity
	•	Score correctness, usefulness, structure, and edit effort
	•	Choose a default tool by task type

Module 3: Build a “Tiny Servant” workflow spec
	•	Choose one recurring task
	•	Define input fields and output schema
	•	Add a gate and a logging requirement
	•	Store as a reusable internal template

Module 4: Voice agent tabletop
	•	Define a safe inbound scenario
	•	Write allowed actions
	•	Write escalation triggers
	•	Write post-call logging format

Module 5: MCP threat modeling mini-session
	•	Pick one agent workflow
	•	List tool access
	•	Identify top abuse cases
	•	Add mitigations and human gates

⸻

13) Operating checklist for instructors and teams

(Teaching note: Use this at the end. Converts learning into an operational plan.)
	1.	Pick 3 priority use cases
	2.	Name decision owners for each
	3.	Define allowed data and forbidden data
	4.	Define human gates
	5.	Define logging requirements
	6.	Define evaluation: what good means, how you test, what breaks the build
	7.	Pilot with a small group
	8.	Review incidents and near-misses
	9.	Expand with change management and training

⸻

14) Recommended Readings and Reference Map

Level 1: working literacy
	•	NIST AI RMF overview: https://www.nist.gov/itl/ai-risk-management-framework  ￼
	•	NIST AI RMF 1.0 (PDF): https://nvlpubs.nist.gov/nistpubs/ai/nist.ai.100-1.pdf  ￼
	•	MITRE ATLAS: https://atlas.mitre.org/  ￼
	•	OWASP LLM Top 10: https://owasp.org/www-project-top-10-for-large-language-model-applications/
	•	OWASP LLM Top 10 repo: https://github.com/OWASP/www-project-top-10-for-large-language-model-applications  ￼

Level 2: building and connecting tools
	•	MCP home: https://modelcontextprotocol.io/
	•	MCP specification: https://modelcontextprotocol.io/specification/2025-11-25
	•	OpenRouter: https://openrouter.ai/
	•	Apify docs: https://docs.apify.com/
	•	Vapi docs: https://docs.vapi.ai/

Level 3: management systems and governance
	•	ISO/IEC 42001 standard overview: https://www.iso.org/standard/42001  ￼
	•	ISO 42001 explained: https://www.iso.org/home/insights-news/resources/iso-42001-explained-what-it-is.html  ￼
	•	NIST GenAI profile (AI RMF profile for GenAI): https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf  ￼

Reading Map (by role)
	•	Executives and functional leaders
	1.	NIST AI RMF overview: https://www.nist.gov/itl/ai-risk-management-framework  ￼
	2.	ISO/IEC 42001 overview: https://www.iso.org/standard/42001  ￼
	3.	ISO 42001 explained: https://www.iso.org/home/insights-news/resources/iso-42001-explained-what-it-is.html  ￼
	•	Workflow owners and operators
	1.	OWASP LLM Top 10: https://owasp.org/www-project-top-10-for-large-language-model-applications/
	2.	MCP home: https://modelcontextprotocol.io/
	3.	NotebookLM: https://notebooklm.google/
	•	Security and IT
	1.	MITRE ATLAS: https://atlas.mitre.org/  ￼
	2.	OWASP LLM Top 10: https://owasp.org/www-project-top-10-for-large-language-model-applications/
	3.	MCP specification: https://modelcontextprotocol.io/specification/2025-11-25
	4.	Apify docs: https://docs.apify.com/
	•	Legal and compliance
	1.	ISO/IEC 42001 overview: https://www.iso.org/standard/42001  ￼
	2.	NIST AI RMF 1.0 (PDF): https://nvlpubs.nist.gov/nistpubs/ai/nist.ai.100-1.pdf  ￼
	3.	OWASP LLM Top 10: https://owasp.org/www-project-top-10-for-large-language-model-applications/
	•	Engineering and product
	1.	MCP home: https://modelcontextprotocol.io/
	2.	OpenRouter: https://openrouter.ai/
	3.	Ollama: https://ollama.com/
	4.	Replit: https://replit.com/
	5.	Bolt: https://bolt.new/

⸻

15) Builder Primer: websites and webapps, for novices (standalone)

15.1 Two build modes and the fastest way to choose
	1.	Website mode

	•	Goal: improve user flow and conversion
	•	Typical work: page redesign, copy, forms, performance, accessibility, instrumentation

	2.	Webapp mode

	•	Goal: deliver a workflow with state and business rules
	•	Typical work: frontend + backend + project data store (“Vault”) + APIs + auth + logs + deployment

Shared discipline:
	•	Define the metric
	•	Define the user
	•	Define the stop rules

15.2 The build pipeline (a repeatable loop that converges)
	1.	Rules and guidelines (one-page control surface)
	•	Objective metric and target
	•	Primary user and top failure points
	•	Scope: in, out, deferred
	•	Vault: what project data exists, who can access it, retention
	•	Non-negotiables: security, privacy, review gates
	2.	Discover
	•	Map the happy path and top 3 failure paths
	•	Identify dependencies and constraints
	3.	MVP
	•	One end-to-end path
	•	Basic error handling
	•	Measurement
	4.	Design
	•	Aesthetic direction plus usability checks
	5.	Spec
	•	Product requirements and technical spec, short is fine, missing is expensive
	6.	Build
	•	Implement
	•	Add logs
	•	Staging deploy
	•	Rollback plan
	7.	Measure
	•	Track the metric and failure points
	8.	Iterate
	•	One improvement at a time
	•	Logged and testable

15.3 Web fundamentals you must know (minimum)

Core mental model: client-server requests and responses, including HTTP status codes.
	•	MDN HTTP overview: https://developer.mozilla.org/en-US/docs/Web/HTTP
	•	MDN HTTP response status codes: https://developer.mozilla.org/en-US/docs/Web/HTTP/Status

15.4 The Vault (project data store), clarified

“Vault” = data relevant to the project, treated as a first-class component.

Minimum Vault decisions:
	1.	What data exists (entities and fields)
	2.	Who can read, write, delete (authorization rules)
	3.	Retention and deletion
	4.	Audit trail: what events must be logged

Practical implication:
	•	Many fast prototypes fail in production because Vault rules are implicit, not enforced.

15.5 Nonfunctional basics (the novice gap)

A) Security baseline
Use OWASP as a default awareness checklist, then tighten per your environment:
	•	OWASP home: https://owasp.org/
	•	OWASP ASVS (application security verification standard): https://owasp.org/www-project-application-security-verification-standard/

B) Accessibility baseline
	•	WCAG 2.2 Quick Reference: https://www.w3.org/WAI/WCAG22/quickref/

C) Performance baseline
Use Core Web Vitals (LCP, INP, CLS) plus measurement tooling:
	•	Core Web Vitals overview: https://web.dev/vitals/

D) Quality checks, fast
	•	Lighthouse: https://developer.chrome.com/docs/lighthouse/overview/

E) Logging mindset
Treat logs as event streams:
	•	12-factor logs: https://12factor.net/logs

15.6 Website mode playbook (conversion)
	1.	Baseline measure (conversion, bounce, load time)
	2.	Redesign one page or one funnel step
	3.	Run Lighthouse
	4.	Run a WCAG quick pass
	5.	Ship to staging, then deploy
	6.	Measure, then iterate

15.7 Webapp mode playbook (frontend + backend + Vault)
	1.	Sketch client-server flow (requests, responses)
	2.	Define Vault data model and access rules
	3.	Define APIs and error behavior
	4.	Implement happy path, then top 3 failure paths
	5.	Add logs, staging deploy, rollback
	6.	Measure task success, errors, latency

15.8 Prompting and build work: one practical rule

Prompts can draft and scaffold. The system must still pass gates:
	•	Security baseline (OWASP, plus your internal policies)
	•	Accessibility baseline (WCAG)
	•	Performance baseline (Core Web Vitals, Lighthouse)
	•	Logging and rollback

Prompt structure references:
	•	OpenAI prompt engineering guide: https://platform.openai.com/docs/guides/prompt-engineering
	•	OpenAI evals guide: https://platform.openai.com/docs/guides/evals

⸻

Closing: the AI Generalist’s rule set
	1.	Start with the decisions.
	2.	Use AI to accelerate drafts, not to replace accountability.
	3.	Constrain scope, control data, and log the work.
	4.	Build small, ship safely, iterate.
	5.	Final Liability rests with the Human.

Final Liability rests with the Human.
