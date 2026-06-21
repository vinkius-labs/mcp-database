# BoardGameGeek MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/boardgamegeek)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Explore the world's largest board game database — search 150,000+ games, view ratings, player counts, complexity, trending titles, user collections and play logs.

## Description
Connect your **BoardGameGeek** account to any AI agent and unlock the full analytical power of the world's largest board game database.

### What you can do

- **Smart Game Search** — Find any of 150,000+ board games by name with fuzzy or exact matching, instantly retrieving BGG IDs for deep inspection
- **Deep Game Intelligence** — Fetch comprehensive metadata for any game: year published, player count range, play time, complexity weight, Bayesian rating, user rating, global rank, description and artwork
- **Trending Discovery** — See what's hot right now across board games, RPGs, video games, and industry people
- **User Collections** — Browse any player's full collection with personal ratings, play counts, wishlist and want-to-play status
- **Play History Analytics** — Analyze a user's logged play sessions filtered by date range, revealing play patterns and favorite games
- **Community Engagement** — Access game forums, read discussion threads, rules clarifications and community reviews
- **Guild Exploration** — Discover BGG guilds, their members and community organizing around shared tabletop interests

### How it works

1. Subscribe to this server
2. No API key needed — BoardGameGeek's API is fully open
3. Start exploring board game data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Board Gamers** — discover new games, compare ratings/complexity, and explore curated collections from veteran players
- **Game Designers & Publishers** — research market positioning, competitive analysis, and community reception for similar titles
- **Content Creators & Reviewers** — gather structured data for videos, articles and podcasts without manually browsing dozens of pages
- **Event Organizers & Café Owners** — find games filtered by player count and duration to curate the perfect game night lineup


## Available Tools
- **get_forum_list**: g. Reviews, Rules, General, Strategy) associated with a specific board game by its BGG ID. Use the returned forum IDs to browse individual threads.

List discussion forums for a board game
- **get_game_plays**: Returns who played, when, and any comments. Useful for gauging a game's active community and recent engagement.

Get recent play logs for a specific board game
- **get_guild**: Guilds are community groups on BGG organized around shared interests.

Get details about a BoardGameGeek guild
- **get_hot_items**: Defaults to "boardgame" type but also supports "rpg", "videogame", "boardgameperson", "boardgamecompany". Ideal for discovering what is popular in the hobby right now.

Get the current trending/hot board games on BoardGameGeek
- **get_thing**: Returns game names, year published, min/max players, playing time, complexity weight, Bayesian/user ratings, rank, description and thumbnail. Use comma-separated IDs for multiple games.

Get detailed info for a board game by BGG ID
- **get_thread**: Useful for reading discussions, rules clarifications, or reviews about a game.

Read a specific forum thread on BoardGameGeek
- **get_user_collection**: Returns all games owned with stats, ratings, play counts, own/want/wishlist status. Optionally filter by subtype or exclude expansions.

Get a BGG user's board game collection
- **get_user_info**: Useful for understanding a user's preferences and social connections on the platform.

Get a BoardGameGeek user profile
- **get_user_plays**: Returns game names, play dates, locations, quantities and comments. Optionally filter by date range using YYYY-MM-DD format.

Get a user's board game play history
- **search_games**: Returns matching games with their BGG IDs, primary names, year published. Use the returned ID with get_thing to fetch full details including ratings, player count and complexity.

Search for board games by name on BoardGameGeek


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BoardGameGeek** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for Catan and show me its full details."

**🤖 AI Agent:**
> Found Catan (ID: 13, 1995) — 3-4 players, 60-120 min, complexity 2.29/5, rating 7.0/10, ranked #402 globally. "In Catan, players try to be the dominant force on the island by building settlements, cities, and roads..."

---

**👤 You:**
> "What board games are trending on BGG right now?"

**🤖 AI Agent:**
> The top 5 hot board games right now are: 1. Ark Nova: Marine Worlds (ID: 416584), 2. Terraforming Mars: Ares Expedition (ID: 328871), 3. Dune: Imperium — Uprising (ID: 397598), 4. Cascadia: Landmarks (ID: 414920), 5. Great Western Trail (ID: 341169). Want full details on any of these?

---

**👤 You:**
> "Show me tomvasel's board game collection and his top-rated games."

**🤖 AI Agent:**
> tomvasel's collection contains 500+ board games. Top-rated titles: Gloomhaven (10/10), Terraforming Mars (9/10), Wingspan (9/10), Scythe (9/10), Pandemic Legacy: Season 1 (9/10). Full collection with personal ratings and play counts available.


## ❓ FAQ

**Q: How do I find a game's BGG ID to get full details?**
Use the `search_games` tool with the game's name. The results include the BGG ID for each match. Then pass that ID to `get_thing` for complete metadata including ratings, player count, complexity weight and description.

**Q: Can I see what board games are currently trending?**
Absolutely! Use the `get_hot_items` tool. By default it returns the 50 hottest board games, but you can also check trending RPGs, video games, or even industry people by specifying the type parameter.

**Q: Does this integration allow modifying data on BoardGameGeek?**
No. All tools are strictly read-only queries. You can search, explore collections, read forums and analyze play history, but no data on BoardGameGeek will be created, modified or deleted through this integration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/boardgamegeek](https://vinkius.com/mcp/boardgamegeek)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BoardGameGeek** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `boardgamegeek` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BoardGameGeek** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "boardgamegeek": {
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
