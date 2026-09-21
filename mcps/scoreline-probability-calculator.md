# Scoreline Probability Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/scoreline-probability-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [statistics](../categories/statistics.md)

Computes exact football scoreline probabilities from goal distributions or matrices.

## Description
This MCP server provides a mathematical engine to calculate the likelihood of specific football match outcomes. By using `calculate_from_distributions`, you can input independent goal probabilities for both teams to derive the most likely scorelines. Alternatively, use `calculate_from_matrix` to analyze a pre-defined joint probability space. The engine also supports identifying the single most probable outcome via `get_most_likely_scoreline` and determining how many outcomes are needed to reach a specific probability threshold using `get_scoreline_coverage`.


## Available Tools (4)
- **calculate_from_distributions**: Calculates exact scoreline probabilities by treating home and away goal counts as independent variables
- **calculate_from_matrix**: Extracts and ranks scoreline probabilities from a pre-defined joint probability matrix
- **get_most_likely_scoreline**: Identifies the single most probable scoreline for a given match configuration
- **get_scoreline_coverage**: Determines how many specific scorelines must be considered to reach a certain threshold of total match probability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scoreline Probability Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the most likely scoreline if the home team has a 50% chance of 1 goal and 30% chance of 2 goals, and the away team has a 40% chance of 0 goals and 40% chance of 1 goal?"

**🤖 AI Agent:**
> The most likely scoreline is 1-0 with a probability of 0.20.

---

**👤 You:**
> "Calculate the top 3 scorelines for these distributions: home [0.1, 0.5, 0.4] and away [0.2, 0.6, 0.2]."

**🤖 AI Agent:**
> The top 3 scorelines are 1-1 (0.30), 1-0 (0.12), and 0-1 (0.10).

---

**👤 You:**
> "Using a joint probability matrix [[0.1, 0.2], [0.3, 0.4]], what are the top 2 scorelines?"

**🤖 AI Agent:**
> The top 2 scorelines are 1-1 (0.40) and 1-0 (0.30).


## ❓ FAQ

**Q: How do I calculate the most likely scoreline?**
You can use the `get_most_likely_scoreline` tool by providing the probability arrays for both the home and away teams.

**Q: What is the difference between distribution and matrix inputs?**
Distributions treat home and away goals as independent events, while a matrix allows you to provide a joint probability where dependencies are already accounted for.

**Q: Can I find out how many scorelines cover 75% of the probability?**
Yes, use the `get_scoreline_coverage` tool and set the threshold parameter to 0.75.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/scoreline-probability-calculator](https://vinkius.com/en/ai-agent-connect/scoreline-probability-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scoreline Probability Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `scoreline-probability-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scoreline Probability Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scoreline-probability-calculator": {
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
