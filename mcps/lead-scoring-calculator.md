# Lead Scoring Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lead-scoring-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Calculate a lead's conversion readiness score instantly using configurable firmographic and behavioral data points.

## Description
**How to Assess Lead Value in Minutes.**Finding high-potential leads is difficult. Traditional methods rely on guesswork or simple demographic matching, leading teams to waste time nurturing cold contacts. The core problem is accurately quantifying a lead's readiness for sales handoff.**The Solution: Weighted Predictive Scoring.** This calculator provides an objective score (0-100) based on measurable data. It operates in three steps:1. **Gather Profile Data:** We first use `query_lead_profile_data` to collect foundational attributes like company size, industry sector, and job title.2. **Retrieve Weights:** Next, we call `query_scoring_configuration` to fetch the latest scoring weights and qualification thresholds (e.g., what constitutes an MQL vs. SQL).3. **Calculate Score:** Finally, `calculate_converted_score` executes the weighted algorithm using all gathered data and configuration parameters, returning a composite score, classification status, and estimated conversion probability.**Key Advantage:** This system moves beyond simple lead counting. It provides actionable intelligence--a definitive status (Cold, Warm, Hot, MQL, SQL)--allowing sales teams to prioritize outreach based on calculated value, maximizing efficiency for the entire pipeline.


## Available Tools
- **calculate_converted_score**: Returns total score, qualification status (Cold/Warm/Hot/MQL/SQL), and estimated conversion probability.

Calculate composite lead score with qualification status and conversion probability
- **query_lead_profile_data**: Optionally specify a scoring version ID.

Retrieve raw lead profile data for scoring
- **query_scoring_configuration**: Retrieve current scoring configuration weights and thresholds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lead Scoring Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run a full scoring check for lead ID 'L12345' targeting the USA market. I need to know if they are MQL or SQL."

**🤖 AI Agent:**
> Calling `query_lead_profile_data` for L12345... Calling `query_scoring_configuration` for weights... Final score calculated via `calculate_converted_score`: Total Score 135/100. Status: SQL (Sales Qualified Lead). Conversion Probability Estimate: 85%-90% (High Confidence).

---

**👤 You:**
> "What is the current weight assigned to 'Director' job titles and what are the minimum scores for MQL in Europe?"

**🤖 AI Agent:**
> The scoring configuration tool provides this data. The `query_scoring_configuration` call reveals that 'Director' titles currently carry a weight of 30 points, and the minimum threshold for MQL in Europe is set at 80.

---

**👤 You:**
> "I have gathered all data for a new lead. Calculate the score."

**🤖 AI Agent:**
> The scoring process is complete. The final calculated score is [TOTAL_SCORE]/100, classifying the lead as a [STATUS]. This indicates a strong potential for conversion, with an estimated probability range of [PROBABILITY]% to [HIGH_END]%.


## ❓ FAQ

**Q: What types of signals does the calculator use?**
The scoring model is comprehensive. It combines static **Firmographic Signals** (like company size and industry sector) retrieved via `query_lead_profile_data` with dynamic **Behavioral Signals** (such as page visits or emails opened). The final score weights these signals to give a true picture of intent.

**Q: How configurable are the scoring rules?**
The model is highly flexible. It fetches all necessary weights and thresholds using `query_scoring_configuration`. This allows administrators to adjust the importance of any attribute (e.g., boosting the value of a 'Director' title) without changing core code.

**Q: What inputs are needed to get a final score?**
To calculate the final result, three pieces of information are required. First, you need raw lead data using `query_lead_profile_data`. Second, you must provide the scoring weights from `query_scoring_configuration`. These inputs feed into the core function, `calculate_converted_score`, which provides the total score and status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lead-scoring-calculator](https://vinkius.com/mcp/lead-scoring-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lead Scoring Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `lead-scoring-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lead Scoring Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lead-scoring-calculator": {
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
