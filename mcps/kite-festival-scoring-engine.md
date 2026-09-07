# Kite Festival Scoring Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/kite-festival-scoring-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sports](../categories/sports.md)

Calculates competition scores, weighted results, and athlete rankings for kite flying events.

## Description
This MCP server provides a specialized scoring engine for kite flying competitions. It allows AI agents to process technical performance metrics into comprehensive athlete rankings. Using `calculate_trick_score`, agents can determine the base value of maneuvers based on difficulty, execution, height, and landing. The engine also supports `calculate_weighted_score` to apply style multipliers and diversity bonuses, as well as `evaluate_rankings` to determine final standings and `get_competition_summary` for high-level event overviews.


## Available Tools (4)
- **calculate_trick_score**: Calculates the base value of a single maneuver
- **calculate_weighted_score**: Applies competitive weighting and stylistic modifiers to a trick's base score
- **evaluate_rankings**: Input must be a JSON string representing an array of objects with "name" and "score" fields.

Determines the final standing of all competitors in the event
- **get_competition_summary**: Input must be a JSON string representing an array of objects with "name" and "score" fields.

Provides a high-level overview of the current competition state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kite Festival Scoring Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the score for a trick with difficulty 8, execution 7, height 9, and landing 8."

**🤖 AI Agent:**
> The total trick score is 32.

---

**👤 You:**
> "Apply a style multiplier of 1.2 and a diversity bonus of 5 to a trick score of 30."

**🤖 AI Agent:**
> The final weighted score is 41.

---

**👤 You:**
> "What are the rankings for Alice (score 85), Bob (score 92), and Charlie (score 85)?"

**🤖 AI Agent:**
> 1. Bob (92), 2. Alice (85), 2. Charlie (85).


## ❓ FAQ

**Q: How do I calculate a single trick's score?**
You can use the `calculate_trick_score` tool by providing the difficulty, execution, height, and landing scores.

**Q: Can I apply style bonuses to the scores?**
Yes, use `calculate_weighted_score` to apply a style multiplier and an optional diversity bonus to a base score.

**Q: How are the final rankings determined?**
The `evaluate_rankings` tool sorts competitors by their total weighted scores in descending order.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/kite-festival-scoring-engine](https://vinkius.com/ai-agent-connect/kite-festival-scoring-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kite Festival Scoring Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kite-festival-scoring-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kite Festival Scoring Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kite-festival-scoring-engine": {
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
