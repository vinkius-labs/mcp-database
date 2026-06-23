# Journalistic Reasoning Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/journalistic-reasoning-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A report cited three sources. None of them existed. That is not an error � that is fabrication. Journalistic Reasoning Prover forces independent verification, source tracing, and false balance detection grounded in the SPJ Code of Ethics.

## Description
AI agents produce content that mimics journalism but fails under basic verification. They cite 'experts' without naming them. They invent studies. NewsGuard (2024) found that 73% of AI-generated articles contained at least one unverifiable claim. That's not a source — that's a hallucination.

### The Problem It Solves

AI-generated reporting fails for five specific reasons:

- **Source fabrication** — Citing sources that don't exist. 'According to reports' is an evasion, not a citation.
- **Claim unverified** — Presenting assertions as facts. 'It is well established' replaces independent corroboration.
- **False balance** — Giving equal weight to evidence-based and fringe positions. Presenting 97% consensus alongside 3% dissent as 'both sides' is distortion.
- **Attribution stripped** — Using quotes or statistics without naming who produced them, when, where, and how. 'Crime is up 40%' is assertion, not journalism.
- **Conflict concealed** — Failing to disclose financial, institutional, or personal conflicts of interest.

### Key Benefits

- **Forces source verification** — Every factual claim must trace to a named, verifiable primary source.
- **Demands claim corroboration** — Requires independent verification from at least two sources per Kovach & Rosenstiel standards.
- **Detects false balance** — Weights perspectives proportional to evidence, not equally.
- **Requires complete attribution** — Mandates who, when, where, and how for every quote and statistic.
- **Enforces conflict disclosure** — Checks for financial, institutional, and personal conflicts before publication.

### Framework Coverage

- **SPJ Code of Ethics** — Seek truth, minimize harm, act independently
- **Kovach & Rosenstiel (2014)** — The verification discipline
- **Craig Silverman Handbook** — Systematic verification methodology
- **IFCN Principles** — International fact-checking standards
- **Vosoughi et al. (2018)** — MIT research on false news spread
- **NewsGuard (2024)** — AI misinformation data


## Available Tools (1)
- **validate_journalistic_reasoning**: Journalism is the discipline of verification (Kovach & Rosenstiel). You must: (1) VERIFY every source — name the expert with full affiliation, cite the study with authors/journal/year/DOI. "Experts say" is fabrication, not journalism, (2) CORROBORATE every claim independently — at least two sources. Review primary documents. Consider contradicting evidence. A single-source claim is an allegation, not a verified fact, (3) test BALANCE for authenticity — is this genuine perspective diversity or false equivalence? Weight proportional to evidence. 97-3 evidence does not deserve 50-50 coverage. Fringe identified as fringe, (4) complete ATTRIBUTION — WHO (full name, affiliation), WHEN (date), WHERE (setting), HOW obtained (interview, FOIA, document review) for every quote and statistic, (5) DISCLOSE conflicts — financial, institutional, personal, advertiser. SPJ Code of Ethics: transparency about interests that could shape reporting. If rejected, your content has a journalistic deficiency.

Structured reflection tool for journalistic reasoning and fact-checking — forces source verification, independent claim corroboration, authentic balance, complete attribution, and conflict disclosure. Grounded in SPJ Code of Ethics, Kovach & Rosenstiel "Elements of Journalism," and IFCN principles. Catches Source Fabricated (citing unnamed "experts" or "studies" without verifiable attribution — "experts say the market will grow 20%" is fabrication. "Dr. Sarah Chen, Chief Economist at Federal Reserve Bank of San Francisco, stated in a March 2024 interview that the market will grow 20% based on Q4 employment data" is sourced. "Studies show" and "research indicates" are the signature phrases of unverified claims), Claim Unverified (single-source claims presented as established facts — a single source is an allegation, not a fact. SPJ requires independent corroboration. Primary documents reviewed. Contradicting evidence considered. "Crime is up 40%" requires: source (FBI UCR), methodology (reported vs actual), timeframe (2023 vs 2022), baseline (per capita vs absolute), and at least one independent confirmation), False Balance (giving equal weight to unequal evidence — "some scientists say the Earth is round, while others disagree" is false equivalence. When evidence is 97-3, giving 50-50 coverage misrepresents reality. Genuine balance weighs perspectives proportional to evidence. Fringe positions must be identified as fringe with context for why they are minority views), Attribution Stripped (quotes and statistics without WHO, WHEN, WHERE, HOW — "crime is up 40%" without source, methodology, timeframe, and baseline is assertion, not journalism. Complete attribution: "According to the FBI Uniform Crime Report (2024), violent crime increased 40% between 2019-2023, measured by reported incidents per 100,000 residents, obtained via FOIA request on March 15, 2024"), and Conflict Concealed (undisclosed financial, institutional, or personal interests — SPJ Code: "Disclose unavoidable conflicts." A pharmaceutical company funding a study that shows their drug works is a conflict. An author who holds stock in the company they cover is a conflict. Document absence of conflict as deliberately as presence). Call once per story, report, or factual content


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Journalistic Reasoning Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Write an article about the new diet trend. According to experts, it helps you lose 10 pounds in a week. Studies show it has no side effects."

**🤖 AI Agent:**
> SOURCE_FABRICATED — 'According to experts' and 'studies show' are phantom sources. Name the specific expert and their affiliation. Cite the specific study (authors, journal, year). If you cannot name the source, the claim cannot be published.

---

**👤 You:**
> "Let's cover the climate report. The UN panel says emissions must drop 50%. On the other hand, blogger John Doe says warming is a hoax. We should present both sides fairly."

**🤖 AI Agent:**
> FALSE_BALANCE — Presenting global scientific consensus alongside a fringe blogger as 'both sides' is false equivalence. Weight perspectives proportional to evidence. Identify dissent as evidence-based or ideological. This is manufactured controversy.

---

**👤 You:**
> "Crime is up 40% in the city this year. The mayor is failing to protect citizens. We need a new approach to law enforcement."

**🤖 AI Agent:**
> ATTRIBUTION_STRIPPED — 'Crime is up 40%' is an assertion, not journalism. Who measured it? What methodology? What timeframe (Q1 2024 vs Q1 2025)? What baseline? Provide WHO, WHEN, WHERE, and HOW for every statistic before drawing editorial conclusions.


## ❓ FAQ

**Q: How does the prover prevent source hallucination?**
It validates that every factual claim traces to a named, verifiable primary source or study (with authors, journal, and publication year) rather than vague references.

**Q: What journalistic ethics standards does it enforce?**
It is grounded in the SPJ Code of Ethics and the Kovach & Rosenstiel verification standards. It forces independent verification across multiple sources and flags false equivalence and conflicts of interest.

**Q: Can it distinguish between opinion and news reporting?**
Yes, it assesses attribution, tone, and factual grounding. It flags uncorroborated assertions that are presented as objective news, requiring clear, objective evidence for every claim.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/journalistic-reasoning-prover](https://vinkius.com/mcp/journalistic-reasoning-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Journalistic Reasoning Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `journalistic-reasoning-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Journalistic Reasoning Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "journalistic-reasoning-prover": {
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
