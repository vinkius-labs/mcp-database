# Both Teams to Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/both-teams-to-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculates mutually exclusive football scoring probabilities from a scoreline matrix.

## Description
This MCP server provides a mathematical engine to transform scoreline probability matrices into specific betting outcomes. Using the `calculate_scoring_outcomes` tool, you can derive the probabilities for Both Teams to Score (BTTS), Home Team Only, Away Team Only, and Neither team scoring. It supports configurable goal thresholds to define what constitutes a 'scoring' event. Additionally, you can use `validate_matrix_integrity` to ensure your probability distributions are mathematically sound and `get_scoreline_summary` to identify the most likely match results.


## Available Tools (4)
- **calculate_scoring_outcomes**: Calculates the four mutually exclusive scoring probabilities based on a provided matrix and a specific goal threshold
- **filter_matrix_by_threshold**: Returns a subset of the matrix containing only scorelines that meet a specific goal requirement for either team
- **get_scoreline_summary**: Provides a human-readable summary of the most likely scorelines and the total number of possible outcomes
- **validate_matrix_integrity**: 0.

Verifies if a given scoreline matrix is mathematically sound and complete


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Both Teams to Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the scoring probabilities for this matrix: {"0-0": 0.1, "1-0": 0.2, "0-1": 0.1, "1-1": 0.2, "2-0": 0.1, "0-2": 0.1, "2-1": 0.1, "1-2": 0.1}"

**🤖 AI Agent:**
> {"bttsProbability": 0.4, "homeOnlyProbability": 0.4, "awayOnlyProbability": 0.1, "neitherProbability": 0.1, "totalProbability": 1.0}

---

**👤 You:**
> "What is the most likely scoreline for this matrix: {"1-0": 0.4, "0-0": 0.3, "1-1": 0.2, "2-0": 0.1}"

**🤖 AI Agent:**
> {"mostLikelyScoreline": "1-0", "topThreeScorelines": ["1-0", "0-0", "1-1"], "totalOutcomes": 4}

---

**👤 You:**
> "Filter the matrix for scores where at least one team scores 2 or more goals: {"0-0": 0.2, "1-1": 0.3, "2-0": 0.2, "0-2": 0.2, "1-0": 0.1}"

**🤖 AI Agent:**
> {"filteredMatrix": {"2-0": 0.2, "0-2": 0.2}, "totalFilteredProbability": 0.4}


## ❓ FAQ

**Q: How do I ensure my scoreline matrix is valid?**
You can use the `validate_matrix_integrity` tool to verify that the sum of all probabilities in your matrix equals exactly 1.0.

**Q: Can I change the definition of a scoring team?**
Yes, by using the `minGoalThreshold` parameter in the `calculate_scoring_outcomes` tool, you can define the minimum goals required for a team to be considered as having scored.

**Q: What outcomes does the calculator provide?**
The engine returns four mutually exclusive outcomes: Both Teams to Score, Home Team Only, Away Team Only, and Neither Team to Score.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/both-teams-to-score-calculator](https://vinkius.com/en/ai-agent-connect/both-teams-to-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Both Teams to Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `both-teams-to-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Both Teams to Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "both-teams-to-score-calculator": {
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
