# the-ai-generalist
A one day corporate workshop.

# The AI Generalist

Recommended inspiration program: https://www.outskill.com/2-day-ai-mastermind

## Learning Objectives
By the end of this workshop, participants will be able to:
1. Frame AI work as a decision-improving workflow, not a tool experiment
2. Produce a Context Packet that captures objective, constraints, risk tier, gates, logs, and escalation
3. Write and version a Prompt Spec that includes success criteria, exclusions, and verification steps
4. Convert a prompt into a governed workflow spec with ownership, review gates, logging, and measurable outputs
5. Apply Slow AI and Final Liability in practice: visible work, explainable steps, auditable evidence packs, named accountable owner
6. Use a controlled experimentation protocol with tiers, stop rules, and evidence packs to try tools safely
7. Identify where agents, voice agents, automation, scraping, local models, and MCP fit, and when they do not

(Teaching note: Read the Learning Objectives out loud at the start. Repeat them right before labs. End the day by mapping each team’s outputs back to these objectives.)

---

## TL;DR
- Become an AI Generalist to surf the tsunami: adapt quickly while holding control
- Your advantage is high context from experience. Encode it into Context Packets, then let AI compress execution
- Learn by building, but in corporate settings experimentation must be governed: scope, gates, logs, escalation
- Operating posture: Slow AI plus Final Liability rests with the Human
- Outputs are reusable: prompt library, governed workflow spec, risk tiering, evidence pack, policy starter

---

## 0) Facilitator guide

### 0.1 Audience and prerequisites
- Best audience
  1. Operators and managers who own workflows
  2. One IT and security liaison, or a stand-in
  3. One legal and compliance liaison, or a stand-in
- Participant prerequisites
  1. Bring one real workflow they own or influence
  2. Access to at least one approved AI assistant
  3. Agreement to follow data handling rules

(Teaching note: If participants do not own a workflow, assign them to a table with a workflow owner. Ownership is the difference between training and shipping.)

### 0.2 Room setup and materials
- Setup
  1. Tables of 4–6
  2. Shared screen for demos
  3. Timer visible to the room
- Materials
  1. One shared doc per table for artifacts
  2. Printed stop rules and risk tiers
  3. Templates compiled into a single workbook doc

(Teaching note: Do not require new account creation live. If a tool is not already approved, treat it as conceptual only.)

### 0.3 Facilitator checklist
Before:
1. Confirm what data can be used in the room
2. Confirm what tools are allowed for the room
3. Prepare today’s default stack, minimum viable set
4. Prepare a workbook with templates
5. Choose one safe demo workflow

During:
1. Keep the day artifact-driven
2. Enforce stop rules
3. Make every table name an owner
4. Timebox tool exploration
5. Collect outputs in one folder

After:
1. Export artifacts into a shared repository
2. Assign owners and a review cadence
3. Run a 2–4 week pilot on Tier 0–1 workflows
4. Schedule a CAPA review for anything that breaks

(Teaching note: Your job is not to impress people with tools. Your job is to create reusable workflow assets with controls.)

### 0.4 Definition of Done for the day
Each team must submit:
1. Context Packet for one workflow
2. Prompt Spec v1, versioned
3. Governed Workflow Spec v1 with gates and logs
4. Risk tier and control mapping
5. Evidence pack checklist completed

(Teaching note: Write the DoD on a board. When discussion drifts, ask which DoD item this improves.)

### 0.5 Suggested one-day agenda
- 09:00–09:20 Opening: tsunami frame, Learning Objectives, rules
- 09:20–10:00 Operating posture: Slow AI, Final Liability, AI GRC
- 10:00–10:40 Foundations: LLMs, diffusion basics, failure modes
- 10:40–12:00 Lab 1: Context Packet
- 13:00–14:10 Lab 2: Prompt Spec
- 14:10–15:20 Lab 3: Governed Workflow Spec
- 15:20–16:10 Agents and advanced patterns, bounded
- 16:10–17:00 AI GRC mapping, scoring, commitments, close

(Teaching note: Protect the labs. If you run short, cut demos, not hands-on artifact time.)

---

