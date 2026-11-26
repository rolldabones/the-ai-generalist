# The AI Generalist

> **Archived edition of 26 November 2026.** This repository is archived and read-only. It receives no corrections, legal ones included: verify every statement of law, regulation or standard against a current primary source before you rely on it. What I maintain, and why this repository is not part of it, is in [DISPOSITION.md](https://github.com/rolldabones/rolldabones/blob/main/DISPOSITION.md). Cite this edition as *The AI Generalist*, v2.1.1 (26 November 2026). The license and [LICENSING.md](https://github.com/rolldabones/rolldabones/blob/main/LICENSING.md) still apply. Reach me at sonupaik@gmail.com. The workshop is brought current for each engagement; this edition is not.

**v2.1.1 · 26 November 2026 (KST) · Archived edition · One-day corporate workshop · License: CC BY-NC-SA 4.0**

A durable operating method for working professionals: what an LLM is, a repeatable prompting workflow, a tool selection map, governed workflow patterns and an AI governance, risk management and compliance (AI GRC) minimum control set. Usable as a participant primer, an instructor runbook and a reference map of dated links.

- **What it is:** a one-day workshop for working professionals, in the four files below.
- **Who it is for:** professionals who use AI at work and must keep it governed, plus the facilitators who run the day.
- **Start here:** participants read [participant-handout.md](participant-handout.md); facilitators read [facilitator-guide.md](facilitator-guide.md).
- **Run it:** agenda, materials and modules are in the facilitator guide; check every link in [tool-map.md](tool-map.md) before the day.
- **Cite it:** How to Cite below, or [CITATION.cff](CITATION.cff).

## Learning Objectives
By the end of this workshop participants will be able to:
1. Explain, at a working level, what a large language model (LLM) is, what it can and cannot do and why its failure modes are predictable.
2. Use a repeatable prompting workflow to produce higher quality outputs with fewer retries.
3. Choose the right tool for a task across chat, search, documents, meetings, coding, image, video and voice agents.
4. Design a simple “mix and remix” workflow across tools (prompt → backend orchestration → UI).
5. Apply **Slow AI**, **Informed Intent** and **Final Liability rests with the Human** to real corporate use cases using an AI governance, risk management and compliance (AI GRC) lens.
6. Build a lightweight control set: the eight controls of [participant-handout.md](participant-handout.md) section 2.4 (use-case registry, data rules, human gates, logging, evaluation, security, vendor and supply chain, change management).

## Contents

| File | What it is |
|---|---|
| [facilitator-guide.md](facilitator-guide.md) | Timed 8-hour agenda, materials, the 23 teaching notes, the five modules, the operating checklist |
| [participant-handout.md](participant-handout.md) | Sections 0 to 11 and 14; the eight controls are stated once, in 2.4 |
| [tool-map.md](tool-map.md) | 41 tools in 18 categories (17 with entries; Agentic coding tools is open), dated; links re-checked 20 October 2026 |
| [builder-primer.md](builder-primer.md) | Websites and webapps for novices; standalone, outside the objectives |

## Regulatory and standards currency

Each line carries its own as-at date (KST). A line dated before this release was not re-verified for it and is not re-dated.

- **NIST AI RMF 1.0** (NIST AI 100-1, January 2023) remains the published version. NIST states that "The AI RMF 1.0 is being revised as part of the White House AI Action Plan"; its framework page lists no revised version and lists the Generative AI Profile (NIST AI 600-1, July 2024). As at 15 November 2026.
- **ISO/IEC 42001:2023** (Edition 1, published December 2023) is the current edition of the AI management system standard. As at 14 July 2026; not re-verified since.
- **OWASP Top 10 for LLM Applications**: the current list is the 2026 edition (OWASP Top 10 for LLM Applications 2026, published 3 August 2026), maintained under the OWASP GenAI Security Project (genai.owasp.org/resource/owasp-genai-llm-top-10-2026/). As at 15 November 2026. The owasp.org project page points readers to the OWASP GenAI Security Project at genai.owasp.org. As at 20 October 2026; not re-verified since.
- **MCP specification**: the 2026-07-28 revision is published at modelcontextprotocol.io/specification/2026-07-28 and is current. Its base protocol is "Stateless, self-contained requests" with per-request capability negotiation; client features list Elicitation only; Tasks, Skills over MCP and MCP Apps are opt-in extensions. As at 15 November 2026. Roots, Sampling and Logging are deprecated in the 2026-07-28 revision (SEP-2577) and stay functional for at least twelve months. As at 20 October 2026; not re-verified since.
- **EU AI Act** (Regulation (EU) 2024/1689, as amended by Regulation (EU) 2026/1744 of 8 July 2026, in force 27 July 2026, which defers Annex III high-risk obligations to 2 December 2027 and Annex I to 2 August 2028) is cited as a reading reference only; the timetable as amended is stated once for the account in the [EU AI Act currency note](https://github.com/rolldabones/ai-governance-for-boards/blob/main/05-jurisdictions/eu.md#eu-ai-act-currency-note) in ai-governance-for-boards, and current status should be verified with counsel at time of use. As at 15 October 2026; not re-verified since.

This is a training reference, not a compliance representation. Verify the current status of any framework, standard or regulation before relying on it.

Primary sources: [NIST AI RMF](https://www.nist.gov/itl/ai-risk-management-framework), [ISO/IEC 42001](https://www.iso.org/standard/42001), [OWASP Top 10 for LLM Applications 2026](https://genai.owasp.org/resource/owasp-genai-llm-top-10-2026/), [MCP specification](https://modelcontextprotocol.io/specification/2026-07-28) and [Regulation (EU) 2024/1689](https://eur-lex.europa.eu/eli/reg/2024/1689/oj), as amended by [Regulation (EU) 2026/1744](http://data.europa.eu/eli/reg/2026/1744/oj); the full reading list is [participant-handout.md](participant-handout.md) section 14.

---

## Part of the ecosystem

This workshop is one entry point into a larger body of AI governance, risk management and compliance work. The canonical map of all repositories is [ECOSYSTEM.md](https://github.com/rolldabones/rolldabones/blob/main/ECOSYSTEM.md) in the profile repository.

The three doctrines are used in this repository as stated in [DOCTRINE.md](https://github.com/rolldabones/rolldabones/blob/main/DOCTRINE.md), the account's single normative statement. Where this repository restates a doctrine, it restates it at its own altitude and adds instruments, not doctrine (ECOSYSTEM.md protocol item 6).

Nearest neighbors:
- [slow-ai-kitchen](https://github.com/rolldabones/slow-ai-kitchen): the twelve-step governed AI methodology behind the workflow discipline taught here
- [grc-workbook](https://github.com/rolldabones/grc-workbook): the module-by-module instrument for building the integrated GRC capability the control set here previews
- [AI-Governance-Academy](https://github.com/rolldabones/AI-Governance-Academy): prompt templates for client-facing governance engagements, a natural follow-on for workshop participants
- [ai-governance-for-boards](https://github.com/rolldabones/ai-governance-for-boards): where the accountability questions raised here go when they reach the board
- [the-ungoverned-channel](https://github.com/rolldabones/the-ungoverned-channel): a live case study of what happens when the controls taught here are absent

---

## Closing: the AI Generalist’s rule set
1. Start with the decisions.
2. Use AI to accelerate drafts, not to replace accountability.
3. Constrain scope, control data and log the work.
4. Build small, ship safely, iterate.
5. Final Liability rests with the Human.

## License

CC BY-NC-SA 4.0 ([LICENSE](LICENSE)). Commercial use, including a Client's use in its own operations, is set out in [LICENSING.md](https://github.com/rolldabones/rolldabones/blob/main/LICENSING.md).

## How to Cite

> Paik, Son-U Michael. *The AI Generalist*, v2.1.1. GRC Solutions Korea, 2026. https://github.com/rolldabones/the-ai-generalist

A machine-readable citation is in [CITATION.cff](CITATION.cff).

**License: [CC BY-NC-SA 4.0](LICENSE) · Changes: [CHANGELOG.md](CHANGELOG.md)**

Acknowledgments: the tool map and the shape of the day derive from the Outskill [2-Day AI Mastermind](https://www.outskill.com/2-day-ai-mastermind) program, whose tool list and category walk the author reorganized into tool-map.md and the agenda; the doctrines, the control set, the exercises and the governance material are the author's own.

---

**Final Liability rests with the Human.**
