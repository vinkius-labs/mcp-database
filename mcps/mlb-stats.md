# MLB Stats MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mlb-stats)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time MLB data, player stats, game schedules, and live feeds directly from your AI agent.

## Description
Connect the **MLB Stats** server to your AI agent to access the most comprehensive database of Major League Baseball information available. From real-time play-by-play to deep historical player statistics, your AI can now act as a professional sabermetrician or a real-time scoreboard.

### What you can do

- **Live Game Tracking** — Use `get_live_game_feed` to retrieve real-time play-by-play, boxscores, and game status updates.
- **Player Deep-Dives** — Access detailed profiles with `get_person` and comprehensive hitting, pitching, or fielding statistics with `get_stats`.
- **League Structure** — Query `list_teams`, `list_leagues`, and `list_divisions` to understand the organizational hierarchy of professional baseball.
- **Schedules & Results** — Plan your viewing or analyze past performances using `get_schedule` for any specific date or range.
- **Standings & Rankings** — Check the current race for the postseason with `get_standings` across different leagues and divisions.

### How it works

1. Subscribe to this server
2. Enter 'PUBLIC' or your specific API identifier
3. Start analyzing MLB data in Claude, Cursor, or any MCP-compatible environment

### Who is this for?

- **Sports Analysts** — Quickly pull specific player stats or team comparisons for articles or research.
- **Fantasy Baseball Players** — Get real-time updates and deep statistical trends to manage your roster.
- **Developers** — Integrate professional sports data into your coding environment for testing or hobby projects.


## Available Tools
- **list_divisions**: List all divisions
- **list_game_status**: g., Final, In Progress).

List valid game state codes
- **list_leagues**: List all leagues
- **get_live_game_feed**: Retrieve real-time game data, play-by-play, and boxscores
- **get_person**: Use hydrate to include extra data like stats or currentTeam.

Retrieve detailed information about a specific player
- **list_positions**: List player position codes
- **get_schedule**: Retrieve game schedules and basic game information
- **list_sports**: List all sports (MLB, MiLB levels)
- **get_standings**: Can be filtered by league, season, and standings type.

Retrieve current or historical league standings
- **list_stat_types**: List valid strings for the stats parameter
- **get_stats**: Retrieve statistical data for players or teams
- **list_teams**: Can be filtered by sport, season, league, or specific team ID.

Retrieve information about MLB teams and their affiliates
- **list_venues**: List information about ballparks/venues


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MLB Stats** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all MLB teams and their IDs for the current season."

**🤖 AI Agent:**
> I've retrieved the team list. Some examples include the Arizona Diamondbacks (ID: 109), Atlanta Braves (ID: 144), and Baltimore Orioles (ID: 110). Would you like to see the full list or details for a specific team?

---

**👤 You:**
> "Show me the American League East standings for 2023."

**🤖 AI Agent:**
> Fetching 2023 AL East standings... The Baltimore Orioles finished first with 101 wins, followed by the Tampa Bay Rays with 99 wins. Would you like the full breakdown including wild card status?

---

**👤 You:**
> "Get the hitting stats for Shohei Ohtani (ID 660271) for the 2023 season."

**🤖 AI Agent:**
> In 2023, Shohei Ohtani had a .304 batting average, 44 home runs, and 95 RBIs over 135 games. He also posted a 1.066 OPS. Would you like to see his pitching stats for the same year?


## ❓ FAQ

**Q: How can I get the play-by-play data for a game currently in progress?**
Use the `get_live_game_feed` tool with the specific `gamePk` (game ID). This provides the most detailed real-time feed, including play-by-play and boxscores.

**Q: Can I retrieve historical statistics for a specific season?**
Yes! The `get_stats` and `get_standings` tools both accept a `season` parameter (e.g., 2023) to filter data for that specific year.

**Q: How do I find the schedule for a specific team?**
You can use `get_schedule` with a date range. While the schedule tool returns all games, you can ask your AI agent to filter the results for a specific team name or ID found via `list_teams`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mlb-stats](https://vinkius.com/mcp/mlb-stats)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MLB Stats** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mlb-stats` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MLB Stats** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mlb-stats": {
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