## 1) Why this workshop exists

### 1.1 Surf the tsunami
- Capability is rising quickly.
- The winning posture is not loyalty to one vendor.
- The winning posture is:
  1. Learning velocity
  2. Workflow design
  3. Governance discipline

(Teaching note: Use one example from the business. AI can draft faster, but without verification it produces confident errors faster.)

### 1.2 What an AI Generalist is
- Definition
  1. A full-stack problem solver who selects tools, designs workflows, and ships outcomes with controls.
- Core competencies
  1. Task framing
  2. Prompting
  3. Workflow design
  4. Selective autonomy
  5. Verification discipline
  6. Governance discipline

(Teaching note: Full-stack does not mean engineer. It means end-to-end accountability for workflow outcomes.)

### 1.3 Your advantage: high context from experience
- Experience provides:
  1. Constraints
  2. Edge cases
  3. Acceptability tests
  4. Risk intuition
- AI amplifies what you provide:
  1. Strong context produces strong output
  2. Weak context produces plausible nonsense

(Teaching note: Tell participants: AI is a multiplier. Your job is to feed it reality, not vibes.)

---

## 2) The operating posture: Slow AI, Final Liability, AI GRC

### 2.1 Slow AI
- Slow AI does not mean slow work. It means governed work.
- Requirements
  1. Visible: inputs, steps, tools, versions, outputs are logged
  2. Explainable: decision-relevant reasoning can be reviewed
  3. Auditable: artifacts are versioned with change control and evidence packs

(Teaching note: Auditability means another team can reproduce the workflow, review assumptions, and see who approved what.)

### 2.2 Final Liability rests with the Human
- Rule
  1. Every meaningful workflow has a named accountable owner with decision rights.
- Enforcement
  1. No owner, no deployment
  2. No log, no trust
  3. No gate, no external release

(Teaching note: Ask this in every lab: Who is the owner. Make them write a name, not a role.)

### 2.3 AI GRC in one page
- Governance
  1. Approved use cases list with owners and review cadence
  2. Model and tool approval process
- Risk management
  1. Risk tiers mapped to controls
  2. Verification requirements by tier
- Compliance
  1. Data classification and retention
  2. Third-party risk review
  3. Incident response and CAPA

(Teaching note: AI GRC is operational plumbing. Gates, logs, owners, escalation. Not a binder.)

⧉ Biggest risk and gap: tool adoption outruns ownership, review gates, and logging.

---

## 3) Minimum technical literacy

### 3.1 The AI stack
1. Artificial intelligence  
2. Machine learning  
3. Deep learning  
4. Large language models  

(Teaching note: The goal is not technical mastery. The goal is to prevent category errors like the chatbot is intelligent therefore it is right.)

### 3.2 How an LLM works
1. Tokenization  
2. Embeddings  
3. Transformer attention  
4. Next-token prediction  
5. Iterative generation  

(Teaching note: This explains fluent error. The model predicts plausible text. It does not guarantee truth.)

### 3.3 Diffusion models for images and video
- Simplified explanation
  1. Start with noise
  2. Iteratively denoise guided by prompt and conditioning
- Why it matters
  1. Outputs vary even with similar prompts
  2. Style bias exists
  3. Rights and provenance matter

(Teaching note: For corporate use, insist on human review for customer-facing assets, plus a rights and brand check.)

### 3.4 Corporate failure modes
1. Hallucination and false confidence  
2. Prompt sensitivity and missing context  
3. Confidential data leakage  
4. Drift across model updates and time  
5. Automation overreach with agents  

(Teaching note: Run a 5-minute exercise. Each table picks one failure mode, invents a plausible incident in their function, then proposes one control.)

---

## 4) Prompting that holds up at work

### 4.1 The prompt formula
1. Role and context  
2. Task and success criteria  
3. Instructions and constraints  
4. Data boundaries, exclusions, output format  

(Teaching note: Make success criteria non-negotiable. If they cannot state it, they do not understand the task yet.)

### 4.2 Reliable techniques and when to use them
- Prompt chaining, default pattern
  1. Draft, critique, revise, verify, format
