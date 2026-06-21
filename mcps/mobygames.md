# MobyGames MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mobygames)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-management](../categories/content-management.md)

Search 100,000+ video games — find games by title, platform, genre, developer and get credits, reviews and scores.

## Description
Connect to **MobyGames** and explore the world's largest video game database through natural conversation.

### What you can do

- **Game Search** — Search 100,000+ games by title, platform, genre and developer
- **Game Details** — Get full game info including release dates, descriptions, screenshots and MobyScores
- **Platform List** — Browse all gaming platforms (consoles, PCs, mobile, arcade)
- **Developer Search** — Find game developers and studios by name
- **Company Search** — Search game publishers and companies
- **Genres** — Get complete list of game genres
- **Reviews** — Access game reviews and critic scores
- **Credits** — View full game credits (developers, artists, testers)
- **Game Groups** — Browse game series and franchises

### How it works

1. Subscribe to this server
2. Enter your MobyGames API Key (free registration)
3. Start exploring game data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Gamers** — discover games by platform, genre or developer and find credits and reviews
- **Researchers** — explore game history, developer portfolios and franchise timelines
- **Journalists** — find game information, reviews and credits for articles and reviews


## Available Tools
- **get_attributes**: g. "Educational", "Free-to-play", "Open world", "Multiplayer"). Returns attribute names and IDs.

Get game attributes/special attributes
- **get_companies**: Returns company names, game counts and profile info.

Search for game publishers and companies by name
- **get_developers**: Returns developer names, game counts and profile info.

Search for game developers by name
- **get_game_by_id**: Returns title, release dates, platforms, genres, descriptions, developers, publishers, MobyScore, screenshots, covers and credits.

Get detailed info for a specific game by MobyGames ID
- **get_game_credits**: ) for a specific game by its MobyGames ID. Returns person names, roles and departments.

Get credits for a specific game
- **get_game_group**: Returns group name, description and list of games in the group.

Get details for a specific game group (series/franchise)
- **get_game_groups**: Returns group names, game counts and descriptions.

Get list of game groups (series/franchises)
- **get_genres**: Returns genre names and IDs for filtering game searches.

Get list of all game genres
- **get_platforms**: Returns platform names and IDs for filtering game searches.

Get list of all gaming platforms
- **get_reviews**: Optionally filter by game ID. Returns review scores, reviewer names, publications and review excerpts.

Get game reviews from the MobyGames database
- **search_games**: Supports filtering by title, platform, genre and developer. Returns game titles, release years, platforms, genres, MobyScores and developer/publisher info.

Search for video games in the MobyGames database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MobyGames** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for The Legend of Zelda games."

**🤖 AI Agent:**
> Found 30+ Legend of Zelda games including: Breath of the Wild (2017, Switch, MobyScore 4.6), Ocarina of Time (1998, N64, MobyScore 4.7), Tears of the Kingdom (2023, Switch, MobyScore 4.5), and many classic entries.

---

**👤 You:**
> "Show me games developed by FromSoftware."

**🤖 AI Agent:**
> Found 40+ FromSoftware games including: Elden Ring (2022, MobyScore 4.6), Dark Souls series, Sekiro (2019), Bloodborne (2015), Armored Core series. Each with platforms, release dates and scores.

---

**👤 You:**
> "What RPGs are available for Nintendo Switch?"

**🤖 AI Agent:**
> Found 200+ RPGs for Nintendo Switch including: Xenoblade Chronicles 3 (2022, MobyScore 4.4), Fire Emblem: Three Houses (2019, 4.3), Octopath Traveler (2018, 4.2), Pokémon Scarlet/Violet (2022), and many more.


## ❓ FAQ

**Q: How do I get a MobyGames API key?**
Visit [**mobygames.com/info/api**](https://www.mobygames.com/info/api/) and register for a free API key. Free tier includes 3,600 requests/day (1 every 24 seconds).

**Q: What is MobyScore?**
MobyScore is MobyGames' user rating system (0-5 scale). It's calculated from user reviews and represents the overall quality of a game as rated by the community.

**Q: Can I search games by platform?**
Yes! Use search_games with the platform parameter. First use get_platforms to discover valid platform names (e.g. "Windows", "PlayStation 5", "Nintendo Switch", "Xbox Series").


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mobygames](https://vinkius.com/mcp/mobygames)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MobyGames** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mobygames` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MobyGames** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mobygames": {
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
