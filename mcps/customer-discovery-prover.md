# Customer Discovery Prover MCP Server

An AI defined the ICP as 'busy professionals aged 25-45 who value productivity.' It described the problem as 'everyone struggles with time management.' Interview questions: 'Would you pay $29/month for this?' The startup built for 14 months, launched to silence, and shut down. 42% of startups fail because of no market need — and the discovery process guaranteed it. This tool forces persona grounding in real interviews, problem evidence from specific conversations, Mom Test methodology, segment separation, and willingness-to-pay commitment signals.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/customer-discovery-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

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


## Installation & Usage

To install and use the **Customer Discovery Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/customer-discovery-prover](https://vinkius.com/mcp/customer-discovery-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