- Meta prompting
  1. Ask AI to propose the best prompt structure and workflow steps, then the human locks it
- Multi-approach exploration
  1. Generate multiple approaches, score, select, refine
- Self-refine against a rubric
  1. Critique output against acceptance tests, then revise

(Teaching note: For junior facilitators, demonstrate prompt chaining only. Mention the others as options, not requirements.)

### 4.3 Parameter knobs, practical controls
1. Temperature: creativity vs determinism  
2. Max tokens: length control  
3. Top-p: diversity control  
4. Frequency and presence penalties: repetition vs novelty  

(Teaching note: If your audience is non-technical, demonstrate temperature and max tokens only. Keep it measurable.)

### 4.4 Prompt governance
- Prompts become controlled assets if reused
  1. Name, owner, purpose
  2. Version and change log
  3. Known failure modes
  4. Acceptance tests

(Teaching note: Rule of thumb. If a prompt is used more than twice, it becomes a named asset with an owner.)

---

## 5) From prompts to systems: mix and remix

### 5.1 The pattern: prompt → workflow → agent → interface
1. Write a Prompt Spec in a prompt container like Custom GPTs or Gemini Gems
2. Move it to an orchestration layer for repeatable steps
3. Add an agent layer for multi-step execution where appropriate
4. Provide a UI with review gates and logging

(Teaching note: Teach the pattern, not the brand. Most corporations will swap tools. The architecture stays.)

### 5.2 Mix and remix, as a learning method
- Example learning pathway
  1. Start with a prompt container and create a high-quality Prompt Spec
  2. Move the Prompt Spec into an orchestration backend
  3. Add an agent execution slot for consistent step-running and tool calls
  4. Build a controlled front-end that enforces inputs, approvals, and logging
- Why this works
  1. It forces you to make assumptions explicit
  2. It forces you to define gates and logs
  3. It turns playing with AI into a repeatable workflow

(Teaching note: The learning goal is not a perfect toolchain. The learning goal is a repeatable, governed workflow.)

### 5.3 Voice agents with Vapi
- Good corporate use cases
  1. Intake and triage
  2. Scheduling
  3. Routing and FAQ
- Required controls
  1. Consent language
  2. Refusal and handoff rules
  3. Logging and retention
  4. No claims, no legal advice, no money movement without explicit confirmation and escalation

(Teaching note: Keep voice agents as a design exercise unless IT and legal approve a sandbox environment.)

---

## 6) Model landscape and selection, durable framing
- Stable view
  1. Several major model families exist and compete across reasoning, coding, multimodal, and long-context.
  2. Specific version names and benchmark claims change frequently.
- Selection criteria to teach
  1. Task fit: reasoning, coding, drafting, multimodal, long-context
  2. Data constraints: what can be sent, stored, retained
  3. Reliability: verification support, tool integration, logging options
  4. Cost and latency: economics and throughput
  5. Deployment: SaaS, private, local
  6. Governance: admin controls, audit logs, policy enforcement

(Teaching note: If someone asks which model is best, redirect to criteria. Corporate safety comes from fit and controls, not fandom.)

---

## 7) Controlled experimentation protocol

### 7.1 Risk tiers
- Tier 0: public, low stakes  
- Tier 1: internal, non-sensitive operational support  
- Tier 2: sensitive internal or customer-facing  
- Tier 3: high-risk decisions, regulated activity, legal claims, money movement  

(Teaching note: Have each team label their workflow. If they argue, default upward.)

### 7.2 Stop rules, hard gates
Stop and escalate if any are true:
1. Touches money movement, approvals, or authorization  
2. Creates legal, compliance, safety, or medical claims  
3. Uses personal data beyond policy  
4. Publishes externally or communicates externally  
5. Executes actions without explicit human confirmation  

(Teaching note: Read these aloud. Then ask each table to name one edge case that triggers a stop rule in their workflow.)

### 7.3 Evidence pack, minimum for trust
1. Owner and scope  
2. Prompt and workflow versions  
3. Data classification used  
4. Output samples  
5. Verification notes  
6. Log excerpt  
7. Incident notes, if any  

