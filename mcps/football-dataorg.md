# Football-Data.org MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/football-dataorg)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/football-dataorg-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/football-dataorg-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time football scores, standings, and player statistics from major global leagues via Football-Data.org.

## Description
Connect the **Football-Data.org** API to your AI agent to retrieve comprehensive football (soccer) data through natural language. Stay updated with live scores, historical results, and deep team analytics.

### What you can do

- **League Standings** — Fetch real-time tables for the Premier League, La Liga, Bundesliga, Serie A, and more using `get_competition_standings`.
- **Match Tracking** — Query upcoming fixtures or past results for specific competitions or teams with `list_competition_matches` and `list_team_matches`.
- **Top Scorers** — Identify the leading goal scorers in any supported tournament using `list_competition_scorers`.
- **Team & Player Insights** — Get detailed profiles, squad lists, and individual player performance history via `get_team` and `get_player`.
- **Global Coverage** — Explore football data across different geographical areas and continents using `list_areas`.

### How it works

1. Subscribe to this server
2. Enter your Football-Data.org API Token
3. Start asking about match results, league tables, or player stats in Claude, Cursor, or any MCP client

### Who is this for?

- **Sports Analysts** — Quickly pull raw data for match previews, post-match reports, and statistical comparisons.
- **Developers & Hobbyists** — Integrate live sports data into your workflow or build sports-aware AI assistants.
- **Football Fans** — Get instant updates on your favorite team's schedule and standing without searching through websites.


## Available Tools
- **get_area**: Get details for a specific area
- **get_competition_standings**: Can be filtered by standing type (TOTAL, HOME, AWAY).

Get standings (league table) for a competition
- **get_competition**: g., PL for Premier League).

Get details for a specific competition
- **get_match**: Get details for a specific match
- **get_player**: Get details for a specific player
- **get_team**: Get details for a specific team
- **list_areas**: List all geographical areas
- **list_competition_matches**: Can be filtered by season, status, stage, group, date range, or matchday.

List matches for a specific competition
- **list_competition_scorers**: List top scorers for a competition
- **list_competition_teams**: List teams in a specific competition
- **list_competitions**: Can be filtered by specific competition IDs or season.

List available competitions
- **list_matches**: List matches across competitions
- **list_player_matches**: List matches for a specific player
- **list_team_matches**: Can be filtered by status, venue, and date range.

List matches for a specific team


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Football-Data.org** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the current Premier League standings."

**🤖 AI Agent:**
> I've retrieved the latest Premier League standings. Manchester City is currently in 1st place with 24 points, followed by Liverpool with 22 points. Would you like to see the full table?

---

**👤 You:**
> "Who are the top scorers in the Champions League right now?"

**🤖 AI Agent:**
> In the current Champions League season, Harry Kane leads with 5 goals, followed by Raphinha and Erling Haaland with 4 goals each. Do you want details on a specific player?

---

**👤 You:**
> "What are the next 3 matches for Real Madrid?"

**🤖 AI Agent:**
> Real Madrid's upcoming matches are: 1. vs AC Milan (Champions League), 2. vs Osasuna (La Liga), and 3. vs Leganés (La Liga). Would you like the exact dates and times?


## Installation & Usage

To install and use the **Football-Data.org** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/football-dataorg](https://vinkius.com/mcp/football-dataorg)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
