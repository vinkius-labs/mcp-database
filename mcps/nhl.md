# NHL MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nhl)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time NHL scores, schedules, standings, and player statistics directly from your AI agent.

## Description
Connect your AI agent to the pulse of the **National Hockey League**. This server provides comprehensive access to NHL data, from live game scores and play-by-play updates to historical player stats and team rosters.

### What you can do

- **Live Scores & Schedules** — Get real-time updates on active games and check upcoming schedules for any date or specific team.
- **Team Standings** — Retrieve current and seasonal standings to track the race for the Stanley Cup.
- **Player Profiles & Search** — Search for any player to get detailed biographical info and career stats.
- **Advanced Skater Stats** — Access deep metrics including powerplay performance, realtime stats, and seasonal summaries.
- **Game Analysis** — Inspect full boxscores and play-by-play data for specific game IDs to understand every goal and penalty.

### How it works

1. Subscribe to this server
2. Enter 'PUBLIC' as your access token
3. Start querying hockey data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sports Analysts** — quickly pull seasonal stats and skater summaries for deep-dive reporting.
- **Fantasy Hockey Players** — check rosters, injuries, and live performance metrics to manage your lineup.
- **Developers** — integrate live sports data into your workflow or build hockey-themed tools with ease.


## Available Tools
- **get_awards**: Get NHL awards
- **get_conferences**: Get NHL conferences
- **get_current_schedule**: Get the NHL schedule for the current day
- **get_current_standings**: Get current NHL standings
- **get_divisions**: Get NHL divisions
- **get_franchises**: Get NHL franchises
- **get_game_boxscore**: Get the boxscore for a specific game
- **get_game_play_by_play**: Get play-by-play data for a specific game
- **get_goalie_advanced**: Get goalie advanced stats
- **get_goalie_saves_by_strength**: Get goalie saves by strength stats
- **get_goalie_summary**: Get goalie summary stats
- **get_legacy_draft**: Get NHL draft data
- **get_legacy_game_boxscore**: Get legacy boxscore for a game
- **get_legacy_game_content**: Get media and highlights for a game
- **get_legacy_game_linescore**: Get legacy linescore for a game
- **get_legacy_game_live_feed**: Get comprehensive play-by-play, coordinates, and player stats for a game
- **get_legacy_player_info**: Get legacy player info
- **get_legacy_player_stats**: Get legacy player stats
- **get_live_scores**: Get live NHL scores
- **get_player_landing**: Get specific stats and biographical info for a player
- **get_records_attendance**: Get NHL records attendance
- **get_records_franchise_season_records**: Get NHL records franchise season records
- **get_records_franchise_team_totals**: Get NHL records franchise team totals
- **get_records_franchises**: Get NHL records franchises
- **get_records_milestone_1000_point**: Get NHL records 1000 point career milestones
- **get_records_milestone_500_goal**: Get NHL records 500 goal career milestones
- **get_records_milestone_50_goal**: Get NHL records 50 goal season milestones
- **get_records_officials**: Get NHL records officials
- **get_records_trophies**: Get NHL records trophies
- **get_roster_seasons**: Get available roster seasons for a team
- **get_schedule_by_date**: Get the NHL schedule for a specific date
- **get_season_standings**: Get season NHL standings
- **get_skater_powerplay**: Get skater powerplay stats
- **get_skater_realtime**: Get skater realtime stats
- **get_skater_summary**: Get skater summary stats
- **get_stats_config**: Get Advanced Stats API configuration
- **get_team_faceoff_percentages**: Get team faceoff percentages stats
- **get_team_monthly_schedule**: Get the monthly schedule for a team
- **get_team_powerplay**: Get team powerplay stats
- **get_team_roster**: Get the roster for a team in a specific season
- **get_team_season_schedule**: Get all games for a team in the current season
- **get_team_summary**: Get team summary stats
- **get_team_weekly_schedule**: Get the weekly schedule for a team
- **get_venues**: Get NHL venues
- **search_player**: Search for a player by name
- **suggest_active_players**: Suggest active players by name fragment
- **suggest_players**: Suggest players by name fragment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NHL** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the NHL schedule for today?"

**🤖 AI Agent:**
> I'll check the current schedule for you. Today there are 5 games scheduled, including the Rangers vs. Bruins at 7:00 PM ET and the Oilers vs. Flames at 9:30 PM ET.

---

**👤 You:**
> "Show me the roster for the Montreal Canadiens for the 20232024 season."

**🤖 AI Agent:**
> Fetching the 2023-2024 roster for MTL... The roster includes key players like Nick Suzuki (C), Cole Caufield (LW), and Mike Matheson (D). Would you like stats for a specific player?

---

**👤 You:**
> "Search for player Connor McDavid and show his current stats."

**🤖 AI Agent:**
> Searching for Connor McDavid... Found Player ID 8478402. He currently has 132 points this season (32 goals, 100 assists) in 76 games played.


## ❓ FAQ

**Q: How can I see the live scores for games happening right now?**
Use the `get_live_scores` tool. It will return all active NHL games with their current scores, period information, and clock status.

**Q: Can I get a detailed breakdown of a specific game's performance?**
Yes! By using the `get_game_boxscore` tool with a valid Game ID, you can retrieve full team statistics, individual player contributions, and scoring summaries.

**Q: How do I find advanced statistics for skaters like powerplay goals?**
You can use the `get_skater_powerplay` or `get_skater_summary` tools to fetch specialized performance metrics across the league.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nhl](https://vinkius.com/mcp/nhl)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NHL** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nhl` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NHL** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nhl": {
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
