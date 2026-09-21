# Passing Accuracy Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/passing-accuracy-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

High-precision football analytics for passing metrics.

## Description
This MCP server provides high-precision football analytics for evaluating ball distribution. It allows AI agents to calculate core metrics like completion, progressive, and key pass rates using `calculate_passing_stats`. Users can also use `compare_passing_performance` to evaluate differences between players or teams, `validate_integrity` to ensure data consistency, and `get_tier_summary` to categorize performance into tiers like Elite or Playmaker.


## Available Tools (4)
- **calculate_passing_stats**: Calculates core passing performance metrics for a single entity
- **compare_passing_performance**: Compares the passing profiles of two different entities
- **get_tier_summary**: Categorizes a player's passing profile into a performance tier
- **validate_integrity**: Verifies that a set of pass counts is logically consistent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Passing Accuracy Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the passing stats for a player with 50 attempts, 45 completed, 15 progressive, 5 key, and 2 turnovers."

**🤖 AI Agent:**
> The player has a completion rate of 0.9, a progressive rate of 0.3, a key rate of 0.1, and a turnover rate of 0.04.

---

**👤 You:**
> "Compare a player with 0.9 completion and 0.3 progressive rate against one with 0.8 completion and 0.2 progressive rate."

**🤖 AI Agent:**
> The first player is superior with a delta completion of 0.1 and a delta progressive rate of 0.1.

---

**👤 You:**
> "What tier is a player in with a 0.95 completion rate and 0.4 progressive rate?"

**🤖 AI Agent:**
> The player is in the Elite tier.


## ❓ FAQ

**Q: How do I calculate a player's passing profile?**
Use the `calculate_passing_stats` tool by providing the total attempts, completed passes, progressive passes, key passes, and turnovers.

**Q: Can I compare two different players?**
Yes, use `compare_passing_performance` by providing the JSON-stringified stats for both entities.

**Q: What determines a player's performance tier?**
The `get_tier_summary` tool categorizes players based on their completion and progressive pass rates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/passing-accuracy-calculator](https://vinkius.com/en/ai-agent-connect/passing-accuracy-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Passing Accuracy Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `passing-accuracy-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Passing Accuracy Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "passing-accuracy-calculator": {
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
