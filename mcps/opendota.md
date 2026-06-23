# OpenDota MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opendota)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Explore Dota 2 match data, player stats, heroes, teams and leagues — no API key required for basic access.

## Description
Connect to **OpenDota** and explore the world's most comprehensive Dota 2 match database through natural conversation.

### What you can do

- **Player Profiles** — Get player stats, rank tier, MMR estimate, winrate and most played heroes
- **Match History** — Browse a player's full match history with hero, result, KDA and duration
- **Match Details** — Get complete match info including all 10 players, items, builds, damage and objectives
- **Heroes** — List all 124 Dota 2 heroes with their roles, attributes and performance benchmarks
- **Teams** — Discover professional teams with their ratings, rosters and win/loss records
- **Leagues** — Browse all pro leagues and tournaments with tiers and dates
- **Records** — See all-time records for kills, GPM, XPM, hero damage and more
- **MMR Distribution** — View rank tier distribution across the entire Dota 2 player base
- **Search** — Find players, teams and leagues by name

### How it works

1. Subscribe to this server
2. No API key needed for basic access (60k requests/hour)
3. Explore Dota 2 data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Players** — review match history, analyze hero performance and compare stats
- **Analysts** — explore team records, league data and player benchmarks
- **Fans** — discover pro teams, check tournament results and search for favorite players
- **Researchers** — access MMR distributions, game mode data and match statistics


## Available Tools (18)
- **get_benchmarks**: Compare any player's stats against the broader player base. Requires a hero ID (from list_heroes).

Get hero performance benchmarks
- **get_constants**: Optionally specify a resource name (e.g. "game_mode", "lobby_type", "lane_role", "patch", "cluster") to get a specific constant set.

Get OpenDota constant data
- **get_distributions**: Shows how many players are in each bracket (Herald, Guardian, Crusader, Archon, Legend, Ancient, Divine, Immortal). Useful for understanding where a player stands in the overall population.

Get MMR and rank distributions
- **run_explorer_query**: Requires a valid SQL query string. Returns query results as an array. Advanced feature for deep data analysis. Example: "SELECT hero_id, count(*) matches FROM player_matches GROUP BY hero_id ORDER BY matches DESC LIMIT 10"

Run a custom SQL query via OpenDota Explorer
- **get_match**: Returns the match duration, game mode, lobby type, league, radiant/dire team compositions, all 10 players' heroes, items, KDA, GPM, XPM, hero damage, tower damage and healing. Also includes draft picks, chat logs and team objectives for professional matches.

Get detailed match info
- **get_player**: Returns the player's profile picture, rank tier, MMR estimate, total matches, winrate and country. Account IDs are numeric Steam IDs (e.g. 87276347 for Arteezy, 19672354 for SumaiL). Use search to find a player by name first.

Get player profile and stats
- **get_player_heroes**: Useful for analyzing a player's hero pool and identifying their best heroes.

Get a player's performance stats by hero
- **get_player_matches**: Each match includes the match ID, hero played, result (win/loss), kills, deaths, assists, duration, game mode, lobby type, league and start time. Sorted by most recent first. Returns thousands of matches for active players.

Get a player's match history
- **get_player_recent_matches**: Each match includes the match ID, hero played, result, KDA, duration and game mode. Useful for checking a player's current form and recent hero pool.

Get a player's recent matches (last 20)
- **get_player_records**: Shows the match ID, hero and value for each record.

Get a player's personal records
- **get_player_wl**: Shows wins and losses for each hero, revealing their strongest and weakest picks. Useful for understanding a player's hero preferences and strengths.

Get a player's win/loss record by hero
- **get_records**: Supported fields: "kills", "deaths", "assists", "last_hits", "denies", "gold_per_min", "xp_per_min", "hero_damage", "tower_damage", "hero_healing", "level", "duration", "longest_word". Returns the top record holders with match IDs and hero info.

Get all-time game records
- **get_team**: Returns the team name, tag, logo, rating, win/loss record, player roster, matches played and recent results.

Get detailed info for a professional team
- **list_heroes**: Returns approximately 124 heroes. Useful for discovering hero IDs to use with other tools.

Get the list of all Dota 2 heroes
- **list_leagues**: Each league includes its ID, name, tier (premium, professional, amateur), region, start/end dates and logo URL. Useful for discovering tournaments and filtering matches by league.

Get the list of professional leagues
- **list_recent_matches**: Each match includes the match ID, start time, duration, radiant/dire team average MMR and winner. Returns up to 500 matches. Useful for browsing recent games and finding match IDs to explore.

Get recent public matches
- **list_teams**: Each team includes its ID, name, tag, logo URL, rating, number of wins/losses and last match time. Sorted by team rating. Useful for discovering pro teams and their IDs.

Get the list of professional teams
- **search**: Returns matching results with their types and IDs. Useful for finding a player's account ID or a team's ID when you only know their name.

Search for players, teams, leagues and heroes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenDota** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the player 'Arteezy'."

**🤖 AI Agent:**
> Found Arteezy (account ID: 87276347). Real name: Artour Babaev. Country: Canada. Current rank: Immortal. Profile picture and full stats available. Use get_player for detailed profile or get_player_recent_matches for recent games.

---

**👤 You:**
> "Show me all Dota 2 heroes."

**🤖 AI Agent:**
> Found 124 heroes. Notable heroes include: Anti-Mage (agi, carry), Invoker (int, mid), Pudge (str, offlane), Phantom Assassin (agi, carry), Crystal Maiden (int, support), Axe (str, offlane) and 118 more. Each with primary attribute, attack type and role classifications.

---

**👤 You:**
> "What are the all-time records for most kills in a single match?"

**🤖 AI Agent:**
> All-time kill record: 75 kills in a single match by a player on Morphling. Other top records include 70 kills (Phantom Assassin), 65 kills (Medusa) and 60 kills (Juggernaut). These are from public matches tracked by OpenDota.


## ❓ FAQ

**Q: Do I need an API key?**
No! OpenDota provides free access with 60,000 requests/hour without any API key. An optional free API key is available from opendota.com for higher rate limits, but it's not required.

**Q: How do I find a player's account ID?**
Use the search tool with the player's name (e.g. 'Arteezy', 'SumaiL', 'Topson'). The results include their Steam account ID which you can then use with player-specific tools. You can also find account IDs on sites like dotabuff.com or stratz.com.

**Q: What data is available for matches?**
Match data includes: all 10 players' heroes, items, KDA, GPM, XPM, hero damage, tower damage, healing, lane positions, draft picks, chat logs, team objectives, ability builds and more. Professional matches have even more detailed data including observer ward placements and rune pickups.

**Q: How many heroes are in Dota 2?**
Dota 2 currently has 124 heroes, each with unique abilities and roles. Use list_heroes to see the complete list with their IDs, names, primary attributes (Strength, Agility, Intelligence, Universal) and roles (carry, support, offlane, mid).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opendota](https://vinkius.com/mcp/opendota)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenDota** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `opendota` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenDota** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opendota": {
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
