# Points Per Game Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/points-per-game-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Calculate football performance metrics, PPG, and projected points.

## Description
This MCP server provides tools to analyze football match data. You can use `calculate_team_stats` to find a specific team's total points, matches played, and points per game (PPG). It also supports projecting future points based on current performance. For broader analysis, `compare_teams_performance` generates comparison tables for multiple teams, while `get_league_summary` provides a high-level overview of the entire league's activity. You can also use `validate_points_system` to ensure your scoring rules are mathematically sound.


## Available Tools (4)
- **calculate_team_stats**: Calculates performance metrics for a specific team
- **compare_teams_performance**: Compares performance of multiple teams
- **get_league_summary**: Provides a high-level league overview
- **validate_points_system**: Validates a points configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Points Per Game Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the stats for team 'Arsenal' given these results: [{'homeTeam': 'Arsenal', 'awayTeam': 'Chelsea', 'homeScore': 2, 'awayScore': 1}, {'homeTeam': 'Chelsea', 'awayTeam': 'Arsenal', 'homeScore': 0, 'awayScore': 0}] and a standard points system (win: 3, draw: 1, loss: 0)?"

**🤖 AI Agent:**
> Arsenal has played 2 matches, earned 4 total points, and has a points per game (PPG) of 2.0.

---

**👤 You:**
> "Compare the performance of 'Man City' and 'Liverpool' using these results: [{'homeTeam': 'Man City', 'awayTeam': 'Liverpool', 'homeScore': 1, 'awayScore': 1}, {'homeTeam': 'Liverpool', 'awayTeam': 'Man City', 'homeScore': 2, 'awayScore': 0}] and a standard points system (win: 3, draw: 1, loss: 0)."

**🤖 AI Agent:**
> Man City: 1 point, 1 match, 1.0 PPG. Liverpool: 4 points, 2 matches, 2.0 PPG.

---

**👤 You:**
> "Give me a league summary for these matches: [{'homeTeam': 'A', 'awayTeam': 'B', 'homeScore': 1, 'awayScore': 0}, {'homeTeam': 'C', 'awayTeam': 'A', 'homeScore': 1, 'awayScore': 1}] with a standard points system (win: 3, draw: 1, loss: 0)."

**🤖 AI Agent:**
> The league has 2 matches played, 3 unique teams, and a total of 4 points distributed.


## ❓ FAQ

**Q: How is Points Per Game (PPG) calculated?**
PPG is calculated by dividing the total points earned by the number of matches played by the team.

**Q: Can I project future points for a team?**
Yes, by using `calculate_team_stats` and providing a target match count, the tool will project points based on the current PPG.

**Q: How do I validate my scoring rules?**
You can use the `validate_points_system` tool to check if your win, draw, and loss values follow a logical progression.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/points-per-game-calculator](https://vinkius.com/en/ai-agent-connect/points-per-game-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Points Per Game Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `points-per-game-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Points Per Game Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "points-per-game-calculator": {
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
