# Accelerator Selection Scoring MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-selection-scoring)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business](../categories/business.md)

Calculate weighted startup scores, adjust for interviewer bias, and evaluate cohort fit.

## Description
This MCP server provides a complete engine for ranking startup candidates in accelerator programs. It uses a weighted scoring model to calculate primary scores via `calculate_application_score`, applies corrective measures to mitigate interviewer tendencies with `apply_bias_correction`, and evaluates strategic alignment using `evaluate_cohort_impact`. Finally, it generates comprehensive selection analytics, including ranking percentiles and acceptance probabilities, through `generate_selection_analytics`.


## Available Tools (4)
- **calculate_application_score**: Calculates the primary weighted score for a single application
- **evaluate_cohort_impact**: Adjusts an application's score based on how well it fits the specific needs of the current cohort
- **generate_selection_analytics**: Provides a holistic view of an application's standing, including percentile and acceptance likelihood
- **apply_bias_correction**: Adjusts raw scores to mitigate the impact of individual interviewer tendencies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Selection Scoring** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the score for a startup with Team: 8, Market: 9, Product: 7, Traction: 6, and weights: team=0.4, market=0.3, product=0.2, traction=0.1."

**🤖 AI Agent:**
> The total weighted score for the application is 7.7.

---

**👤 You:**
> "An interviewer gave a score of 7, but the cohort average is 8. What is the adjusted score?"

**🤖 AI Agent:**
> The adjusted score has been moved toward the cohort average to mitigate bias.

---

**👤 You:**
> "What is the acceptance probability for a score of 8.5 when the historical threshold is 8.0 and the pool scores are [7.0, 7.5, 8.0, 8.5, 9.0]?"

**🤖 AI Agent:**
> The application has a high acceptance probability and ranks in the 80th percentile.


## ❓ FAQ

**Q: How does the scoring model handle different criteria?**
The `calculate_application_score` tool uses a weighted model where you assign decimal weights to Team, Market, Product, and Traction scores. The sum of these weights must equal 1.0.

**Q: Can I adjust for interviewers who are too lenient?**
Yes, the `apply_bias_correction` tool adjusts raw scores toward the cohort average to ensure fairness across different interviewers.

**Q: How is cohort fit calculated?**
The `evaluate_cohort_impact` tool takes a base score and a fit score to calculate a boost, which is then added to the base score (capped at 10) based on a specified weight.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-selection-scoring](https://vinkius.com/ai-agent-connect/accelerator-selection-scoring)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Selection Scoring** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-selection-scoring` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Selection Scoring** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-selection-scoring": {
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