(Teaching note: Evidence packs are the bridge between innovation and audit. Without them, pilots cannot scale.)

---

## 8) Advanced modules, optional and gated

### 8.1 OpenRouter, model routing
- What it is
  1. A routing layer that can provide access to multiple models behind one interface.
- Corporate value
  1. Standardize access and selection rules
  2. Improve portability across model changes
- Controls
  1. Log model selection
  2. Restrict models by tier
  3. Keep data boundaries explicit

(Teaching note: Treat routing as governance. It reduces random tool and model sprawl.)

### 8.2 Bolt setups and quick prototyping
- What it is
  1. A fast way to prototype apps and workflows from prompts.
- How to teach it
  1. Use it to build a front-end form around a Prompt Spec
  2. Enforce input validation and required fields
  3. Add a human review gate before any external output
- Controls
  1. Do not connect to sensitive systems without IT approval
  2. Keep logs of inputs and outputs
  3. Version the prompt and workflow

(Teaching note: Bolt is a speed tool. Your job is to slow it down at the gates: permissions, review, logging.)

### 8.3 Ollama, local hosting
- What it is
  1. A way to run some models locally.
- When it helps
  1. Privacy constraints
  2. Offline operation
  3. Cost control for certain tasks
- What it does not solve
  1. Quality parity with top hosted models is not guaranteed
  2. Governance still required: logs, gates, owners

(Teaching note: Local does not automatically mean safe. Safety comes from permissions, logging, and scope.)

### 8.4 Plug local models into your builds
- Pattern
  1. Treat the local model as a service endpoint
  2. Connect it to your workflow tooling for Tier 0–1 use cases
  3. Keep the same gates and logs you would use for SaaS models
- Why it matters
  1. Helps teams learn model ops basics
  2. Makes cost and privacy tradeoffs real

(Teaching note: The point is literacy. Most teams will still use hosted models for critical work.)

### 8.5 MCP, Model Context Protocol
- What it is
  1. An open standard for connecting AI applications to tools and data sources.
- Why it matters
  1. Reduces brittle prompt stuffing
  2. Makes tool access explicit and more auditable
- Controls to enforce
  1. Tool permissioning
  2. Input and output logging
  3. Prompt injection and data poisoning assumptions
  4. Treat every tool connection as privileged access. Default deny.

(Teaching note: Teach MCP as standardized ports for tools and data. Then teach the security truth: tool access expands attack surface.)

### 8.6 Goose, computer automation
- What it is
  1. An on-machine agent that can automate developer tasks.
- Corporate guardrails
  1. Tier 0–1 only at first
  2. Human confirmation before irreversible actions
  3. Short sessions and strong logs

(Teaching note: Frame this as power tools. Helpful, injury-prone without guards.)

### 8.7 Apify, scraping and automation
- Guardrails
  1. Confirm platform terms and internal policy before use
  2. Minimize personal data
  3. Define purpose, retention, access controls
  4. Maintain a collection log

(Teaching note: If legal and compliance are not present, keep this as theory only. Do not run hands-on scraping in a corporate room.)

### 8.8 Fiddle with diffusion models
- Goal
  1. Learn prompt control, reference images, seeds, and post-processing
- Output
  1. A small brand-safe asset pack for internal training, not external marketing
- Controls
  1. Rights and provenance tracking
  2. Disclosure rules for synthetic media
  3. Human review before reuse

(Teaching note: Keep this framed as literacy. Do not let it turn into an art contest.)

### 8.9 Kimi, agent swarms
- Use for
  1. Parallel research, critique, verification, synthesis
- Controls
  1. One accountable owner
  2. No autonomous external actions
  3. Human sign-off

(Teaching note: Multi-agent can multiply errors. Require a single-voice review and signed decision.)

### 8.10 Take the leap, try vibe coding
- What it is
  1. Rapid AI-assisted building where the user guides by intent and review.
- Minimum production controls
  1. Access control
  2. Logging
  3. Basic tests
  4. Rollback plan
  5. Review gate

(Teaching note: Define prototype vs production. The control set is the line.)

---

## 9) Labs, step-by-step runbook

