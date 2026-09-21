# Shooting Efficiency Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/shooting-efficiency-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Transform raw football shooting data into professional efficiency metrics and per-90 statistics.

## Description
This MCP server provides a specialized analytical engine for football performance analysis. It allows AI agents to process raw shooting statistics--such as total shots, shots on target, and expected goals (xG)--into high-level metrics like shot accuracy, conversion rates, and normalized per-90-minute statistics. Use `calculate_shooting_metrics` to generate a full efficiency profile, `compare_player_efficiency` to benchmark two players, or `validate_shot_integrity` to ensure statistical data is logically sound. It is designed to help analysts and fans understand player lethality and scoring patterns through precise mathematical modeling.


## Available Tools (4)
- **calculate_shooting_metrics**: Calculates comprehensive efficiency metrics for a player
- **compare_player_efficiency**: Compares two different shooting profiles
- **get_shooting_summary_by_volume**: Filters and categorizes players based on shot volume
- **validate_shot_integrity**: Verifies if shot statistics are mathematically and logically sound


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shooting Efficiency Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the efficiency for a player with 10 shots, 4 shots on target, 2 goals, 1.5 xG, and 90 minutes played."

**🤖 AI Agent:**
> The player has a shot accuracy of 40%, a conversion rate of 20%, and 0.5 xG overperformance. Their per-90 stats are 2.0 goals, 10.0 shots, and 4.0 shots on target.

---

**👤 You:**
> "Is it valid to have 5 shots, 6 shots on target, and 2 goals?"

**🤖 AI Agent:**
> No, the data is invalid because the number of shots on target cannot exceed the total number of shots.

---

**👤 You:**
> "Compare a player with a 20% conversion rate to a player with a 25% conversion rate."

**🤖 AI Agent:**
> The second player is more efficient with a 5% higher conversion rate.


## ❓ FAQ

**Q: How can I verify if my shooting data is logically consistent?**
You can use the `validate_shot_integrity` tool. It checks if the number of goals exceeds shots on target or if shots on target exceeds total shots, ensuring the data follows strict hierarchical rules.

**Q: Can I compare two players directly?**
Yes, the `compare_player_efficiency` tool allows you to compare specific metrics, such as conversion rate or goals per 90, between two player profiles to determine who is more clinical.

**Q: What metrics are included in the efficiency profile?**
The `calculate_shooting_metrics` tool provides shot accuracy, conversion rate, goals per shot, goals per shot on target, xG overperformance, and per-90 rates for goals, shots, and shots on target.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/shooting-efficiency-calculator](https://vinkius.com/en/ai-agent-connect/shooting-efficiency-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shooting Efficiency Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shooting-efficiency-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shooting Efficiency Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shooting-efficiency-calculator": {
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
