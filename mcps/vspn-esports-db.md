# VSPN Esports DB MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vspn-esports-db)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/vspn-esports-db-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/vspn-esports-db-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Automate esports intelligence via VSPN — fetch live tournament brackets, deep player telemetry, and team rosters directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VSPN Esports DB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the current team standings for the KPL Spring 2024 group stage."

**🤖 AI Agent:**
> Group Stage standings retrieved! Team Wolves leads Group A with 12 points (4W-0L), followed closely by eStar Pro at 9 points (3W-1L). Group B is tighter with QGhappy and Hero Jiuyue tied at 6 points each. Would you like me to pull the upcoming match schedule for the next round?

---

**👤 You:**
> "Show me the full match telemetry for match ID KPL-2024-0412."

**🤖 AI Agent:**
> Match KPL-2024-0412 telemetry loaded! Team Wolves vs. eStar Pro — final score 3-1. Game 1: Wolves won with a 12K gold lead at 18 minutes. MVP: Player 'FlyCat' with KDA 7/1/9. Game 2: eStar Pro bounced back winning a 35-minute macro contest. Should I export the full per-player stat sheet?

---

**👤 You:**
> "List all active roster members for team 'QGhappy' with their current KDA averages."

**🤖 AI Agent:**
> QGhappy roster retrieved! 5 active players this season: 'Fly' (Mid, KDA 5.2), 'Cat' (Jungle, KDA 4.8), 'Hurt' (Clash Lane, KDA 3.9), 'Qing' (Support, KDA 7.1), and 'Xiào' (Farm Lane, KDA 4.5). Last roster change: 'Qing' promoted from substitute on March 15. Would you like a comparison against last season's performance?


## Installation & Usage

To install and use the **VSPN Esports DB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vspn-esports-db](https://vinkius.com/mcp/vspn-esports-db)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
