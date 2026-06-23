# Concurso Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/concurso-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate final examination scores, manage stage thresholds, and estimate competition rankings for civil service exams.

## Description
This MCP server provides specialized tools to automate the complex scoring logic of competitive examinations. Use `calculate_weighted_score` to determine a candidate's total score based on stage weights, and `verify_stage_thresholds` to ensure minimum requirements are met for each exam phase. You can also use `resolve_tiebreaker` to handle identical scores using a priority hierarchy, or `predict_ranking_position` to estimate a candidate's rank relative to available vacancies.


## Available Tools (4)
- **predict_ranking_position**: Estimates where a candidate stands in the overall competition relative to available job openings
- **calculate_weighted_score**: All stages in scores must have corresponding weights, and total weight must be 1.0.

Determines the total accumulated score for a candidate based on stage performance and importance weights
- **resolve_tiebreaker**: Decides a winner between two or more candidates who have identical final weighted scores
- **verify_stage_thresholds**: All stages in thresholds must be present in scores.

Checks if a candidate's performance meets the minimum requirements to remain in the competition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concurso Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total score for a candidate with 80 in Written (60%) and 90 in Oral (40%)."

**🤖 AI Agent:**
> The `calculate_weighted_score` tool would return a total score of 84.0.

---

**👤 You:**
> "Check if a candidate is qualified with scores: Written: 70, Oral: 50, where minimums are Written: 60, Oral: 60."

**🤖 AI Agent:**
> The `verify_stage_thresholds` tool would identify 'Oral' as a failed stage and return isQualified: false.

---

**👤 You:**
> "Predict the rank of a candidate with score 85 among competitors [90, 85, 80, 75] for 2 vacancies."

**🤖 AI Agent:**
> The `predict_ranking_position` tool would return an estimated rank of 2 and indicate the candidate is within the vacancy limit.


## ❓ FAQ

**Q: How does the weighted score calculation work?**
The `calculate_weighted_score` tool multiplies each stage's achieved score by its assigned weight. The sum of all weights must equal exactly 1.0 for a valid calculation.

**Q: What happens if a candidate fails a minimum threshold?**
Using `verify_stage_thresholds`, the system checks every stage. If any score is below the required minimum, the candidate is marked as disqualified.

**Q: How are ties resolved between candidates?**
The `resolve_tiebreaker` tool uses a pre-defined hierarchy of stages. It compares scores stage-by-stage, starting with the most important stage, until a difference is found.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/concurso-score-calculator](https://vinkius.com/mcp/concurso-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concurso Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concurso-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concurso Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concurso-score-calculator": {
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
