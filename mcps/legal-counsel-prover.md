# Legal Counsel Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/legal-counsel-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

AI agents cite fabricated statutes, ignore deadlines, and deliver one-sided legal memos. This tool forces rigorous reasoning: identify jurisdiction, cite verifiable law, map procedure, address the opposing argument, connect to the client's facts.

## Description
AI agents generating legal analysis produce dangerously confident output that falls apart under professional scrutiny. They cite non-existent statutes, fabricate case law, ignore statutes of limitation, present one-sided assessments, and deliver generic memos that could apply to any client in any jurisdiction.

### The Problem It Solves

AI-generated legal analysis fails on five axes:

- **Jurisdiction blindness** — "You can sue for breach of contract" without specifying which jurisdiction's law applies, which court has competence, or why
- **Statutory hallucination** — Citing "Article 47 of the Civil Code" when no such article exists, or fabricating case names and docket numbers
- **Procedural negligence** — "File a complaint" without mentioning the 2-year statute of limitations that expires next month, or the mandatory pre-litigation mediation
- **Risk whitewashing** — "You will win this case" without acknowledging the opposing party's strongest defense or adverse precedents
- **Client-fact disconnect** — Generic legal templates that start with "in general" instead of analyzing the client's specific dates, parties, events, and evidence

These aren't knowledge gaps. They're **reasoning gaps.** The agent never stops to ask: which law applies here? Can another attorney verify this citation? What is the deadline? What will the other side argue?

### How It Works

Legal Counsel Prover uses 5 Decision Pivots — boolean checkpoints that force the agent to validate its own legal reasoning before delivering analysis:

1. **jurisdictionIdentified** — Can you name the EXACT jurisdiction? Country, state/province, competent court, and basis for jurisdiction.
2. **legalBasisVerifiable** — Is the cited law specific enough for another attorney to locate? Statute number + article, or case name + court + date.
3. **proceduralRequirementsMapped** — Are ALL deadlines, mandatory steps, and prerequisites identified? Statutes of limitation, pre-litigation notices, filing rules.
4. **adverseAnalysisIncluded** — Have you addressed the opposing party's strongest arguments and identified weaknesses in your position?
5. **factPatternConnected** — Does the analysis connect to THIS client's specific facts — dates, parties, events, documents — not a generic framework?

The tool validates logical consistency. If the agent says `ANALYSIS_PROVEN` but `jurisdictionIdentified: false`, the tool rejects with a clear explanation. If the legal basis reads like a vague reference instead of a citable source, it rejects. If the adverse analysis dismisses the opposition entirely, it rejects.

### Why It Works

- **Tool calls are obligations, instructions are suggestions.** The agent can ignore "be specific about the jurisdiction" in a prompt. It cannot ignore a schema that requires naming the jurisdiction, citing verifiable law, and committing to a verdict.
- **The commit pattern.** The agent proposes its own verdict, then the server validates it against the pivots. This forced commitment deepens the reasoning — the agent must actively decide if its analysis is sound.
- **Semantic traps.** The engine catches legal-specific anti-patterns: vague citations ("the law says", "applicable provisions"), dismissive adverse analysis ("no counterargument", "guaranteed outcome"), boilerplate risk assessments ("consult a lawyer", "no risk"), and hypothetical fact analysis ("in general", "typically").


## Available Tools (1)
- **validate_legal_analysis**: You must: (1) identify the EXACT jurisdiction — country, state/province, federal vs. state, competent court, basis for jurisdiction (domicile, contract clause, subject matter). "Under applicable law" is never acceptable, (2) cite SPECIFIC legal bases — statute number and section, OR case name with Bluebook citation (volume, reporter, page, court, year), OR regulation with issuing body. Every citation must be verifiable by another attorney, (3) map ALL procedural requirements — statute of limitations with specific period and accrual date, mandatory pre-litigation steps (notice, mediation, administrative exhaustion), filing rules, appeal deadlines. Missing a deadline is malpractice, (4) address the STRONGEST adverse position — what the opposing party will argue, contrary precedents in the jurisdiction, factual weaknesses in the client's position. ABA Rule 3.3(a)(2) mandates disclosure of adverse authority, (5) connect every element to the CLIENT'S specific facts — dates, parties, events, documents, evidence. A framework without facts is a textbook, not counsel. If rejected, fix the specific gap before advising.

