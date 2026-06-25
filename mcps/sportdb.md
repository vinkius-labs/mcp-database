# SportDB MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sportdb)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access live scores, standings, fixtures, and player data across football, basketball, hockey, and tennis from any AI agent.

## Description
Turn your AI agent into a dedicated sports analyst with **SportDB**. Query real-time match data, historical league tables, and deep player intelligence across multiple sports — all through natural conversation.

### What you can do

- **Live Match Tracking** — Retrieve real-time scores for football, basketball, hockey, and tennis as they happen
- **League Standings** — Fetch full league tables with points, wins, draws, losses, and goal difference for any season
- **Fixture Schedules** — Browse completed and upcoming matches for specific leagues and seasons
- **Match Deep Dive** — Inspect individual matches with lineups, formations, substitutions, and in-game statistics
- **Club Intelligence** — Search for clubs, view profiles with stadium information, and retrieve current squad rosters
- **Player Analytics** — Search players, view career profiles, seasonal statistics, and complete transfer histories

### How it works

1. Subscribe to this server
2. Enter your SportDB API Key from the [SportDB Dashboard](https://dashboard.sportdb.dev)
3. Start querying sports data from Claude, Cursor, or any MCP-compatible client

Your agent navigates the entire competition hierarchy — from country to league to season to match — so you never have to dig through sports websites manually.

### Who is this for?

- **Sports Analysts & Journalists** — instantly pull live scores, standings, and player stats to enrich reporting
- **Fantasy League Managers** — monitor player form, transfer activity, and team performance from your workspace
- **Developers & Data Engineers** — integrate professional-grade multi-sport data into AI-powered applications


## Available Tools (18)
- **get_club_players**: Requires the numeric club ID.

List all players currently registered to a specific club
- **get_live_basketball**: Use this when the user asks about ongoing basketball games or live NBA/EuroLeague results.

Get live basketball match scores happening right now
- **get_club_profile**: Requires the numeric club ID obtained from search results.

Get the full profile of a club by its ID
- **get_competition_seasons**: g., "premier-league"), returns all available seasons. Use this to find the season identifier needed for standings and fixtures queries.

List available seasons for a specific competition
- **get_country_competitions**: g., "england", "spain", "germany"), returns all competitions available in that country. The response includes competition slugs needed to drill deeper into seasons and standings.

List competitions (leagues/cups) available in a specific country for a sport
- **get_fixtures**: Includes dates, teams, scores for completed matches, and upcoming schedule. Requires sport, country_slug, competition_slug, and season.

Get scheduled and completed match fixtures for a season
- **get_match**: Use the match_id obtained from fixtures or live results.

Get detailed information for a specific match by its ID
- **get_match_lineups**: Returns player names and positions for each side.

Get starting lineups and substitutions for a specific match
- **get_match_stats**: Requires a valid match_id.

Get in-match statistics for a specific match
- **get_player_profile**: Requires the numeric player ID obtained from search results.

Get the full profile of a player by their ID
- **get_player_stats**: Requires the numeric player ID.

Get career and seasonal statistics for a specific player
- **get_player_transfers**: Requires the numeric player ID.

Get the complete transfer history of a specific player
- **get_standings**: Requires sport, country_slug, competition_slug, and season (e.g., "2024-2025"). This is the primary tool for answering "who is top of the league" questions.

Get league table standings for a specific season of a competition
- **list_countries**: The sport parameter should be a slug like "football", "basketball", "hockey", or "tennis". Use this as the starting point to navigate the competition hierarchy.

List all countries available for a given sport
- **get_live_football**: Use this when the user asks about ongoing football games, current scores, or live results.

Get live football (soccer) match scores happening right now
- **get_live_hockey**: Use this when the user asks about ongoing hockey games or live NHL/KHL results.

Get live ice hockey match scores happening right now
- **search_clubs**: Returns a list of matching clubs with their IDs and basic metadata. Use this to find a club ID before requesting its profile or player roster.

Search for clubs/teams by name keyword
- **search_players**: Returns matching players with their IDs and basic profile data. Use this to find a player ID before requesting their detailed profile, statistics, or transfer history.

Search for players by name keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SportDB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the live football scores right now."

**🤖 AI Agent:**
> I've retrieved the live matches. There are currently 4 active games: Manchester City 2–1 Arsenal (67'), Real Madrid 0–0 Atlético Madrid (32'), Flamengo 1–0 Palmeiras (55'), and Bayern Munich 3–2 Dortmund (81'). Would you like me to pull the match stats for any of these?

---

**👤 You:**
> "Search for Erling Haaland and show me his transfer history."

**🤖 AI Agent:**
> Found Erling Haaland (ID: 48291). Here is his transfer history: Bryne FK → Molde FK (Jan 2017), Molde FK → Red Bull Salzburg (Jan 2019, €5M), Red Bull Salzburg → Borussia Dortmund (Jan 2020, €20M), Borussia Dortmund → Manchester City (Jul 2022, €60M). Would you like to see his seasonal statistics?

---

**👤 You:**
> "Get the La Liga standings for the 2024-2025 season."

**🤖 AI Agent:**
> Here are the La Liga 2024-2025 standings: 1. Barcelona — 52 pts (W16 D4 L2), 2. Real Madrid — 48 pts (W15 D3 L4), 3. Atlético Madrid — 43 pts (W13 D4 L5). The table includes 20 teams with full records. Want me to pull the upcoming fixtures for any of these clubs?


## ❓ FAQ

**Q: Can my AI agent show me live football scores while I work?**
Yes! Simply ask your agent to run the `get_live_football` tool and it will instantly retrieve all ongoing matches with real-time scores, minute markers, and status updates. You can also use `get_live_basketball` or `get_live_hockey` for other sports.

**Q: How do I find the Premier League standings for the current season?**
Navigate the hierarchy: first use `list_countries` with sport 'football', then `get_country_competitions` for 'england', then `get_competition_seasons` for 'premier-league', and finally `get_standings` with the season slug. Your agent can chain these steps automatically from a simple question like 'Show me the Premier League table'.

**Q: Can the integration modify any data on SportDB, or is it strictly read-only?**
All 18 tools are strictly read-only query operations. The integration cannot create, update, or delete any data on SportDB. Your API key is used solely for authenticated reads, ensuring your account remains safe from any destructive operations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sportdb](https://vinkius.com/mcp/sportdb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SportDB** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sportdb` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SportDB** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sportdb": {
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
