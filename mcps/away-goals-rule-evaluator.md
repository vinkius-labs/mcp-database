# Away Goals Rule Evaluator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/away-goals-rule-evaluator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Determines the winner of two-legged football ties using aggregate scores and away goals rules.

## Description
This MCP server provides tools to evaluate two-legged football ties. It calculates aggregate scores and applies the away-goals rule to determine a winner or identify if a tie must proceed to a next stage like extra time. Use `evaluate_tie` to find the winner, `get_tie_summary` for scorelines, `validate_scores` to ensure data integrity, and `check_away_goal_advantage` to verify away goal status.


## Available Tools (4)
- **check_away_goal_advantage**: 
- **evaluate_tie**: 
- **get_tie_summary**: 
- **validate_scores**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Away Goals Rule Evaluator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Team A won 2-1 at home and lost 0-1 away. Team B won 1-0 at home and lost 1-2 away. The away-goals rule is enabled. Who won?"

**🤖 AI Agent:**
> Team A won with an aggregate score of 2-2 and 1 away goal compared to Team B's 0 away goals.

---

**👤 You:**
> "Calculate the tie result for Team A (Home: 1, Away: 1) and Team B (Home: 1, Away: 1) with the away-goals rule enabled."

**🤖 AI Agent:**
> The tie moves to the next stage because aggregate scores and away goals are identical.

---

**👤 You:**
> "Get a summary for Team A (Home: 3, Away: 0) and Team B (Home: 0, Away: 3) with the away-goals rule enabled."

**🤖 AI Agent:**
> The aggregate score is 3-3, and the away-goals rule was applied to determine the winner.


## ❓ FAQ

**Q: How does the away-goals rule work in this tool?**
When aggregate scores are tied and the rule is enabled, the team with more away goals is declared the winner via `evaluate_tie`.

**Q: Can I validate if my input scores are valid?**
Yes, you can use the `validate_scores` tool to ensure all goal counts are non-negative integers.

**Q: What happens if the away-goals rule is disabled?**
If the rule is disabled and aggregate scores are tied, the tie will proceed to the next stage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/away-goals-rule-evaluator](https://vinkius.com/en/ai-agent-connect/away-goals-rule-evaluator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Away Goals Rule Evaluator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `away-goals-rule-evaluator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Away Goals Rule Evaluator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "away-goals-rule-evaluator": {
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
