# Changelog

All notable changes to this repository are documented here. Versioning follows [Semantic Versioning](https://semver.org/). The README and this file version in lockstep; prior versions are superseded, never silently overwritten.

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
