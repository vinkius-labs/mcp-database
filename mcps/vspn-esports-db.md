# VSPN Esports DB MCP Server

Automate esports intelligence via VSPN — fetch live tournament brackets, deep player telemetry, and team rosters directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/vspn-esports-db)

## Overview
**Category:** data-analytics
**Tools Count:** 10

## Description
Connect your intelligent agents directly to **VSPN**, Asia's premier esports tournament operator and broadcaster running major leagues across Honor of Kings, Peacekeeper Elite, and League of Legends.

### What you can do

- **Tournament Tracking** — Fetch upcoming schedules, live brackets, group stage standings, and playoff trees dynamically
- **Match Analysis** — Retrieve detailed round-by-round scorecards including map victories, team compositions, and MVP selections
- **Team Rosters** — Monitor active lineups, substitute players, and seasonal transfer movements across all sponsored teams
- **Player Telemetry** — Audit individual KDA ratios, damage output, and objective contributions extracted directly from game telemetry feeds

### How it works

1. Register on the [VSPN Developer Portal](https://www.vspn.com/)
2. Request API access and obtain your **Bearer Token** from the developer dashboard
3. Paste the token below — your agent will authenticate automatically against the VSPN REST endpoints

Stop manually refreshing league standings pages. Your AI now monitors tournament progression in real-time, summarizing match results and roster changes directly into your workflow.

### Who is this for?

- **Fantasy Esports Operators** — calculate custom scoring models pulling raw VSPN engine stats without manual data entry
- **Broadcast Production Teams** — generate real-time stats overlays and pre-match analysis packages via autonomous agents
- **Esports Journalists** — compile post-match summaries with accurate KDA and team performance data instantly


## Available Tools
- **get_match_detail**: Retrieve comprehensive data on a single match
- **get_match_stream**: Get live streaming URLs for a match
- **get_matches**: List matches within a tournament
- **getPlayerStats**: Retrieve individual player tournament stats
- **get_players**: List rostered players on a team
- **get_standings**: Retrieve current tournament standings
- **get_team_stats**: Retrieve aggregate team statistics
- **get_teams**: Retrieve esports teams in the database
- **get_tournament_detail**: Retrieve details about a specific tournament
- **get_tournaments**: Get a list of active VSPN tournaments


## Installation & Usage

To install and use the **VSPN Esports DB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vspn-esports-db](https://vinkius.com/mcp/vspn-esports-db)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
