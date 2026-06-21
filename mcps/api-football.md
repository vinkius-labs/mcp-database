# API-Football MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/api-football)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/api-football-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/api-football-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Comprehensive football data platform — get live scores, standings, and player stats via AI.

## Description
Empower your AI agent to orchestrate your football tracking and fan engagement with **API-Football**, the premier API for global football data. By connecting API-Football to your agent, you transform complex fixture auditing, live score monitoring, and player statistical analysis into a natural conversation. Your agent can instantly retrieve real-time results for over 1,000 leagues, access detailed standings, and even perform head-to-head comparisons between teams without you ever needing to navigate multiple sports apps or websites. Whether you are conducting a seasonal performance audit or coordinating real-time match alerts, your agent acts as a real-time sports data coordinator, providing accurate results from a single, authorized source.

### What you can do

- **Live Orchestration** — Retrieve real-time scores and match status for thousands of games across the globe.
- **Standings Auditing** — Access comprehensive league tables and team rankings for major global competitions.
- **Fixture Management** — Retrieve scheduled matches and fixture lists for specific dates and leagues.
- **Deep Metadata** — Access detailed profile data for teams and players, including performance stats.
- **H2H Comparison** — Perform historical head-to-head audits between any two teams to gauge competitive history.

### How it works

1. Subscribe to this server
2. Enter your API-Football (API-SPORTS) Key
3. Start managing your football data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Football Analysts & Fans** — automate the gathering of match results and league trends through natural language.
- **Fantasy League Managers** — monitor player statistics and team performance directly from your workspace.
- **Developers** — integrate professional-grade football APIs into your AI-driven daily routines.
- **API-Sports Power Users** — integrate your existing sports data projects into your AI-driven daily routines.


## Available Tools
- **get_fixtures**: List match fixtures
- **get_league_topscorers**: Get top scorers
- **get_player_info**: Get player statistics
- **get_standings**: Get league standings
- **get_team_info**: Get team details
- **list_leagues**: List football leagues
- **list_live_fixtures**: Get live matches
- **search_football_teams**: Search for teams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **API-Football** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all live football matches in the Premier League (ID: 39)."

**🤖 AI Agent:**
> I've retrieved the live fixtures for the Premier League. Currently, 'Manchester United' is tied 1-1 with 'Chelsea' (65'). Would you like me to check the match statistics or the live standings?

---

**👤 You:**
> "Get the latest standings for the Brasileirão Serie A (ID: 71) season 2023."

**🤖 AI Agent:**
> I've retrieved the standings for Brasileirão 2023. 'Botafogo' is leading with 51 points, followed by 'Palmeiras' with 44 points. Should I show you the full top 10 or the top scorers for this league?

---

**👤 You:**
> "What is the H2H history between Flamengo (ID: 127) and Fluminense (ID: 124)?"

**🤖 AI Agent:**
> I've analyzed the H2H history between Flamengo and Fluminense. In their last 10 encounters, Flamengo has won 4 times, Fluminense 3 times, and they have drawn 3 times. The average goals per game is 2.4. Would you like to see the details of their next scheduled derby?


## Installation & Usage

To install and use the **API-Football** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/api-football](https://vinkius.com/mcp/api-football)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
