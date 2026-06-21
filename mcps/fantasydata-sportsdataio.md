# FantasyData (SportsDataIO) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fantasydata-sportsdataio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time sports data via FantasyData (SportsDataIO) — track players, scores, and schedules for NFL, NBA, and MLB.

## Description
Connect your **FantasyData (SportsDataIO)** account to any AI agent and take full control of your sports data analysis through natural conversation.

### What you can do

- **NFL, NBA & MLB Player Intelligence** — List all active players and fetch detailed profiles, positions, and statuses across major leagues
- **Real-Time Score Tracking** — Query live scores and game results for specific dates to stay updated on every match
- **Schedule Navigation** — Retrieve full schedules for upcoming seasons to plan your fantasy roster or betting strategies flawlessly
- **Detailed Player Context** — Resolve specific player IDs to get deep-dive metadata and performance background
- **Multi-Sport Coverage** — Unified access to football, basketball, and baseball data from a single integration

### How it works

1. Subscribe to this server
2. Enter your SportsDataIO (FantasyData) API Key
3. Start querying sports stats from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fantasy Sports Players** — quickly research player status and upcoming match schedules without leaving your chat
- **Sports Analysts** — pull historical scores and player data through simple natural language questions
- **Betting Enthusiasts** — monitor real-time scores and team availability directly within your AI-powered workflow


## Available Tools (12)
- **get_mlb_player_details**: Get details for a specific MLB player
- **get_mlb_schedule**: Get the MLB schedule for a specific season
- **get_mlb_scores**: Get MLB scores for a specific date
- **get_nba_player_details**: Get details for a specific NBA player
- **get_nba_schedule**: Get the NBA schedule for a specific season
- **get_nba_scores**: Get NBA scores for a specific date
- **get_nfl_player_details**: Get details for a specific NFL player
- **get_nfl_schedule**: Get the NFL schedule for a specific season
- **get_nfl_scores**: Get NFL scores for a specific date
- **list_mlb_players**: List all active MLB players
- **list_nba_players**: List all active NBA players
- **list_nfl_players**: List all active NFL players


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FantasyData (SportsDataIO)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active NFL players."

**🤖 AI Agent:**
> I've retrieved the NFL player roster. You have over 2,000 active players including 'Patrick Mahomes' (QB, ID: 18877) and 'Justin Jefferson' (WR, ID: 21685). Which team or position should I filter by?

---

**👤 You:**
> "Show me the NBA scores for last night."

**🤖 AI Agent:**
> Fetching NBA scores for 2024-04-03... The Lakers beat the Celtics 112-105, and the Warriors won against the Mavericks 120-118. Would you like the box score for any of these games?

---

**👤 You:**
> "Get the MLB schedule for the 2024 season."

**🤖 AI Agent:**
> Retrieving 2024 MLB schedule... The regular season consists of 2,430 games starting from March 28th. Opening day featured match-ups like Yankees vs Astros and Dodgers vs Cardinals.


## ❓ FAQ

**Q: How do I obtain a SportsDataIO (FantasyData) API Key?**
You can sign up for a free trial or a paid plan at [**sportsdata.io**](https://sportsdata.io/developers). Once registered, you can find your API key in the developer portal dashboard.

**Q: Does this support live scores during games?**
Yes! The `get_scores` tools for NFL, NBA, and MLB retrieve the most recent game data available for the specified date, including live updates if supported by your API plan.

**Q: Can I search for players in multiple sports?**
Absolutely. This integration provides dedicated tools for NFL, NBA, and MLB player directories, allowing you to query rosters across all three major sports.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fantasydata-sportsdataio](https://vinkius.com/mcp/fantasydata-sportsdataio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FantasyData (SportsDataIO)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fantasydata-sportsdataio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FantasyData (SportsDataIO)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fantasydata-sportsdataio": {
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
