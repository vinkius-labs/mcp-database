# Customer Discovery Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/customer-discovery-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

An AI defined the ICP as 'busy professionals aged 25-45 who value productivity.' It described the problem as 'everyone struggles with time management.' Interview questions: 'Would you pay $29/month for this?' The startup built for 14 months, launched to silence, and shut down. 42% of startups fail because of no market need — and the discovery process guaranteed it. This tool forces persona grounding in real interviews, problem evidence from specific conversations, Mom Test methodology, segment separation, and willingness-to-pay commitment signals.

## Description
AI agents define customer personas from demographics and assumptions — then the startup builds for 14 months and launches to silence. They invent ICPs from stereotypes. They assert problems without citing a single conversation. They write leading interview questions. They treat all small businesses as one segment. They confuse verbal interest with willingness-to-pay.

### The Problem

LLMs commit five customer discovery failures that kill startups:

- **Invented Persona** — 'Busy professionals aged 25-45 who value productivity.' That is a demographic, not a persona. No interviews conducted. No observed behaviors. No specific pain point from a specific person at a specific company.
- **Assumed Problem** — 'Everyone struggles with time management.' Who said this? When? How often? What does it cost them? 'The market needs' is an assumption — evidence comes from conversations, not assertions.
- **Biased Validation** — 'Would you pay $29/month for this?' The most biased question in discovery. People say yes to be polite. The Mom Test: ask about past behavior ('When did you last encounter X? What did you do?'), never about future promises.
- **Conflated Segments** — 'Our target: SMBs.' A 5-person design agency and a 200-person manufacturer are both 'SMBs' — they have nothing else in common. Different pains, different budgets, different buying processes, different decision makers.
- **Untested WTP** — 'Strong interest from potential customers.' 'They said they would pay.' Verbal interest costs nothing. Willingness-to-pay requires commitment: a deposit, a signed letter of intent, a scheduled pilot with dates, or an introduction to a colleague.

### How It Works

Customer Discovery Prover validates discovery rigor through 5 Decision Pivots:

1. **personaGrounded** — ICP built from real interview data. Named people, specific roles, observed behaviors, current workarounds. Not demographics.
2. **problemEvidenced** — Pain validated with specific conversations. Quotes, frequencies, severity, cost of current workaround. Not 'the market needs.'
3. **validationUnbiased** — Methodology follows The Mom Test. Past behavior questions, falsification attempts, commitment asks. Not 'would you pay for this.'
4. **segmentsSeparated** — Distinct buyer groups with different pains, budgets, and buying processes. Not 'SMBs' or 'enterprise' as monolithic groups.
5. **wtpTested** — Willingness-to-pay tested with commitment signals. Deposits, LOIs, pilot dates, referrals. Not verbal interest.

### The Verdict Matrix

| First Failing Pivot | Verdict | Meaning |
|---|---|---|
| personaGrounded = false | PERSONA_INVENTED | Demographic, not persona. No real interviews. |
| problemEvidenced = false | PROBLEM_ASSUMED | Assertion, not evidence. No specific conversations. |
| validationUnbiased = false | VALIDATION_BIASED | Leading questions. Confirming, not discovering. |
| segmentsSeparated = false | SEGMENTS_CONFLATED | One group. Different buyers treated as identical. |
| wtpTested = false | WTP_UNTESTED | Verbal interest. No commitment signal. |
| All pivots pass | DISCOVERY_PROVEN | Grounded, evidenced, unbiased, separated, tested. |

### Why It Works

- **Tool calls are obligations.** The agent cannot skip persona grounding or claim validated discovery without citing specific interview quotes. Filling the fields IS the discovery work.
- **Consistency engine catches contradictions.** If the agent claims `validationUnbiased=true` but asks 'would you pay for this,' the engine rejects with Mom Test coaching.
- **Semantic traps detect hand-waving.** Phrases like 'busy professionals,' 'the market needs,' 'would you pay for,' 'SMBs,' and 'strong interest' trigger automatic rejection. Name the person. Cite the conversation. Show the commitment.


## Available Tools
- **validate_customer_discovery**: Think like a YC partner reviewing a pitch — "How do you know?" is the only question that matters. You must: (1) ground the PERSONA in real interview data — named people, specific roles, observed behaviors. "Busy professionals" is a demographic, not a persona. "Sarah, VP Eng at a 200-person fintech, spends 8h/week manually reconciling data" is a persona, (2) evidence the PROBLEM with specific conversations — who said what, how often it happens, what it costs them, what they do today to work around it. "The market needs X" is not evidence, (3) apply THE MOM TEST — ask about past behavior ("when did you last encounter this?"), never about future intentions ("would you pay for this?"). Seek falsification ("what would make this NOT useful?"). Extract commitment ("can you introduce me to your team lead?"), (4) separate SEGMENTS — different buyer groups have different pains, budgets, and buying processes. "Enterprise" is not a segment. "Head of Data at Series B fintechs with 50-200 employees using Snowflake" is a segment, (5) test WTP with COMMITMENT signals — deposits, LOIs, pilot dates with specific dates, referrals. "They said they would pay" is verbal interest, not willingness-to-pay. Money or time committed is WTP. If rejected, your discovery is assumption-based, not evidence-based.

