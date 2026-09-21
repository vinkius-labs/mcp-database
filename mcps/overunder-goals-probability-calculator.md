# Over/Under Goals Probability Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/overunder-goals-probability-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [statistics](../categories/statistics.md)

Calculate football total-goals probabilities for any goal line using scoreline matrices.

## Description
This MCP server provides specialized tools for football (soccer) analysts to calculate the likelihood of total goals in a match. By providing a scoreline matrix (a distribution of possible match outcomes), users can determine the exact probabilities for 'Over', 'Under', and 'Push' scenarios across various goal lines. Use `calculate_over_under_probabilities` to find probabilities for specific thresholds, `get_distribution_summary` for statistical insights like expected total goals, or `filter_scorelines_by_total` to isolate specific goal counts. The server also includes `validate_matrix_integrity` to ensure your probability distributions are mathematically sound.


## Available Tools (4)
- **calculate_over_under_probabilities**: Calculates the probability of the total goals being over, under, or pushing a specific goal line
- **filter_scorelines_by_total**: Filters a distribution to only show outcomes that result in a specific total number of goals
- **get_distribution_summary**: Provides a high-level statistical summary of a provided goal distribution
- **validate_matrix_integrity**: Checks if a provided scoreline matrix is mathematically valid for probability calculations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Over/Under Goals Probability Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the over/under probabilities for a 2.5 goal line using this matrix: [{"homeGoals": 0, "awayGoals": 0, "probability": 0.1}, {"homeGoals": 1, "awayGoals": 0, "probability": 0.2}, {"homeGoals": 0, "awayGoals": 1, "probability": 0.2}, {"homeGoals": 1, "awayGoals": 1, "probability": 0.5}]"

**🤖 AI Agent:**
> {"overProbability": 0.5, "underProbability": 0.5, "pushProbability": 0.0}

---

**👤 You:**
> "What is the expected total goals for this distribution: [{"homeGoals": 1, "awayGoals": 0, "probability": 0.5}, {"homeGoals": 0, "awayGoals": 1, "probability": 0.5}]"

**🤖 AI Agent:**
> {"expectedTotalGoals": 1.0, "mostLikelyTotalGoals": 1, "probabilityOfZeroGoals": 0.0}

---

**👤 You:**
> "Check if this matrix is valid: [{"homeGoals": 1, "awayGoals": 0, "probability": 0.8}]"

**🤖 AI Agent:**
> {"isValid": false, "reason": "Probabilities sum to 0.8 instead of 1.0"}


## ❓ FAQ

**Q: What is a 'push' in goal probability?**
A 'push' occurs when the total goals scored exactly match the integer goal line. For half-integer lines like 2.5, a push is impossible.

**Q: How do I format the scoreline matrix?**
The matrix should be a JSON array of objects, where each object contains `homeGoals`, `awayGoals`, and `probability` (e.g., `[{"homeGoals": 1, "awayGoals": 0, "probability": 0.4}]`).

**Q: Can I use this with Claude Desktop?**
Yes, this server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/overunder-goals-probability-calculator](https://vinkius.com/en/ai-agent-connect/overunder-goals-probability-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Over/Under Goals Probability Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `overunder-goals-probability-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Over/Under Goals Probability Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "overunder-goals-probability-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
