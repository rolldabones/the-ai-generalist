# Changelog

All notable changes to this repository are documented here. Versioning follows [Semantic Versioning](https://semver.org/). The README and this file version in lockstep; prior versions are superseded, never silently overwritten.

## v2.0.0 (2026-10-18)

Front door and split into five files, session T7 of the whole-account review of 15 October 2026 (KST); review doc section 9 (change 6) and reviewer report 14, items 1, 3, 4, 5, 16 to 20, 23 and 25, and the :7 acknowledgments. Workshop content moved, not rewritten: every sentence of v1.1.4 is carried into one of the five files by programmatic slicing on the README's section headings, and the additions are listed here.

- **`README.md` is the front door.** Masthead at v2.0.0 with the KST date, the description paragraph as it stood, an entry path of five lines (what it is, who it is for, start here, run it, cite it), the Learning Objectives with objective 6 citing the eight controls of participant-handout.md section 2.4, a Contents table of the four companion files, the Regulatory and standards currency section as it stood plus one trailing line of primary-source links (the section's claims had lost their links to the handout, which the B3 guard reports), Part of the ecosystem as it stood, the closing rule set, How to Cite at v2.0.0, the license line and an Acknowledgments line stating that the tool map and the shape of the day derive from the Outskill 2-Day AI Mastermind program; the "Recommended program (inspiration)" line at :7 is removed (item 25). The file is 7.7 KB against the 6 KB target because the currency section (2.3 KB) and the ecosystem section (1.5 KB) are kept as they stood.
- **`facilitator-guide.md` added** (item 16): a timed agenda table for the 8-hour day in the house form of Academy template 03 Mode B (five blocks of 90, 90, 90, 90 and 45 minutes with two 15-minute breaks and a 45-minute lunch, each with purpose, facilitation steps with timings, exercise and expected artifact), a materials and prerequisites list, the 23 "(Teaching note: ...)" parentheticals of v1.1.4 lifted out of the participant text and placed under the section each belonged to, 21 collected by section and 2 kept in place in sections 12 and 13, which are facilitator text, former section 12 Practical exercises with Module 2 gaining the exercise data rule, synthetic inputs only and no Client or personal data (item 17), and Module 3 gaining the Tiny Servant definition in the account's form, the link to *Made to Hold* and a ten-line spec template with the fields purpose, inputs, outputs, boundaries, owner, exit, evidence, review, tier and done-when (item 18), and former section 13 Operating checklist with a pointer to the handout's section 2.4 as the one statement of the control set.
- **`participant-handout.md` added** (item 25): sections 0 to 11 and 14 with every teaching note removed (0 remain). Section 2.4 is the single statement of the eight controls; the five-item "Translate posture into controls" list in 2.1 becomes a pointer mapping its items to controls 3, 4, 5 and 8, and scope and escalation are folded into controls 1 and 3 (item 5). Section 3.3 gains three paragraphs on the context window, retrieval-augmented generation and agents, and thinking models, naming no model (item 19). Section 14 lists each URL once: the Level lists are numbered and the Reading Map by role cites them by level and item, the four tool entries pointing to tool-map.md (item 25, the re-listed URLs). Section 6 is one line pointing to tool-map.md.
- **`tool-map.md` added** (item 20): the 42 tools and two documentation links of section 6 regenerated as one list in 18 categories, dated 18 October 2026 (KST) with the author's last link verification of 14 July 2026 stated in the masthead; OpenRouter moved from agent platforms to a new "Model routers and gateways" category, Emergent and Emily moved to builders (category P of v1.1.4 merged into it), Happenstance moved to research, notes and people search, Kimi and Moonshot AI merged into one entry, and an "Agentic coding tools" category opened with no entry, since the v1.1.4 text named none and nothing is added that the author has not named. No URL was re-verified in this session; 41 tools remain.
- **`builder-primer.md` added**: former section 15 as it stood, with a masthead and one sentence placing it standalone and outside the workshop objectives.
- **Findings by class.** Confirmed and edited: items 5, 16, 17, 18, 19, 20, 25 and the :7 acknowledgments. Already fixed: items 1 and 4 (v1.1.3), 3 (v1.1.3 and v1.1.4) and 23 (v1.1.4, the serial comma at :11), verified by content. Not reproducible: none. Outside the review: none edited. Unknown: whether any tool URL in tool-map.md is still live (not re-verified from the session; the masthead says so).
- Masthead, How to Cite and `CITATION.cff` to 2.0.0 in lockstep. `LICENSE` unchanged.

## v1.1.4 (2026-10-17)

Doctrine short forms and the mechanical train, session T3 of the whole-account review of 15 October 2026 (KST); reviewer report 14, items 1, 5 and 23, and review doc sections 1 and 8.

- **Section 2.2, Informed Intent, conformed to DOCTRINE.md v1.2.0 section 8.** The authorization now names the four elements of the instrument, purpose, authority, boundaries and exit; it had listed purpose, scope and limits with a named owner and omitted exit, which DOCTRINE.md section 2 says leaves no authorization at all. Scope and limits are folded into Boundaries; the owner becomes Authority, given by a human meeting the five authorizer conditions. The teaching note states the exit rule.
- **Section 2.1, Slow AI, and section 2.3, Final Liability, conformed in the same way.** Slow AI is stated as the precondition, with the three tests (governed, explained, audited) carrying the earlier list of visible, monitored and pausable under "governed"; the heading reads "precondition" rather than "operating posture". Final Liability carries its sentence form and the three attributes, decision rights, oversight and the power to intervene; the earlier four-item list (decision authority, understanding of limits, ownership of consequences, ability to stop) did not reduce to them.
- **Objective 6 cites the control set by section.** It had named seven controls (scope, data handling, logging, human gates, evaluation, escalation, change management) against the eight of section 2.4, omitting security and vendor and supply chain and naming two the set does not hold; it now lists the eight.
- **House style.** One serial comma removed in Objective 1. How to Cite moves above the footer, so the closing line is the last line of the README, and it is set in bold; the closing line is added, last, to this changelog.
- Masthead (both occurrences), How to Cite and `CITATION.cff` to 1.1.4 in lockstep. Tool map, modules and every other section unchanged.

## v1.1.3 (2026-10-15)

Currency patch, session T1 of the whole-account review of 15 October 2026 (KST). Workshop content unchanged.

- **MCP references re-pointed.** The three links to the 2025-11-25 specification (Day 1 reading, Day 2 reading, the three-step build list) now point to the published 2026-07-28 revision, which the currency note of 14 July 2026 described as a release candidate and promised to review after publication; neither v1.1.1 nor v1.1.2 logged that review, so this entry is it. The note records what changed in the revision: a stateless base protocol with per-request capability negotiation, Elicitation as the only client feature, Tasks, Skills over MCP and MCP Apps as extensions. Verified at modelcontextprotocol.io on 15 October 2026 (KST). Reviewer report 14, item 3; review doc §3.
- **EU AI Act line** names Regulation (EU) 2026/1744 ([OJ L, 2026/1744](http://data.europa.eu/eli/reg/2026/1744/oj)) and the deferred dates and links to the account's canonical [EU AI Act currency note](https://github.com/rolldabones/ai-governance-for-boards/blob/main/05-jurisdictions/eu.md#eu-ai-act-currency-note), published the same day. Item 4.
- Masthead (both occurrences), How to Cite and `CITATION.cff` to 1.1.3 in lockstep. All other files unchanged byte for byte.

## v1.1.2 (2026-09-06)

Citation infrastructure, doctrine citation line and lockstep maintenance. Session C of the September 2026 improvement pack, one patch release per repository across all 21 public repositories.

- **`CITATION.cff` added** in the house form settled at D-C1: no `type` field, `version` and `date-released` in lockstep with the README, `license` as the SPDX identifier for this repository's licence, `abstract` taken from this repository's ECOSYSTEM.md role line rather than newly written.
- **How to Cite block** aligned to this release and pointing at `CITATION.cff`.
- **Doctrine citation line added** to the Part of the ecosystem section. This repository restates a doctrine and cited DOCTRINE.md nowhere, which is the Class E2 finding the new guards report.
- **Lockstep lag corrected, second occurrence.** The closing version block read `v1.1.0 · 14 July 2026` against a masthead of `v1.1.1`. Found by reading in Session C, not by any guard.
- All other files in this repository are unchanged byte for byte.

## v1.1.1 (2026-08-13)

License metadata sweep. An `SPDX-License-Identifier: CC-BY-NC-SA-4.0` line and the canonical Creative Commons legal code are now carried inside the existing license file. The filename is unchanged and the human-readable summary is retained above the legal code.

- The primary audience is automated intake and provenance tooling, which reads the SPDX tag rather than prose. Automated license detection previously reported nothing across all twenty-one repositories in this account.
- No change to the licence in force. The identifier records what was already true.

## v1.1.0 (2026-07-14)

First versioned release under the repository improvement program. The pre-existing README is treated as implicit v1.0.0.

### Added
- Version, date and license header; version and license footer.
- Section 2.2 Informed Intent (authorization gate), completing the three-doctrine set alongside Slow AI and Final Liability rests with the Human; former 2.2 and 2.3 renumbered to 2.3 and 2.4. Learning Objective 5 updated to name all three doctrines.
- Regulatory and standards currency section, dated 14 July 2026: NIST AI RMF 1.0 current with revision in progress per NIST; ISO/IEC 42001:2023 Edition 1 current; OWASP LLM Top 10 2025 edition under the OWASP GenAI Security Project; MCP 2025-11-25 current stable with 2026-07-28 revision at release-candidate stage; EU AI Act cited as reading reference only.
- EU AI Act (Regulation (EU) 2024/1689, EUR-Lex ELI link) added to Level 3 readings and the legal and compliance reading map.
- "Part of the ecosystem" section linking the canonical ECOSYSTEM.md and five nearest neighbors.
- Opening summary paragraph stating what the document is and its three intended uses.
- CHANGELOG.md and LICENSE (CC BY-NC-SA 4.0) added to the repository.

### Changed
- OWASP references updated to the current 2025 list at genai.owasp.org/llm-top-10/; the owasp.org project page retained and labeled as the legacy/archived v1.1 (2023) location.
- Chronicle moved from "Research and notes" to "Images, design and presentations" (category F renamed): it is an AI presentation tool, not a notes tool.
- Core Web Vitals link updated to the canonical https://web.dev/articles/vitals (old /vitals/ URL redirects).
- MDN HTTP status codes link updated to the canonical /docs/Web/HTTP/Reference/Status (old URL redirects).
- MCP specification links annotated as "current stable, 2025-11-25".
- House-style sweep: serial (Oxford) commas removed throughout prose.
- Section 6 intro notes that categories, not tools, are the durable layer.

### Verified (2026-07-14, KST)
- All standards and framework links resolve: NIST AI RMF overview and PDFs, ISO/IEC 42001 pages, OWASP GenAI Security Project, MITRE ATLAS, MCP specification, WCAG 2.2 quick reference, OWASP ASVS, MDN, web.dev, Lighthouse, 12factor.net.
- Tool links spot-checked live: Outskill program page, Chronicle, Emily (meetemily.ai), Kling, all core assistants.

## v1.0.0 (implicit)

Original single-file workshop primer (README.md only; no license, changelog or tags).

---

Final Liability rests with the Human.

---

**Final Liability rests with the Human.**