Structured reflection tool for legal analysis — forces jurisdictional precision, verifiable citations, procedural mapping, adverse engagement, and fact-pattern connection before any counsel is delivered. Catches Jurisdiction Blind (analyzing a contract dispute without identifying whether state or federal court has subject matter jurisdiction, which state's substantive law governs under Erie, or whether a forum selection clause controls — "under applicable law" is not jurisdiction analysis. A California non-compete analysis that ignores Business and Professions Code § 16600 is malpractice. A diversity jurisdiction claim that does not verify complete diversity and amount in controversy exceeding $75,000 under 28 U.S.C. § 1332 fails at the threshold), Basis Unverifiable (citing "the relevant statute provides" without naming it — LLMs hallucinate 30-40% of legal citations. "Smith v. Jones (2019)" with no reporter volume, no page number, no court, no holding is unverifiable. A proper Bluebook citation: "Twombly, 550 U.S. 544, 570 (2007) — held that a complaint must plead facts stating a claim plausible on its face." If another attorney cannot locate and verify the citation, it does not exist), Procedurally Negligent (missing a statute of limitations is malpractice, not an oversight — a personal injury claim in New York has a 3-year SOL under CPLR § 214. A mandatory pre-litigation notice under the Federal Tort Claims Act requires 2 years from accrual. A motion to compel arbitration must be filed before answering the complaint or waiver applies. Every procedural requirement has a deadline — missing one forfeits the client's rights), One-Sided Analysis (presenting only favorable authority without addressing the strongest counterargument — ABA Model Rule 3.3(a)(2) requires disclosure of directly adverse controlling authority in the jurisdiction. "There are no counterarguments" means you have not researched the issue. Every legal position has an adverse authority — the opposing counsel will find it even if you do not), and Fact Disconnected (delivering a generic legal framework without connecting it to the client's specific dates, parties, events, documents, and evidence — "breach of contract requires offer, acceptance, consideration, and breach" is a textbook, not counsel. "On March 15, 2024, the defendant signed the SaaS agreement [Exhibit A] containing a 12-month minimum commitment at $4,200/month" is fact-connected analysis). Call once per legal question or client matter


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Legal Counsel Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My client wants to sue their landlord for not returning the security deposit. Analyze this legal situation."

**🤖 AI Agent:**
> Verdict: JURISDICTION_BLIND. 'Sue the landlord' — under which jurisdiction's law? Which state or country? Which court has competence? Landlord-tenant law varies dramatically between jurisdictions. In New York, security deposit disputes go to Small Claims Court with a $10,000 limit. In São Paulo, it's a civil court action under Lei do Inquilinato. Without jurisdiction, there is no applicable law.

---

**👤 You:**
> "Under Brazilian law (Art. 37 of Lei 8.245/91), the landlord must return the security deposit within 30 days of lease termination. My client's lease ended on March 1, 2026, the deposit was R$5,000, and the landlord has not returned it despite written demand sent April 15. The property is in São Paulo. The landlord may argue deductions for damages, but the move-out inspection report signed by both parties shows no damage. Analyze."

**🤖 AI Agent:**
> Verdict: ANALYSIS_PROVEN. Jurisdiction identified (Brazilian law, São Paulo, Lei do Inquilinato). Legal basis verifiable (Art. 37, Lei 8.245/91). Procedural path mapped (30-day return period expired, written demand sent, civil court action in São Paulo). Adverse positions addressed (landlord's damage deduction defense neutralized by signed inspection report). Fact pattern connected (specific dates, amounts, documents cited). This analysis is ready for attorney review.

---

**👤 You:**
> "My client signed an NDA and now wants to report their employer's illegal dumping of toxic waste to the EPA. Under US federal law, they are protected by the Clean Water Act whistleblower provisions. There is no risk. They will certainly win."

**🤖 AI Agent:**
> Verdict: RISK_WHITEWASHED. Multiple failures. (1) 'No risk' and 'certainly win' are dangerous overstatements — whistleblower retaliation cases are notoriously complex. (2) The NDA may contain arbitration clauses affecting the procedural path. (3) The employer WILL argue the NDA applies and may seek injunctive relief. (4) Clean Water Act Section 507 has specific filing requirements (30 days from retaliation) — mapped those? Overconfidence is the most dangerous failure mode in legal analysis.


## ❓ FAQ

**Q: Does Legal Counsel Prover generate legal analysis or draft documents?**
No. Legal Counsel Prover performs zero content generation. It forces the AI agent to structure its own legal reasoning into verifiable fields, then validates that the reasoning is logically consistent. The agent does all the thinking — the tool catches jurisdiction gaps, unverifiable citations, procedural omissions, one-sided risk assessments, and fact-disconnected analysis.

**Q: What does it catch that a system prompt instruction doesn't?**
Prompt instructions are suggestions — agents routinely ignore 'always cite the specific statute' or 'consider the opposing argument.' Tool calls are obligations — the agent must fill every field. Beyond that, Legal Counsel Prover has 12 consistency rules that catch legal-specific anti-patterns: vague citations ('the law says', 'applicable provisions'), dismissive adverse analysis ('no counterargument', 'guaranteed outcome'), boilerplate risk assessments ('consult a lawyer', 'no risk'), and hypothetical fact analysis ('in general', 'typically'). A prompt can't enforce these — a tool schema can.

**Q: Does it replace a human attorney?**
Absolutely not. Legal Counsel Prover is a quality gate for AI-assisted legal reasoning. It ensures the AI agent has done the minimum due diligence before presenting analysis to an attorney for review. The tool validates reasoning structure — jurisdiction, citations, procedure, adverse analysis, fact connection — but it cannot verify the accuracy of legal citations or the correctness of legal conclusions. A human attorney must always review the output.

**Q: Which legal systems and jurisdictions does it support?**
Legal Counsel Prover is jurisdiction-agnostic — it validates reasoning structure, not legal content. It works with any legal system: common law, civil law, hybrid systems. The consistency rules check that the agent HAS identified a jurisdiction, cited verifiable law, and mapped procedural requirements — not whether those citations are correct. Whether you're analyzing Brazilian Civil Code, US federal statute, or French administrative law, the reasoning validation applies equally.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/legal-counsel-prover](https://vinkius.com/mcp/legal-counsel-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Legal Counsel Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `legal-counsel-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Legal Counsel Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "legal-counsel-prover": {
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
