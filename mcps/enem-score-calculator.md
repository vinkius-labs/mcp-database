# ENEM Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/enem-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Calculate ENEM performance metrics and simulate university admission possibilities based on historical cutoff scores.

## Description
This MCP server provides specialized tools to quantify student performance in the ENEM exam. Use `calculate_area_averages` to determine the arithmetic mean of objective exam areas. You can also use `calculate_weighted_score` to compute a final score based on specific subject weights, and `simulate_admission_possity` to compare your results against historical cutoff scores for various courses and universities.


## Available Tools
- **simulate_admission_possibility**: Compare a student's score against historical data to predict admission success
- **calculate_area_averages**: Calculate the arithmetic mean of the four objective exam areas
- **calculate_weighted_score**: Calculate the final performance score based on custom importance weights


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ENEM Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my average for the four objective areas with these scores: Languages 600, Math 700, Science 550, Humanities 650."

**🤖 AI Agent:**
> The `calculate_area_averages` tool would return an average score of 625.0.

---

**👤 You:**
> "Will I pass Medicine at University X if my weighted score is 800 in 2023?"

**🤖 AI Agent:**
> You can use `simulate_admission_possibility` with the course and university IDs to check this against historical records.

---

**👤 You:**
> "Calculate a weighted score: Languages 600 (weight 1), Math 700 (weight 2), Science 550 (weight 1), Humanities 650 (weight 1), and Essay 800 (weight 3)."

**🤖 AI Agent:**
> The `calculate_weighted_score` tool will process these inputs to return your final weighted performance score.


## ❓ FAQ

**Q: What is the purpose of this tool?**
It allows students to calculate their ENEM averages and simulate whether they would have met the cutoff scores for specific university courses in previous years.

**Q: How do I use the weighted score feature?**
Use the `calculate_weighted_score` tool by providing your subject scores, their corresponding weights, and your essay score as JSON objects.

**Q: Where does the historical data come from?**
The tool uses hardcoded historical cutoff scores for specific universities and courses within the server's internal data catalog.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/enem-score-calculator](https://vinkius.com/mcp/enem-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ENEM Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `enem-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ENEM Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enem-score-calculator": {
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
