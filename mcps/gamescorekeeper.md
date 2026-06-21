# GameScorekeeper MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gamescorekeeper)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gamescorekeeper-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gamescorekeeper-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access live sports scores, fixtures, lineups, team form, and player statistics via AI — covering major football competitions worldwide.

## Description
Connect **GameScorekeeper** to your AI agent for real-time football (soccer) intelligence across major competitions.

### What you can do

- **Competitions** — Browse and list active competitions with detailed metadata
- **Fixtures** — Get fixture schedules, live scores, and match results
- **Lineups** — Access full match lineups with player positions and numbers
- **Team Intelligence** — View team profiles, current form, and recent results
- **Player Stats** — Access individual player statistics, career data, and performance metrics
- **Stage Navigation** — Browse competition stages (group stage, knockouts, etc.)

### How it works

1. Subscribe to this server
2. Get your GameScorekeeper API token
3. Start tracking football from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sports Analysts** — access match lineups, team form, and player stats for tactical analysis
- **Fantasy Football Players** — get player performance data directly from the AI for informed picks
- **Sports App Developers** — build football data features with natural language access


## Available Tools
- **get_competition_details**: Get detailed info for a specific tournament
- **get_fixture_lineup**: Get player lineups for a specific match
- **get_fixture_details**: Get detailed match information
- **get_player_stats**: Retrieve historical performance metrics for a player
- **get_player_details**: Get individual player profile
- **get_team_form**: Get recent performance form for a team
- **get_team_details**: Get basic information and logo for an esports team
- **list_competition_stages**: List stages (e.g., Playoffs, Group Stage) for a competition
- **list_competitions**: List all supported esports tournaments and leagues
- **list_fixtures**: List upcoming and past esports matches


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GameScorekeeper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the upcoming Champions League fixtures."

**🤖 AI Agent:**
> Here are the next 4 Champions League fixtures: Real Madrid vs Bayern Munich (Apr 30, 21:00 CET), Arsenal vs PSG (Apr 30, 21:00 CET), Barcelona vs Dortmund (May 1, 21:00 CET), Inter vs Man City (May 1, 21:00 CET). Want lineups or team form for any match?


## Installation & Usage

To install and use the **GameScorekeeper** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gamescorekeeper](https://vinkius.com/mcp/gamescorekeeper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
