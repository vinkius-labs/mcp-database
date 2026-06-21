# Legal Reasoning Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/legal-reasoning-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A legal memo cited cases that do not exist and confused jurisdiction. Legal Reasoning Prover forces IRAC-based arguments grounded in US law — real Bluebook citations, jurisdiction analysis, ABA-compliant counter-arguments, and specific remedies.

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


## Available Tools (1)
- **validate_legal_reasoning**: You must: (1) frame the legal ISSUE with governing rule and disputed facts — specific enough that a judge could understand the controversy from this paragraph alone, (2) state the controlling RULE — statute with section, regulation with CFR cite, or case holding with full Bluebook citation. "The law provides" is not a rule statement, (3) APPLY the rule to the specific facts — show the logical bridge element by element. Each element of the rule mapped to a specific fact, (4) cite REAL authorities — actual cases with volume, reporter, page, court, year, and the specific holding relied upon. LLMs hallucinate 30-40% of citations, (5) identify the JURISDICTION — federal vs. state, which circuit or district, Erie analysis for substantive law, choice-of-law if multi-state, (6) address the strongest COUNTER-ARGUMENT — ABA Rule 3.3(a)(2) mandates disclosure of adverse controlling authority. State the opposing position at its strongest, then distinguish, (7) propose a SPECIFIC remedy — procedural vehicle, rule basis, relief sought, timing. "Consult an attorney" is not a remedy. If rejected, fix the structural deficiency before advising.

Structured reflection tool for US legal reasoning — forces IRAC methodology, Bluebook-verifiable citations, jurisdiction identification, counter-argument engagement, and actionable remedies grounded in ABA Model Rules and federal/state procedural frameworks. Catches Syllogism Broken (the legal conclusion does not follow from the rule applied to the facts — "the contract is void because the defendant acted in bad faith" skips the syllogism. Major premise: under Restatement (Second) of Contracts § 205, every contract imposes an obligation of good faith and fair dealing. Minor premise: the defendant refused to process legitimate claims for 6 months despite contractual obligation. Conclusion: the defendant breached the implied covenant. If the conclusion does not follow from premise + facts, the reasoning is broken), Authority Ungrounded (citing fabricated or inaccurately characterized cases — LLMs hallucinate 30-40% of legal citations. "Johnson v. State (2021)" with no reporter volume, no page, no court is unverifiable. A Bluebook citation: "Bell Atl. Corp. v. Twombly, 550 U.S. 544, 570 (2007) — plausibility standard for pleadings." The holding must be accurately stated — mischaracterizing a holding is worse than no citation), Jurisdiction Blind (analyzing without identifying which court has jurisdiction and why — subject matter jurisdiction (federal question under 28 U.S.C. § 1331, diversity under § 1332, supplemental under § 1367), personal jurisdiction (minimum contacts under Int'l Shoe Co. v. Washington, 326 U.S. 310 (1945)), governing substantive law under Erie, and choice-of-law analysis. "Under US law" is not jurisdiction — the US has 50 states, 94 federal districts, and 13 circuits), Counter Absent (ignoring adverse authority in violation of ABA Model Rule 3.3(a)(2) — counsel must disclose directly adverse controlling authority in the jurisdiction. "There are no counterarguments" means the analysis is incomplete. The opposing position must be stated at its strongest, then distinguished on facts, law, or policy), and Remedy Detached (concluding with "consult an attorney" instead of a specific procedural step — a remedy must name the procedural vehicle (Motion for Summary Judgment under FRCP 56, Complaint under FRCP 8, Appeal under FRAP 4), the statutory basis, the specific relief sought (injunction scope, damages theory, declaratory judgment), and the standard of review). Call once per legal issue or IRAC analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Legal Reasoning Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "A client was fired after reporting safety violations. Analyze whether they have a wrongful termination claim under federal law."

**🤖 AI Agent:**
> Verdict: JURISDICTION_BLIND. You state 'federal law' but don't identify which statute — SOX § 806 (public company whistleblower)? OSHA § 11(c) (workplace safety retaliation)? False Claims Act 31 U.S.C. § 3730(h) (government contractor fraud)? Each has different elements, filing deadlines, and administrative exhaustion requirements. Name the statute, the court, and whether the employee exhausted administrative remedies before filing suit.

---

**👤 You:**
> "Issue: Whether employer violated Title VII (PDA) by terminating employee after pregnancy announcement. Rule: 42 U.S.C. § 2000e; McDonnell Douglas, 411 U.S. 792 (1973). Application: Pregnancy announced March 1, PIP March 15 (no prior warnings), terminated April 1. Three comparable non-pregnant employees retained. Jurisdiction: NDIL, 7th Circuit. Counter: Employer claims performance; Ortiz v. Werner, 834 F.3d 760 (7th Cir. 2016). Remedy: EEOC charge within 300 days, back pay, damages capped $300K."

**🤖 AI Agent:**
> Verdict: REASONING_PROVEN. Syllogism sound — PDA elements mapped to facts (temporal proximity, no prior warnings, comparator retention). Authority grounded — McDonnell Douglas and Ortiz v. Werner properly cited. Jurisdiction identified — NDIL, 7th Circuit, 28 U.S.C. § 1331. Counter addressed — pretext analysis distinguishes performance defense. Remedy specific — EEOC timeline, damages cap, statutory fees.

---

**👤 You:**
> "The contract has a non-compete clause. Analyze whether it's enforceable. Courts have generally held that non-competes must be reasonable. The law supports the client's position that this is too broad."

**🤖 AI Agent:**
> Multiple rejections. (1) AUTHORITY_UNGROUNDED — 'courts have generally held' is weasel authority. Which court? Which case? (2) JURISDICTION_BLIND — non-compete enforceability varies by state. California bans them (Bus. & Prof. Code § 16600), Texas requires ancillary agreement, Illinois requires $75K salary. Which state governs? (3) SYLLOGISM_BROKEN — 'too broad' lacks element-by-element analysis of scope, duration, and restriction.


## ❓ FAQ

**Q: Does it verify if cited cases actually exist?**
It catches the most common hallucination patterns — placeholder names like 'Smith v. Jones' and 'Doe v. Roe', weasel authority language like 'courts have generally held', and citations that lack proper Bluebook format. It cannot access legal databases to verify every case, but it forces the agent to provide full citation details (party names, reporter, court, year, specific holding) — which dramatically reduces fabrication because the agent must commit to verifiable specifics.

**Q: Is it only for litigation or does it work for transactional law?**
The IRAC framework is most natural for litigation analysis, but the five pivots apply broadly. For transactional work: the 'syllogism' becomes 'does the contract structure achieve the stated objective?', 'authority' becomes 'is the statutory basis for this structure valid?', 'jurisdiction' becomes 'which state law governs this agreement?', and 'remedy' becomes 'what happens if the counterparty breaches?' The reasoning validation is universal — the domain language adapts.

**Q: Does it generate legal advice?**
No. Legal Reasoning Prover generates zero content. It validates the STRUCTURE of legal reasoning — whether the argument follows IRAC, whether citations are properly formed, whether jurisdiction is identified, whether counter-arguments are addressed. The agent does the legal analysis; the tool proves whether that analysis is structurally sound. It is a reasoning quality gate, not a legal advisor.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/legal-reasoning-prover](https://vinkius.com/mcp/legal-reasoning-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Legal Reasoning Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `legal-reasoning-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Legal Reasoning Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "legal-reasoning-prover": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
