# MySportsFeeds MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mysportsfeeds)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time and historical sports data for NFL, MLB, NBA, NHL, and more—get standings, player stats, and game boxscores directly.

## Description
Connect to **MySportsFeeds** to bring professional sports data into your AI workflows. Query live scores, seasonal standings, and deep player statistics across major leagues including NFL, MLB, NBA, NHL, CBB, and CFB.

### What you can do

- **Standings & Schedules** — Retrieve seasonal standings and full game schedules for any supported league and season.
- **Boxscores & Play-by-Play** — Get detailed game results, starting lineups, and chronological play-by-play event logs.
- **Player & Team Stats** — Fetch cumulative totals for player and team performance metrics to analyze seasonal trends.
- **Injuries & Updates** — Stay informed with the latest player injury reports and track the most recent data feed updates.
- **Daily Coverage** — Access specific daily game schedules and player performance stats for active game days.

### How it works

1. Subscribe to this server
2. Enter your MySportsFeeds API Key
3. Start querying sports data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sports Analysts** — instantly retrieve historical data and seasonal totals for deep performance analysis
- **Fantasy Players** — check injury reports and daily player stats to optimize lineups without leaving your chat
- **Developers** — integrate professional sports data into applications or research projects via natural language


## Available Tools
- **get_daily_games**: Get daily games schedule
- **get_daily_player_stats**: Get daily player stats
- **get_game_boxscore**: Get game boxscore
- **get_game_lineup**: Get game lineup
- **get_game_playbyplay**: Get game play-by-play
- **get_latest_updates**: Get latest updates
- **get_player_injuries**: Get player injuries
- **get_player_stats_totals**: Get seasonal player stats totals
- **get_players**: Get players roster
- **get_seasonal_games**: Get seasonal games schedule
- **get_seasonal_standings**: Get seasonal standings for a league
- **get_team_stats_totals**: Get seasonal team stats totals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MySportsFeeds** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the seasonal standings for the MLB 2023-regular season."

**🤖 AI Agent:**
> I've retrieved the MLB 2023-regular standings. The AL East is led by the Baltimore Orioles (101-61) followed by the Tampa Bay Rays (99-63). Would you like to see the full division breakdown?

---

**👤 You:**
> "Show me the play-by-play for the NBA game with ID 60234 in the 2023-2024-regular season."

**🤖 AI Agent:**
> Fetching play-by-play data for game 60234... The game started with a jump ball won by the home team. Notable events include a 3-pointer by Curry at 10:42 in the 1st. Should I summarize the scoring runs?

---

**👤 You:**
> "What are the latest player injuries in the NHL?"

**🤖 AI Agent:**
> I've scanned the latest NHL injury reports. Current notable injuries include Connor McDavid (Upper Body, Day-to-day) and Nathan MacKinnon (Lower Body, Out 2 weeks). Would you like the full list for a specific team?


## ❓ FAQ

**Q: Can I get cumulative player stats for a whole season?**
Yes! Use the `get_player_stats_totals` tool. Provide the league (e.g., 'NBA') and season identifier (e.g., '2023-2024-regular') to receive a comprehensive list of player performance metrics.

**Q: How do I see the starting lineup for a specific game?**
Use the `get_game_lineup` tool with the specific league, season, and game identifier. It will return the active rosters and starting positions for both teams involved.

**Q: Is it possible to track player injuries across a league?**
Absolutely. Use the `get_player_injuries` tool to fetch the most recent injury reports for any supported league like NFL, MLB, or NHL.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mysportsfeeds](https://vinkius.com/mcp/mysportsfeeds)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MySportsFeeds** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mysportsfeeds` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MySportsFeeds** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mysportsfeeds": {
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