### Lab 1: Context Packet, 70 minutes
- Steps
  1. Choose one workflow, 10 min
  2. Fill Context Packet, 25 min
  3. Identify tier, stop rules, required gate, 15 min
  4. Peer review with another table, 20 min
- Output
  1. Completed Context Packet v1

(Teaching note: Script: If success criteria and exclusions are unclear, stop and tighten. Do not prompt yet.)

### Lab 2: Prompt Spec, 70 minutes
- Steps
  1. Write role, context, task, success criteria, 10 min
  2. Add constraints, exclusions, output format, 20 min
  3. Add verification step and acceptance tests, 20 min
  4. Run one prompt chain, capture outputs and failures, 20 min
- Output
  1. Prompt Spec v1 with acceptance tests

(Teaching note: Require one verification step. Example: List factual claims and flag unknowns.)

### Lab 3: Governed Workflow Spec, 70 minutes
- Steps
  1. Define steps and tool slots, vendor-neutral, 15 min
  2. Define gates and approvals, 20 min
  3. Define logs and storage, 15 min
  4. Define metrics and rollout plan, 20 min
- Output
  1. Governed Workflow Spec v1

(Teaching note: Push gate design. The gate is where Final Liability becomes real.)

### Lab 4: AI GRC mapping, 50 minutes
- Steps
  1. Map tier → controls, 15 min
  2. Define evidence pack fields, 15 min
  3. Define escalation path and CAPA trigger, 20 min
- Output
  1. Risk and control mapping plus evidence pack checklist

(Teaching note: Escalation path must name a real person or real group, not management.)

---

## 10) Templates

### 10.1 Context Packet
- Objective
- Decision owner
- Users and stakeholders
- Inputs and data sources
- Constraints
- Success criteria
- Exclusions
- Edge cases
- Failure modes
- Risk tier
- Required gate
- Logging plan
- Escalation path

(Teaching note: Exclusions prevent accidental expansion. They are a safety feature.)

### 10.2 Prompt Spec
- Name, owner, purpose
- Prompt text
- Required inputs
- Exclusions
- Output format
- Verification step
- Acceptance tests
- Known failure modes
- Version and change log

(Teaching note: Acceptance tests can be simple. Example: Must list assumptions and must output a checklist.)

### 10.3 Governed Workflow Spec
- Name, owner, scope, exclusions
- Steps and tool slots
- Models used and routing rules, if relevant
- Data handling and retention
- Gates and approvals
- Logging and storage
- Metrics: time saved, error rate, adoption
- Rollout plan: pilot → expand → standardize

(Teaching note: Rollout plan forces realism. Many teams design workflows that never ship.)

### 10.4 Incident and CAPA
- What happened
- Impact
- Root cause
- Containment
- Corrective action
- Preventive action
- Owner and due date
- Evidence retained

(Teaching note: CAPA is learning at scale. It is how you avoid repeating the same failure with a new tool name.)

---

## 11) Tool links

### Core assistants and search
- ChatGPT: https://chatgpt.com/
- Claude: https://claude.ai/
- Gemini: https://gemini.google.com/
- Perplexity: https://www.perplexity.ai/
- NotebookLM: https://notebooklm.google/

### Meetings and notes
- Fireflies: https://fireflies.ai/
- Granola: https://granola.so/

### Dictation, voice, avatars
- Wispr Flow: https://wisprflow.ai/
- Vapi: https://vapi.ai/
- ElevenLabs: https://elevenlabs.io/
- HeyGen: https://www.heygen.com/
- Suno: https://suno.com/

### Images and video
- Phot AI: https://www.phot.ai/
- Runway: https://runwayml.com/
- Midjourney: https://www.midjourney.com/
- Krea: https://krea.ai/
- Leonardo: https://leonardo.ai/
- Magnific: https://magnific.ai/
- Kling: https://klingai.com/
- Higgsfield: https://higgsfield.ai/

### Builders, dev tools, routing, local models, protocols
- Replit: https://replit.com/
- Bolt: https://bolt.new/
- Lovable: https://lovable.dev/
- OpenRouter: https://openrouter.ai/
- Ollama: https://ollama.com/
- MCP: https://modelcontextprotocol.io/

