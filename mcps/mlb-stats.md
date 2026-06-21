# MLB Stats MCP Server

Access real-time MLB data, player stats, game schedules, and live feeds directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mlb-stats)

## Overview
**Category:** data-analytics
**Tools Count:** 13

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


## Installation & Usage

To install and use the **MLB Stats** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mlb-stats](https://vinkius.com/mcp/mlb-stats)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
