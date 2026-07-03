# BallDontLie MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/balldontlie)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

NBA data platform — access player stats, team info, and game results via AI.

## Description
Equip your AI agent with the most accessible NBA intelligence via **BallDontLie**. This unified server provides your agent with instant access to extensive basketball data, including player profiles, team technical details, and historical game results. Your agent can search for specific players, audit team rosters, and retrieve real-time or historical statistics without you ever manually checking a sports site. Whether you are analyzing season averages or tracking live game scores, your agent acts as a dedicated sports data analyst through natural conversation.

### What you can do

- **Player Intelligence** — Search for thousands of active and retired NBA players and retrieve their detailed metadata.
- **Team Auditing** — Fetch technical details and identifiers for all 30 NBA teams.
- **Game Tracking** — Retrieve lists of games with scores and specific results, filtered by date or season.
- **Statistical Analysis** — Access player statistics for specific games and calculate season averages for deep performance auditing.
- **Comprehensive Metadata** — List and inspect technical identifiers for teams and players to build complex sports workflows.

### How it works

1. Subscribe to this server
2. Enter your BallDontLie API Key
3. Start managing your NBA intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sports Analysts & Fans** — instantly retrieve exact player stats and game results through natural language.
- **Fantasy Basketball Players** — audit player performance and season averages to optimize their roster decisions.
- **Data Scientists** — integrate clean NBA technical data into analysis models and visualizations.
- **Developers** — build sports-centric applications with a reliable and easy-to-use NBA data source.
- **Content Creators** — retrieve historical game data and player metadata for sports commentary and media production.


## Available Tools (8)
- **get_player_details**: Get player details
- **get_team_details**: Get team details
- **list_games**: List NBA games
- **list_players**: List or search NBA players
- **list_player_stats**: List player statistics
- **list_teams**: List all NBA teams
- **get_season_averages**: Get season averages
- **get_game_details**: Get game details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BallDontLie** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are LeBron James's career stats on BallDontLie?"

**🤖 AI Agent:**
> Searching for LeBron James... I've found his profile (ID: 237). He plays for the Los Angeles Lakers. I can now pull his season averages or specific game stats for you.

---

**👤 You:**
> "Show me the scores for NBA games yesterday."

**🤖 AI Agent:**
> Retrieving game results for yesterday... There were 5 games played. Notable results include the Warriors beating the Suns 115-110 and the Celtics winning over the Bucks 120-105.

---

**👤 You:**
> "Get the season averages for player ID 237 in 2023."

**🤖 AI Agent:**
> Fetching 2023 season averages for player 237... In that season, they averaged 25.7 points, 7.3 rebounds, and 8.3 assists per game across 71 games played.


## ❓ FAQ

**Q: Can I search for a specific player by name?**
Yes! Use the `list_players` tool and provide the name in the `search` parameter. Your agent will return a list of matching players with their unique IDs and metadata.

**Q: How do I see the scores for all games played on a specific date?**
Use the `list_games` tool and provide the date in the `dates` parameter (format YYYY-MM-DD). The response will include all games played on that day with their final scores.

**Q: Does the integration provide player season averages?**
Absolutely. Use the `get_season_averages` tool by providing the specific season year and the player IDs. This will return averaged performance metrics for the requested period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/balldontlie](https://vinkius.com/mcp/balldontlie)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BallDontLie** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `balldontlie` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BallDontLie** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "balldontlie": {
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
