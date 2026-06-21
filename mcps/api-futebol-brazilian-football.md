# API-Futebol (Brazilian Football) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/api-futebol-brazilian-football)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/api-futebol-brazilian-football-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/api-futebol-brazilian-football-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

The definitive server for Brazilian football — track Brasileirão, Copa do Brasil, and State Leagues via AI.

## Description
Equip your AI agent with the most comprehensive intelligence on Brazilian football via **API-Futebol**. This unified server provides unprecedented access to the heart of South American soccer, allowing your agent to instantly retrieve real-time live scores, detailed championship standings, official match lineups, and full tournament brackets. From the elite Brasileirão Série A to local State Championships, your agent acts as a dedicated Brazilian football scout and analyst, providing precise metadata and tactical insights through natural conversation.

### What you can do

- **Championship Auditing** — List and query standings for Brasileirão (Série A, B, C, D), Copa do Brasil, and all major State Leagues
- **Real-time Match Ticker** — Retrieve live scores, goal notifications, and match status for all games currently occurring in Brazil
- **Historical & Future Fixtures** — Fetch complete match histories and upcoming schedules for any professional Brazilian club
- **Statistical Deep-Dives** — Audit top scorer leaderboards, team-specific performance, and tournament phases with precision

### How it works

1. Subscribe to this server
2. Enter your API-Futebol Token from the [**Developer Portal**](https://api-futebol.com.br/)
3. Start managing your Brazilian football intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sports Journalists** — instantly retrieve lineups and historical data for technical reporting and match previews
- **Fantasy Football Enthusiasts** — monitor player performance and team standings directly from your workflow
- **Professional Fans** — track your favorite team's journey through State Leagues and National Cups with micro-metric accuracy


## Available Tools
- **get_cup_brackets**: Get the phases and brackets for a cup competition
- **list_championships**: List all available football championships in Brazil
- **get_live_matches**: Get real-time scores for matches currently in-play
- **get_match_details**: Get full details for a specific match ID
- **list_championship_matches**: List all matches for a specific championship
- **get_round_details**: Get details and results for a specific championship round
- **list_championship_rounds**: List all rounds for a specific championship
- **list_top_scorers**: Get the leading goal scorers for a championship
- **get_championship_standings**: Get the points table for a specific championship
- **get_api_status**: Check the API status and quota usage
- **get_team_matches**: Get the match history and schedule for a specific team
- **search_teams**: Search for Brazilian football clubs by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **API-Futebol (Brazilian Football)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the current standings for the Brasileirão Série A."

**🤖 AI Agent:**
> I've retrieved the Série A standings. Currently, Palmeiras is leading with 62 points, followed closely by Botafogo. Would you like to see the full table including the relegation zone?

---

**👤 You:**
> "Which Brazilian football matches are happening live right now?"

**🤖 AI Agent:**
> Running the live query... I found 3 active matches. In the Brasileirão, Corinthians is drawing 1-1 with São Paulo (75'). I also found two State League matches. Would you like the live lineups for the Corinthians game?

---

**👤 You:**
> "Get the top scorers list for the latest Copa do Brasil."

**🤖 AI Agent:**
> Inspecting the scoring charts... I've retrieved the top scorers for the Copa do Brasil. Currently, the leader is 'Player Name' with 7 goals. I have the full list of the top 10. Shall I provide their club details as well?


## Installation & Usage

To install and use the **API-Futebol (Brazilian Football)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/api-futebol-brazilian-football](https://vinkius.com/mcp/api-futebol-brazilian-football)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