Structured reflection tool for customer discovery grounded in real interviews, not invented personas. Forces the agent to evidence every claim with named interviews, apply The Mom Test methodology, separate buyer segments with distinct pains, and test willingness-to-pay with commitment signals. Catches Invented Personas ("busy professionals aged 25-45" — demographics are not personas. A persona needs a name, a role, a company context, observed behaviors, and interview quotes), Assumed Problems ("the market needs X" without citing specific conversations where someone described the pain, its frequency, and what they currently spend solving it), Biased Validation ("would you pay for this?" — leading questions produce false positives. The Mom Test: ask about past behavior, never about future intentions), Conflated Segments (treating "SMBs" as one group when a 5-person agency and a 200-person SaaS company have different pains, budgets, and buying processes), and Untested WTP ("they said they would pay" — verbal interest is not willingness-to-pay. Commitment signals: deposits, LOIs, pilot dates, referrals). Call once per customer persona, segment analysis, or product-market fit evaluation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Customer Discovery Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Our target customer is tech-savvy millennials who value productivity. The market clearly needs better project management tools. We asked 20 people if they would pay for this and 85% said yes."

**🤖 AI Agent:**
> PERSONA_INVENTED — 'Tech-savvy millennials who value productivity' is a demographic, not a persona. Who specifically? What role? What company? What is their specific pain — not 'productivity,' a behavior you observed? Also: 'Would you pay for this?' is a leading question (Mom Test violation) and '85% said yes' is biased validation, not WTP. This discovery fails on 4 of 5 axes.

---

**👤 You:**
> "Persona: 23 interviews with engineering managers at B2B SaaS companies (50-200 employees). Named: Sarah K. (VP Eng, fintech, 180 people), Mike R. (Eng Manager, healthtech, 85 people), Lisa T. (CTO, edtech, 60 people). Problem: 19/23 spend 6+ hours/week reconciling sprint data across Jira, Slack, and spreadsheets. Sarah: 'I lose every Monday morning to copying numbers between tools. It's 2026 and I'm doing manual data entry.' Current workaround: $2,400/year on Zapier + custom scripts, still takes 4 hours/week. Methodology: past behavior only — 'Walk me through your last sprint planning. What took the longest? What did you try to fix it?' Falsification: 'What would make this tool NOT worth switching for?' 8/23 said switching cost is the barrier. Segments: Segment A — VP Eng at 100-200 person companies, buying trigger is board reporting pressure, budget $500-1000/month, 6-week sales cycle. Segment B — Eng Managers at 50-100 person companies, buying trigger is team growth pain, budget $200-400/month, 2-week self-serve. WTP: 3 signed LOIs (Sarah K., Mike R., one unnamed), 2 paid pilots at $400/month starting June 15, Sarah agreed to be a launch case study."

**🤖 AI Agent:**
> DISCOVERY_PROVEN — Rigorous customer discovery validated. Persona: 23 named interviews, 3 specific people cited with roles and company context. Problem: 19/23 confirmation with quoted pain and $2,400/year workaround cost. Methodology: past behavior questions, falsification attempted (8/23 cited switching cost). Segments: VP Eng (100-200, board pressure, $500-1000) vs. Eng Manager (50-100, growth pain, $200-400). WTP: 3 LOIs, 2 paid pilots at $400/month with start dates, case study commitment. This discovery survives investor scrutiny.

---

**👤 You:**
> "Persona: 15 interviews with operations managers at manufacturing companies. Problem: 12/15 report spending 10+ hours/week on inventory reconciliation. Methodology: past behavior — 'Describe your last inventory audit. What went wrong?' Segments: We target SMBs in manufacturing. WTP: Strong interest from 8 companies, 3 requested demos."

**🤖 AI Agent:**
> SEGMENTS_CONFLATED — Persona, problem, and methodology pass. But segments fail: 'SMBs in manufacturing' is one label, not segmented. A 20-person machine shop and a 180-person food processor have different inventory systems, compliance requirements, budgets, and decision makers. Separate by: company size, sub-industry, regulatory requirements, and buying process. Also: WTP fails — 'strong interest' and 'requested demos' are not commitment. Show deposits, LOIs, or pilot agreements with dates.


## ❓ FAQ

**Q: Does it conduct interviews?**
No. It validates that your discovery process is grounded in real data — interview evidence, unbiased methodology, separated segments, and commitment-based WTP signals. It does not replace conversations with customers. It forces you to prove you had them.

**Q: What is The Mom Test?**
A framework by Rob Fitzpatrick for conducting customer interviews that produce truthful data. The core rule: never ask leading questions about the future ('Would you use this?'). Instead, ask about past behavior ('When did you last encounter X? What did you do?'). People lie about future behavior — past behavior is a reliable signal.

**Q: Can pre-product startups use this?**
Yes — it is designed for pre-product discovery. WTP signals for pre-product include: signed LOIs, paid design partnerships, deposits against future delivery, time commitments (agreed to a weekly feedback session), and reputation commitments (willing to be named as a design partner). You do not need a product to test willingness-to-pay.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/customer-discovery-prover](https://vinkius.com/mcp/customer-discovery-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Customer Discovery Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `customer-discovery-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Customer Discovery Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "customer-discovery-prover": {
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
