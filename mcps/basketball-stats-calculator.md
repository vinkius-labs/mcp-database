# Basketball Stats Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/basketball-stats-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Compute advanced basketball metrics like TS%, eFG%, USG%, and PER.

## Description
This MCP server provides a deterministic engine for calculating advanced basketball analytics. It allows AI agents to transform raw box score data into meaningful efficiency and impact metrics. Use `calculate_shooting_metrics` to find True Shooting and Effective Field Goal percentages, `calculate_usage_and_per_36` to determine Usage Rate and normalized per-36 minute statistics, and `calculate_impact_ratings` to evaluate Player Efficiency Rating (PER), Offensive/Defensive Ratings, and Win Shares. It is designed to help analysts and fans understand player productivity relative to team pace.


## Available Tools (3)
- **calculate_impact_ratings**: Calculate impact ratings
- **calculate_shooting_metrics**: Calculate shooting efficiency
- **calculate_usage_and_per_36**: Calculate usage and per-36 stats


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Basketball Stats Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the shooting efficiency for a player with 20 points, 8 FGM, 15 FGA, 2 3PM, 5 FTM, and 6 FTA."

**🤖 AI Agent:**
> The player's True Shooting Percentage (TS%) is 61.2% and the Effective Field Goal Percentage (eFG%) is 53.3%.

---

**👤 You:**
> "What are the per-36 minute stats for a player with 15 points, 5 rebounds, 4 assists, 2 steals, 1 block, and 2 turnovers in 20 minutes played, given a team pace of 100?"

**🤖 AI Agent:**
> The player's per-36 minute stats are 27.0 points, 9.0 rebounds, 7.2 assists, 3.6 steals, 1.8 blocks, and 3.6 turnovers.

---

**👤 You:**
> "Calculate the impact ratings for a player with 25 points, 10 rebounds, 5 assists, 2 steals, 1 block, 3 turnovers, 10 FGA, 4 FTA, 20 minutes played, and a team pace of 100."

**🤖 AI Agent:**
> The player's simplified PER is 24.5, Offensive Rating is 115.0, Defensive Rating is 102.0, and Win Shares is 4.2.


## ❓ FAQ

**Q: What metrics can I calculate?**
You can calculate shooting efficiency (TS%, eFG%), usage rate (USG%), per-36 minute normalized stats, and impact ratings including PER, Offensive/Defensive Ratings, and Win Shares.

**Q: Do I need to provide team pace?**
Yes, providing the team pace (possessions per 48 minutes) is required for calculating usage rate and pace-adjusted impact ratings.

**Q: How is the per-36 minute stat calculated?**
The `calculate_usage_and_per_36` tool scales raw statistics by multiplying them by 36 and dividing by the total minutes played.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/basketball-stats-calculator](https://vinkius.com/ai-agent-connect/basketball-stats-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Basketball Stats Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `basketball-stats-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Basketball Stats Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "basketball-stats-calculator": {
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
