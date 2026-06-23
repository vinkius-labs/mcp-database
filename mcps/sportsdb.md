# SportsDB MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sportsdb)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access global sports data via AI — search teams, players, and events, track scores, league tables, and match history across 200+ leagues.

## Description
Connect **SportsDB** (sportdb.dev) to your AI agent for comprehensive sports intelligence across hundreds of leagues worldwide.

### What you can do

- **Team & Player Search** — Find teams and players by name across all sports and leagues
- **Event Search** — Search for matches and events by name or keyword
- **League Navigation** — Browse all sports, leagues, and countries in the database
- **Match Tracking** — Check upcoming fixtures and recent results for any team or league
- **League Tables** — Access current standings with points, goals, and form data
- **Team & Player Profiles** — Detailed info including badges, venues, and career stats

### How it works

1. Subscribe to this server
2. Get a free API key from [sportdb.dev](https://sportdb.dev)
3. Start querying sports data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sports Fans** — get instant match scores, standings, and player stats
- **Sports Journalists** — research team histories and match data quickly
- **Fantasy Sports Players** — analyze player and team performance data for better picks


## Available Tools (12)
- **get_last_events**: Get last results for a team
- **get_league_details**: Get detailed information about a league
- **get_league_table**: Get league standings/table
- **get_next_events**: Get upcoming events for a team
- **get_player_details**: Get detailed information about a player
- **get_team_details**: Get detailed information about a team
- **list_all_countries**: List all countries with sports data
- **list_all_leagues**: List all available leagues
- **list_all_sports**: List all available sports
- **search_events**: Search for sports events by name
- **search_players**: Returns player metadata including team and nationality.

Search for players by name
- **search_teams**: Returns team metadata including ID, sport, league, and country.

Search for sports teams by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SportsDB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the current Premier League standings."

**🤖 AI Agent:**
> Here are the current Premier League standings: 1st Arsenal (78 pts), 2nd Man City (74 pts), 3rd Liverpool (72 pts). Arsenal have won 8 of their last 10 matches. Want to see upcoming fixtures?


## ❓ FAQ

**Q: What sports are supported?**
SportsDB covers 200+ leagues across football (soccer), basketball, baseball, American football, ice hockey, motorsport, tennis, rugby, cricket, and many more.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sportsdb](https://vinkius.com/mcp/sportsdb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SportsDB** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sportsdb` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SportsDB** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sportsdb": {
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
