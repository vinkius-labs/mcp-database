# Legal Reasoning Prover MCP Server

A legal memo cited cases that do not exist and confused jurisdiction. Legal Reasoning Prover forces IRAC-based arguments grounded in US law — real Bluebook citations, jurisdiction analysis, ABA-compliant counter-arguments, and specific remedies.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/legal-reasoning-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
AI agents hallucinate legal citations at an alarming rate. Stanford HAI (2024) documented that LLMs fabricate case names in 30-40% of legal analysis outputs. The citations look right — proper party names, plausible reporter volumes, realistic court designations. But the cases don't exist. The holdings are invented. And the conclusions don't follow from the rules stated.

### The Problem It Solves

AI-generated legal reasoning fails for five specific reasons:

- **Broken syllogism** — The conclusion doesn't follow from the rule applied to the facts. The agent states a legal standard, then leaps to a conclusion without showing how the facts satisfy each element.
- **Phantom authority** — Fabricated case citations. "Smith v. Jones, 542 F.3d 891 (9th Cir. 2019)" — sounds real, doesn't exist. LLMs generate these with complete confidence.
- **Jurisdiction blindness** — Analysis that says "the law provides" without specifying which court, which state, which circuit, whether Erie applies, or what standard of review governs.
- **Missing counter-argument** — One-sided analysis that ignores adverse authority. Under ABA Model Rule 3.3(a)(2), counsel must disclose directly adverse controlling authority.
- **Detached remedy** — Legal analysis disconnected from actionable relief. "Consult an attorney" is not a remedy. "File a 12(b)(6) motion under Twombly/Iqbal" is.

### Key Benefits

- **Eliminates phantom citations** — Catches fabricated case names, placeholder parties, and weasel authority language before they reach your memo.
- **Enforces IRAC discipline** — Every legal conclusion must trace back through Issue, Rule, Application, and Conclusion with verifiable logical steps.
- **Requires jurisdiction specificity** — No more "under applicable law." The agent must name the court, the governing law, and the choice-of-law basis.
- **Guarantees adversarial rigor** — Forces the agent to confront the strongest counter-argument, not just present a one-sided analysis.
- **Connects analysis to action** — Every legal analysis must end with a specific procedural remedy: motion type, statutory basis, and relief sought.

### US Legal Framework Coverage

- **IRAC Method** — Issue, Rule, Application, Conclusion
- **Bluebook Citation** — 21st Edition standard
- **ABA Model Rules** — Professional conduct requirements
- **Erie Doctrine** — Federal/state choice of law
- **FRCP/FRE** — Federal Rules of Civil Procedure and Evidence
- **Stare Decisis** — SCOTUS > Circuit > District hierarchy
- **Standards of Review** — De novo, abuse of discretion, clearly erroneous, substantial evidence


## Available Tools
- **validate_legal_reasoning**: You must: (1) frame the legal ISSUE with governing rule and disputed facts — specific enough that a judge could understand the controversy from this paragraph alone, (2) state the controlling RULE — statute with section, regulation with CFR cite, or case holding with full Bluebook citation. "The law provides" is not a rule statement, (3) APPLY the rule to the specific facts — show the logical bridge element by element. Each element of the rule mapped to a specific fact, (4) cite REAL authorities — actual cases with volume, reporter, page, court, year, and the specific holding relied upon. LLMs hallucinate 30-40% of citations, (5) identify the JURISDICTION — federal vs. state, which circuit or district, Erie analysis for substantive law, choice-of-law if multi-state, (6) address the strongest COUNTER-ARGUMENT — ABA Rule 3.3(a)(2) mandates disclosure of adverse controlling authority. State the opposing position at its strongest, then distinguish, (7) propose a SPECIFIC remedy — procedural vehicle, rule basis, relief sought, timing. "Consult an attorney" is not a remedy. If rejected, fix the structural deficiency before advising.

Structured reflection tool for US legal reasoning — forces IRAC methodology, Bluebook-verifiable citations, jurisdiction identification, counter-argument engagement, and actionable remedies grounded in ABA Model Rules and federal/state procedural frameworks. Catches Syllogism Broken (the legal conclusion does not follow from the rule applied to the facts — "the contract is void because the defendant acted in bad faith" skips the syllogism. Major premise: under Restatement (Second) of Contracts § 205, every contract imposes an obligation of good faith and fair dealing. Minor premise: the defendant refused to process legitimate claims for 6 months despite contractual obligation. Conclusion: the defendant breached the implied covenant. If the conclusion does not follow from premise + facts, the reasoning is broken), Authority Ungrounded (citing fabricated or inaccurately characterized cases — LLMs hallucinate 30-40% of legal citations. "Johnson v. State (2021)" with no reporter volume, no page, no court is unverifiable. A Bluebook citation: "Bell Atl. Corp. v. Twombly, 550 U.S. 544, 570 (2007) — plausibility standard for pleadings." The holding must be accurately stated — mischaracterizing a holding is worse than no citation), Jurisdiction Blind (analyzing without identifying which court has jurisdiction and why — subject matter jurisdiction (federal question under 28 U.S.C. § 1331, diversity under § 1332, supplemental under § 1367), personal jurisdiction (minimum contacts under Int'l Shoe Co. v. Washington, 326 U.S. 310 (1945)), governing substantive law under Erie, and choice-of-law analysis. "Under US law" is not jurisdiction — the US has 50 states, 94 federal districts, and 13 circuits), Counter Absent (ignoring adverse authority in violation of ABA Model Rule 3.3(a)(2) — counsel must disclose directly adverse controlling authority in the jurisdiction. "There are no counterarguments" means the analysis is incomplete. The opposing position must be stated at its strongest, then distinguished on facts, law, or policy), and Remedy Detached (concluding with "consult an attorney" instead of a specific procedural step — a remedy must name the procedural vehicle (Motion for Summary Judgment under FRCP 56, Complaint under FRCP 8, Appeal under FRAP 4), the statutory basis, the specific relief sought (injunction scope, damages theory, declaratory judgment), and the standard of review). Call once per legal issue or IRAC analysis


## Installation & Usage

To install and use the **Legal Reasoning Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/legal-reasoning-prover](https://vinkius.com/mcp/legal-reasoning-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
