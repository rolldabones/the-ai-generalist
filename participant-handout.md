# The AI Generalist: Participant Handout

Son-U Michael Paik · CEO, GRC Solutions Korea

**v2.0.0 · 18 October 2026 (KST)**

The participant text of the one-day workshop, sections 0 to 11 and 14. Section numbers are kept from v1.1.4: sections 12 (practical exercises) and 13 (operating checklist) are in the facilitator guide and section 15 is [builder-primer.md](builder-primer.md). The learning objectives, the regulatory and standards currency note and the citation are in [README.md](README.md); the tool map is [tool-map.md](tool-map.md); the facilitator's agenda, teaching notes, exercises and operating checklist are in [facilitator-guide.md](facilitator-guide.md). The eight controls are stated once, in section 2.4.

## 0) Workshop contract: how we work today

### 0.1 Mode
- This is not a “one tool” class.
- We are building a durable method that survives tool churn.

### 0.2 Outcome
Participants leave with:
- A reusable prompting workflow
- A tool selection map
- A minimum governance control set
- One small, working workflow spec they can reuse at work

### 0.3 Definition of Done
This handout should be usable as:
- Participant primer

---

## 1) Workshop posture

### 1.1 Become an AI Generalist to surf the tsunami
AI is now a general capability layer across functions. “Generalist” does not mean shallow. It means you can:
- Understand the core mechanism
- Choose tools rationally
- Build small workflows fast
- Control risk with discipline
- Keep humans accountable

### 1.2 Your leverage is experience and context
Models can draft, summarize, transform, plan and assist with code. You supply:
- Objectives and constraints
- Edge cases and acceptable risk
- Reality checks and tradeoffs
- The decision and the owner

### 1.3 Learn by building, but govern the build
Practical loop:
1. Try a tool on a synthetic task
2. Compare outputs across 2–3 tools
3. Add constraints and checks
4. Log what worked as a reusable pattern

---

## 2) Slow AI, Informed Intent, Final Liability and AI governance, risk management and compliance (AI GRC)

### 2.1 Slow AI (precondition)
Slow AI: AI that cannot be governed, explained and audited is not deployed; the three tests are conjunctive, and the doctrine is a precondition, not a speed limit. In workshop terms, a workflow is:
- Governed: a named owner, defined boundaries and a working intervention path, so it is visible, monitored and pausable
- Explained: the team can state why an output was produced, in terms the person affected can use, enough for the decision at hand
- Audited: the evidence exists before it is asked for

Translate posture into controls: the eight controls of section 2.4, stated there once. Versioning of prompt, model and tools and the stop rules sit inside logging (control 4) and human gates (control 3); evaluation is control 5 and change control is control 8.

### 2.2 Informed Intent (authorization gate)
Informed Intent: no AI system acts without prior authorization stating its purpose, authority, boundaries and exit, given by a human who meets the five authorizer conditions. In workshop terms, the authorization specifies:
- Purpose: what the workflow is for
- Authority: on whose authority it acts, given by a named human with the knowledge, evidence, authority, time and permission to give it
- Boundaries: what it may and may not touch, with its data boundaries, action boundaries and tolerance thresholds
- Exit: how the workflow is paused, rolled back and retired

### 2.3 Final Liability rests with the Human (accountability rule)
Final Liability rests with the Human: every material outcome attaches to a named human owner with decision rights, oversight and the power to intervene. In workshop terms, the owner:
- Holds the decision rights over the output
- Holds oversight of the workflow and its limits
- Has the power to intervene, including stopping the workflow

### 2.4 AI GRC minimum control set
Treat AI as a capability that changes decision quality, record creation, process velocity and risk pathways.

Minimum control set (workable in most organizations):
1. Use-case registry: what AI is doing, where, for whom, by which owner, with the scope of each use
2. Data rules: what data may be used, where it may go, retention rules
3. Human gates: which outputs require review and approval, with the escalation triggers
4. Logging: inputs, outputs, versions, approvals, exceptions
5. Evaluation: accuracy, hallucination rate, regressions after updates
6. Security: prompt injection defenses, tool permissions, secrets handling
7. Vendor and supply chain: models, plugins, connectors, agent tools
8. Change management: updates, drift monitoring, rollback plan, CAPA (corrective and preventive action)

Reference anchors:
- NIST AI Risk Management Framework overview: https://www.nist.gov/itl/ai-risk-management-framework
- NIST AI RMF 1.0 (PDF): https://nvlpubs.nist.gov/nistpubs/ai/nist.ai.100-1.pdf

Biggest recurring gap: adoption outruns ownership, allowed data, stop rules and logging.

---

## 3) Foundations: what an LLM is and why failure modes are predictable

### 3.1 The “AI stack” nesting map (operational, not academic)
1. Artificial intelligence: machines doing tasks associated with human intelligence
2. Machine learning: systems learning patterns from data to make predictions
3. Deep learning: neural networks at scale
4. Large language models: deep learning models trained on large text corpora to predict and generate language