### Automation and scraping
- Goose: https://block.github.io/goose/
- Apify: https://apify.com/

### Multi-agent
- Kimi: https://www.kimi.com/en

### Marketing, writing, growth
- Writesonic: https://writesonic.com/
- Supergrow: https://www.supergrow.ai/
- SocialSonic: https://socialsonic.com/
- Genspark: https://www.genspark.ai/
- Numerous AI: https://numerous.ai/

### People and network intelligence
- Crystal: https://www.crystalknows.com/
- Happenstance: https://happenstance.ai/

### Other referenced tools
- Chronicle: https://chroniclehq.com/
- Emily: https://meetemily.ai/
- Lyzr AI: https://lyzr.ai/
- Humanic AI: https://humanic.ai/
- Emergent: https://emergent.sh/
- Rocket: https://www.rocket.new/

---

## 12) Recommended Readings

### 12.1 Reading map by role
Use this to assign pre-reads and to guide deeper study after the workshop.

- Executives and functional leaders
  1. NIST AI RMF overview: https://www.nist.gov/itl/ai-risk-management-framework
  2. NIST Generative AI Profile (PDF): https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf
  3. ISO/IEC 42001 standard page: https://www.iso.org/standard/42001
  4. EU AI Act final text: https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng

  (Teaching note: Leaders should learn the control vocabulary: ownership, tiering, gates, logs, monitoring, incident response.)

- Workflow owners and operators
  1. OpenAI prompt engineering guide: https://developers.openai.com/api/docs/guides/prompt-engineering/
  2. Claude prompt engineering overview: https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/overview
  3. Gemini prompting strategies: https://ai.google.dev/gemini-api/docs/prompting-strategies
  4. AI Incident Database: https://incidentdatabase.ai/
  5. OpenAI evals guide: https://developers.openai.com/api/docs/guides/evals

  (Teaching note: Operators should learn two habits: write acceptance tests and run evals before and after model changes.)

- Security and IT
  1. OWASP Top 10 for LLM Applications: https://owasp.org/www-project-top-10-for-large-language-model-applications/
  2. MITRE ATLAS: https://atlas.mitre.org/
  3. Secure AI Framework (SAIF) overview: https://safety.google/safety/saif/
  4. MCP specification: https://modelcontextprotocol.io/specification/2025-11-25
  5. OpenAI safety best practices: https://developers.openai.com/api/docs/guides/safety-best-practices

  (Teaching note: Emphasize that tool connections are privileged access. Default deny, then grant least privilege with logs.)

- Legal and compliance
  1. ISO/IEC 42001 standard page: https://www.iso.org/standard/42001
  2. ISO/IEC 23894 standard page: https://www.iso.org/standard/77304.html
  3. GDPR legal text: https://eur-lex.europa.eu/eli/reg/2016/679/oj/eng
  4. EU AI Act final text: https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng
  5. NIST Privacy Framework (PDF): https://nvlpubs.nist.gov/nistpubs/CSWP/NIST.CSWP.01162020.pdf

  (Teaching note: Focus on the operational controls that make compliance real: classification, retention, vendor review, audit logs, approvals, CAPA.)

- Engineering, data, and product
  1. OpenAI GPT-5.2 Prompting Guide: https://developers.openai.com/cookbook/examples/gpt-5/gpt-5-2_prompting_guide/
  2. OpenAI Evals (GitHub): https://github.com/openai/evals
  3. Stanford HELM benchmark: https://crfm.stanford.edu/helm/
  4. LangChain RAG tutorial: https://docs.langchain.com/oss/python/langchain/rag
  5. LangGraph agentic RAG tutorial: https://docs.langchain.com/oss/python/langgraph/agentic-rag

  (Teaching note: Engineers should treat prompts like code. Version them. Test them. Monitor them. Plan for rollback.)

### 12.2 Foundations: how the core models work
- Transformers: Attention Is All You Need (paper): https://arxiv.org/abs/1706.03762
- Transformers (PDF): https://arxiv.org/pdf/1706.03762
- Diffusion models: Denoising Diffusion Probabilistic Models (paper): https://arxiv.org/abs/2006.11239
- Diffusion models (PDF): https://arxiv.org/pdf/2006.11239

