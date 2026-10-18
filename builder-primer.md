# The AI Generalist: Builder Primer

Son-U Michael Paik · CEO, GRC Solutions Korea

**v2.0.0 · 18 October 2026 (KST)**

Standalone; outside the workshop objectives. Section 15 of the workshop as it stood at v1.1.4, for novices building a website or a webapp with AI assistance.

## Builder Primer: websites and webapps, for novices (standalone)

### 15.1 Two build modes and the fastest way to choose

1) Website mode  
- Goal: improve user flow and conversion  
- Typical work: page redesign, copy, forms, performance, accessibility, instrumentation  

2) Webapp mode  
- Goal: deliver a workflow with state and business rules  
- Typical work: frontend + backend + project data store (“Vault”) + APIs + auth + logs + deployment  

Shared discipline:
- Define the metric
- Define the user
- Define the stop rules

### 15.2 The build pipeline (a repeatable loop that converges)
1. Rules and guidelines (one-page control surface)
   - Objective metric and target
   - Primary user and top failure points
   - Scope: in, out, deferred
   - Vault: what project data exists, who can access it, retention
   - Non-negotiables: security, privacy, review gates
2. Discover
   - Map the happy path and top 3 failure paths
   - Identify dependencies and constraints
3. MVP
   - One end-to-end path
   - Basic error handling
   - Measurement
4. Design
   - Aesthetic direction plus usability checks
5. Spec
   - Product requirements and technical spec, short is fine, missing is expensive
6. Build
   - Implement
   - Add logs
   - Staging deploy
   - Rollback plan
7. Measure
   - Track the metric and failure points
8. Iterate
   - One improvement at a time
   - Logged and testable

### 15.3 Web fundamentals you must know (minimum)
Core mental model: client-server requests and responses, including HTTP status codes.
- MDN HTTP overview: https://developer.mozilla.org/en-US/docs/Web/HTTP
- MDN HTTP response status codes: https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Status

### 15.4 The Vault (project data store), clarified
“Vault” = data relevant to the project, treated as a first-class component.

Minimum Vault decisions:
1. What data exists (entities and fields)
2. Who can read, write, delete (authorization rules)
3. Retention and deletion
4. Audit trail: what events must be logged

Practical implication:
- Many fast prototypes fail in production because Vault rules are implicit, not enforced.

### 15.5 Nonfunctional basics (the novice gap)

A) Security baseline  
Use OWASP as a default awareness checklist, then tighten per your environment:
- OWASP home: https://owasp.org/
- OWASP ASVS (Application Security Verification Standard): https://owasp.org/www-project-application-security-verification-standard/

B) Accessibility baseline  
- WCAG 2.2 Quick Reference: https://www.w3.org/WAI/WCAG22/quickref/

C) Performance baseline  
Use Core Web Vitals (LCP, INP, CLS) plus measurement tooling:
- Core Web Vitals overview: https://web.dev/articles/vitals

D) Quality checks, fast  
- Lighthouse: https://developer.chrome.com/docs/lighthouse/overview/

E) Logging mindset  
Treat logs as event streams:
- 12-factor logs: https://12factor.net/logs

### 15.6 Website mode playbook (conversion)
1. Baseline measure (conversion, bounce, load time)
2. Redesign one page or one funnel step
3. Run Lighthouse
4. Run a WCAG quick pass
5. Ship to staging, then deploy
6. Measure, then iterate

### 15.7 Webapp mode playbook (frontend + backend + Vault)
1. Sketch client-server flow (requests, responses)
2. Define Vault data model and access rules
3. Define APIs and error behavior
4. Implement happy path, then top 3 failure paths
5. Add logs, staging deploy, rollback
6. Measure task success, errors, latency

### 15.8 Prompting and build work: one practical rule
Prompts can draft and scaffold. The system must still pass gates:
- Security baseline (OWASP, plus your internal policies)
- Accessibility baseline (WCAG)
- Performance baseline (Core Web Vitals, Lighthouse)
- Logging and rollback

Prompt structure references:
- OpenAI prompt engineering guide: https://platform.openai.com/docs/guides/prompt-engineering
- OpenAI evals guide: https://platform.openai.com/docs/guides/evals

---

**Final Liability rests with the Human.**