### 3.2 How an LLM works (simple pipeline)
1. Tokenization: text is broken into tokens
2. Embeddings: tokens map to vectors capturing relationships in meaning
3. Transformer attention: model weights which prior tokens matter most
4. Next-token prediction: model predicts the next token repeatedly
5. Response generation: predictions become text, code or structured outputs

Anchor sentence:
- An LLM predicts plausible next tokens, not truth.

### 3.3 Practical implications you can use immediately
- Strong at drafting, summarizing, transforming, patterning and code assistance
- Weak at guaranteed factuality without retrieval and verification
- Output quality depends heavily on constraints, context and evaluation

**Context window.** A model reads a bounded amount of text at once, its context window. Everything it is to use must be inside it: the prompt, the documents supplied, the conversation so far and its own output. What falls outside is not known to the model, however recently it was said. Long inputs are not read with uniform care; put the controlling facts and the output specification where they cannot be lost and state them once, precisely.

**Retrieval-augmented generation and agents.** Retrieval-augmented generation (RAG) fetches passages from a chosen corpus at the moment of the request and places them in the context window, so the model answers from supplied evidence rather than from memory; the answer is then bounded by the quality of the retrieval, which must be tested like any other component. An agent is a model given tools and a loop: it reads, decides, calls a tool, reads the result and continues until a stop condition. Every tool is an action surface and every retrieved passage is untrusted input; section 8 carries the controls.

**Thinking models.** Some models spend additional computation before answering and produce intermediate reasoning that the product may or may not show. Visible reasoning helps review and guarantees nothing: the answer is still verified against sources, and cost and latency rise with the reasoning budget. Set the budget to the decision at hand and keep the human gate where the cost of being wrong is high.

---

## 4) Prompting as a professional skill

### 4.1 The Magic Prompt structure
A durable pattern:
1. Role: who the assistant is acting as
2. Objective: what success looks like
3. Context: facts, constraints, audience, inputs
4. Instructions: steps, boundaries, checks
5. Output spec: format, headings, length, style rules
6. Verification: assumptions, unknowns, how it checked

### 4.2 The 4-pass workflow
1. FRAME: objective, decision owner, constraints, risk tier, stop rules
2. DRAFT: generate a first pass fast
3. TIGHTEN: add checks, edge cases, counterarguments, formatting, tests
4. LOCK: finalize, record assumptions, store as a reusable template

### 4.3 Common failure modes and fixes
- Vague objective → add acceptance tests and examples
- Missing constraints → add must and must-not rules
- Overconfidence → force “Unknown/Insufficient data” plus explicit assumptions
- Inconsistent style → provide an output schema and style block
- Factual errors → require sources, or use retrieval, then verify

Helpful references:
- OpenAI prompt engineering guide: https://platform.openai.com/docs/guides/prompt-engineering
- OpenAI evals guide: https://platform.openai.com/docs/guides/evals

---

## 5) Landscape: models vs assistants
Think in two layers:
- Models: engines (capabilities, context length, latency, cost)
- Assistants: products packaging models with UX, memory, tools and connectors

Selection heuristics:
1. Risk: higher-risk tasks require stronger controls, not just “better models”
2. Data: where data goes, what is retained, what can be isolated
3. Workflow: docs, meetings, IDE, APIs, agents, automations
4. Cost and latency: speed vs depth
5. Governance: admin controls, audit logs, policy enforcement

---

## 6) Tooling map for an AI Generalist
The tool map, forty-plus tools by category with the corrections of 18 October 2026 (KST), is [tool-map.md](tool-map.md). Tools churn; the categories are the durable layer. Re-verify every link before use.

---

## 7) Mix and remix: how AI Generalists build workflows

### 7.1 Pattern 1: Prompt → structured output → reuse
1. Write one Magic Prompt for a recurring task
2. Produce output in a fixed schema
3. Save prompt and schema as a template
4. Re-run with new inputs

### 7.2 Pattern 2: Front door prompt → backend orchestration → UI
Example composition:
1. Draft a strong “front door” prompt (fixed inputs, fixed outputs)
2. Move the same prompt into an orchestration layer with tool permissions
3. Run the workflow repeatedly with logs and evaluations
4. Plug outputs into a simple UI for adoption

### 7.3 Pattern 3: Voice agents with Vapi
1. Define role and allowed actions
2. Write the call script as policy, not improvisation
3. Add hard stops and escalation triggers
4. Log calls, decisions and exceptions

### 7.4 Pattern 4: Local hosting when privacy constraints are real
- Use local models for privacy, cost control or offline work
- Treat local models as still risky: hallucinations persist, tool access can still leak
- Keep the same controls: gates, logs, evals, rollback

---