(Teaching note: Use these to anchor why outputs are probabilistic, fluent, and sometimes wrong.)

### 12.3 Prompting and workflow design
- OpenAI prompt engineering guide: https://developers.openai.com/api/docs/guides/prompt-engineering/
- OpenAI GPT-5.2 Prompting Guide: https://developers.openai.com/cookbook/examples/gpt-5/gpt-5-2_prompting_guide/
- Claude prompt engineering overview: https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/overview
- Anthropic: Effective context engineering for AI agents: https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents
- Gemini prompting strategies: https://ai.google.dev/gemini-api/docs/prompting-strategies
- Gemini for Workspace prompting guide (PDF): https://services.google.com/fh/files/misc/gemini-for-google-workspace-prompting-guide-101.pdf

(Teaching note: Use these to justify prompt assets, success criteria, constraints, critique loops, and structured outputs.)

### 12.4 AI governance, risk, and controls
- NIST AI RMF 1.0 (PDF): https://nvlpubs.nist.gov/nistpubs/ai/nist.ai.100-1.pdf
- NIST Generative AI Profile (PDF): https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf
- ISO/IEC 42001 standard page: https://www.iso.org/standard/42001
- ISO/IEC 23894 standard page: https://www.iso.org/standard/77304.html

(Teaching note: Tie Slow AI to documentation, ownership, risk tiering, verification discipline, monitoring, and change control.)

### 12.5 Security for LLM and agent workflows
- OWASP Top 10 for LLM Applications: https://owasp.org/www-project-top-10-for-large-language-model-applications/
- MITRE ATLAS: https://atlas.mitre.org/
- OpenAI safety best practices: https://developers.openai.com/api/docs/guides/safety-best-practices

(Teaching note: Use these to justify default deny for tool connections, adversarial testing, prompt injection assumptions, and human approval gates.)

### 12.6 Enterprise security anchors
- ISO/IEC 27001 standard page: https://www.iso.org/standard/27001
- Secure AI Framework (SAIF) overview: https://safety.google/safety/saif/

(Teaching note: These are your security posture anchors when someone tries to treat agents as harmless chatbots.)

### 12.7 Evaluation, monitoring, and upgrade safety
- OpenAI evals guide: https://developers.openai.com/api/docs/guides/evals
- OpenAI Evals (GitHub): https://github.com/openai/evals
- OpenAI cookbook: Getting started with evals: https://developers.openai.com/cookbook/examples/evaluation/getting_started_with_openai_evals/
- Stanford HELM benchmark: https://crfm.stanford.edu/helm/
- MLflow GenAI eval and monitoring: https://mlflow.org/docs/latest/genai/eval-monitor/

(Teaching note: This is the operational spine. You need evals to upgrade models safely, detect regressions, and justify trust with evidence packs.)

### 12.8 RAG and grounding
- LangChain RAG tutorial: https://docs.langchain.com/oss/python/langchain/rag
- LangGraph agentic RAG tutorial: https://docs.langchain.com/oss/python/langgraph/agentic-rag

(Teaching note: Teach RAG as do not ask the model to remember what you can retrieve. Then connect it to governance: source logging.)

### 12.9 Privacy and compliance anchor points
- GDPR legal text: https://eur-lex.europa.eu/eli/reg/2016/679/oj/eng
- NIST Privacy Framework (PDF): https://nvlpubs.nist.gov/nistpubs/CSWP/NIST.CSWP.01162020.pdf

(Teaching note: Keep this scoped to data minimization, retention, access controls, and documentation unless the client requests jurisdiction depth.)

### 12.10 Regulation reference point
- EU AI Act final text: https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng

(Teaching note: Use this to explain why risk tiering, documentation, and post-deployment monitoring are becoming non-optional.)

### 12.11 Learning from real failures
- AI Incident Database: https://incidentdatabase.ai/

(Teaching note: Pick one incident relevant to the audience’s sector. Run a short which gate would have stopped this drill.)

---
**Final Liability rests with the Human.**
