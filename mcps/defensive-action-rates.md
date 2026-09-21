# Defensive Action Rates MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/defensive-action-rates)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Calculate football defensive metrics including success rates, actions per 90, and efficiency comparisons.

## Description
This MCP server provides deep analytical tools for football defensive performance. It allows AI agents to retrieve detailed player summaries using `get_player_defensive_summary`, analyze team-wide defensive profiles with `get_team_defensive_profile`, and perform direct efficiency comparisons via `compare_defensive_efficiency`. Additionally, users can explore positional trends through `get_defensive_action_rates_by_role`. The server handles complex normalization, such as actions per 90 minutes and duel win percentages, providing precise data for player and team evaluations.


## Available Tools (4)
- **compare_defensive_efficiency**: How does player A's defensive efficiency compare to player B or a team average?
- **get_defensive_action_rates_by_role**: How do defensive metrics vary between different player roles?
- **get_player_defensive_summary**: What are the core defensive volume and efficiency metrics for a specific player?
- **get_team_defensive_profile**: How effective is a team's defense across all primary defensive actions?


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Defensive Action Rates** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the defensive stats for player ID 'p123'?"

**🤖 AI Agent:**
> Player p123 has an actions per 90 rate of 4.5 tackles and a tackle success rate of 72%.

---

**👤 You:**
> "How does player 'p123' compare to team 't456' in defensive efficiency?"

**🤖 AI Agent:**
> Player p123 has a 5% higher tackle success rate compared to the average for team t456.

---

**👤 You:**
> "Show me the average defensive metrics for midfielders."

**🤖 AI Agent:**
> The average for midfielders includes 3.2 interceptions per 90 and a 65% success rate on duels.


## ❓ FAQ

**Q: How is the 'actions per 90' metric calculated?**
The `get_player_defensive_summary` tool calculates actions per 90 by multiplying the raw action count by ninety and dividing by the total minutes played.

**Q: Can I compare a specific player to a team average?**
Yes, you can use `compare_defensive_efficiency` and set the `comparisonType` to 'team' to evaluate a player against a team's average performance.

**Q: What happens if a player has zero defensive actions recorded?**
If a denominator such as total attempts or minutes is zero, the specific rate will be returned as null with an explanation provided in the response.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/defensive-action-rates](https://vinkius.com/en/ai-agent-connect/defensive-action-rates)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Defensive Action Rates** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `defensive-action-rates` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Defensive Action Rates** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "defensive-action-rates": {
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