## 8) Essential concepts for safe agentic work

### 8.1 MCP is essential
MCP is a standard for connecting AI applications to tools and data sources.
- MCP home: https://modelcontextprotocol.io/
- MCP specification (current, 2026-07-28): https://modelcontextprotocol.io/specification/2026-07-28

### 8.2 Prompt injection and tool risk (the practical version)
When a model can call tools, untrusted content can try to:
- Exfiltrate secrets
- Rewrite files or records
- Trigger actions that look reasonable

Controls:
1. Least-privilege tool permissions
2. Allowlists for actions
3. Separation of duties for high-impact actions
4. Human approval gates
5. Logging and monitoring

### 8.3 Threat literacy you can actually use
Baseline references:
- OWASP Top 10 for LLM Applications 2026 (current list, published 3 August 2026, OWASP GenAI Security Project): https://genai.owasp.org/resource/owasp-genai-llm-top-10-2026/
- MITRE ATLAS: https://atlas.mitre.org/
- OWASP LLM Top 10 legacy project page: https://owasp.org/www-project-top-10-for-large-language-model-applications/
- OWASP LLM Top 10 project repository: https://github.com/OWASP/www-project-top-10-for-large-language-model-applications

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

---

## 10) Vibe coding, safely
Vibe coding compresses time-to-prototype. It can also ship invisible risk.

Safe rules:
1. Keep secrets out of prompts and repos
2. Require tests, even basic smoke tests
3. Use dependency scanning and security linting
4. Use staged rollout and rollback
5. Human review remains mandatory for production

---

## 11) Corporate use cases (cross-functional)

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
- Agent workflows touching tickets, repos and deployments, with gates

---

## 14) Recommended Readings and Reference Map

### Level 1: working literacy
1. NIST AI RMF overview: https://www.nist.gov/itl/ai-risk-management-framework
2. NIST AI RMF 1.0 (PDF): https://nvlpubs.nist.gov/nistpubs/ai/nist.ai.100-1.pdf
3. MITRE ATLAS: https://atlas.mitre.org/
4. OWASP Top 10 for LLM Applications 2026 (current list, published 3 August 2026): https://genai.owasp.org/resource/owasp-genai-llm-top-10-2026/
5. OWASP LLM Top 10 repo: https://github.com/OWASP/www-project-top-10-for-large-language-model-applications

### Level 2: building and connecting tools
1. MCP home: https://modelcontextprotocol.io/
2. MCP specification (current, 2026-07-28): https://modelcontextprotocol.io/specification/2026-07-28
3. OpenRouter: https://openrouter.ai/
4. Apify docs: https://docs.apify.com/
5. Vapi docs: https://docs.vapi.ai/

### Level 3: management systems and governance
1. ISO/IEC 42001:2023 standard overview: https://www.iso.org/standard/42001
2. ISO 42001 explained: https://www.iso.org/home/insights-news/resources/iso-42001-explained-what-it-is.html
3. NIST GenAI profile (AI RMF profile for GenAI, NIST AI 600-1) (PDF): https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf
4. EU AI Act (Regulation (EU) 2024/1689): https://eur-lex.europa.eu/eli/reg/2024/1689/oj, as amended by Regulation (EU) 2026/1744 of 8 July 2026, in force 27 July 2026: http://data.europa.eu/eli/reg/2026/1744/oj; the timetable as amended is in the EU AI Act currency note: https://github.com/rolldabones/ai-governance-for-boards/blob/main/05-jurisdictions/eu.md#eu-ai-act-currency-note

### Reading Map (by role)
- Executives and functional leaders
  1. NIST AI RMF overview (Level 1, item 1)
  2. ISO/IEC 42001 overview (Level 3, item 1)
  3. ISO 42001 explained (Level 3, item 2)

- Workflow owners and operators
  1. OWASP Top 10 for LLM Applications (Level 1, item 4)
  2. MCP home (Level 2, item 1)
  3. NotebookLM (tool-map.md)

- Security and IT
  1. MITRE ATLAS (Level 1, item 3)
  2. OWASP Top 10 for LLM Applications (Level 1, item 4)
  3. MCP specification (Level 2, item 2)
  4. Apify docs (Level 2, item 4)

- Legal and compliance
  1. ISO/IEC 42001 overview (Level 3, item 1)
  2. NIST AI RMF 1.0 (PDF) (Level 1, item 2)
  3. EU AI Act (Regulation (EU) 2024/1689, as amended by Regulation (EU) 2026/1744) (Level 3, item 4)
  4. OWASP Top 10 for LLM Applications (Level 1, item 4)

- Engineering and product
  1. MCP home (Level 2, item 1)
  2. OpenRouter (Level 2, item 3)
  3. Ollama (tool-map.md)
  4. Replit (tool-map.md)
  5. Bolt (tool-map.md)

---

**Final Liability rests with the Human.**
