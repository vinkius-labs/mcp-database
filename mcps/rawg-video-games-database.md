# RAWG Video Games Database MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rawg-video-games-database)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Universal video game intelligence — search 500,000+ games, platforms, and ratings via AI.

## Description
Equip your AI agent with the world's largest video game database through the **RAWG** MCP server. This integration provides real-time access to metadata for over half a million games across 50+ platforms. Your agent can search for specific titles, retrieve detailed descriptions, check average community ratings, and list supported platforms for any game. Whether you are building a discovery engine, auditing gaming history, or checking release dates, your agent acts as a dedicated gaming encyclopedist through natural conversation.

### What you can do

- **Global Game Search** — Find video games by title or partial string across a massive catalog.
- **Detailed Metadata** — Access descriptions, release dates, and community ratings for any game.
- **Platform Intelligence** — Check which consoles or systems a game was released on.
- **Discovery & Exploration** — List all gaming platforms and explore related titles.
- **Gaming Auditing** — Summarize historical performance and availability of classic and modern games.

### How it works

1. Subscribe to this server
2. Enter your RAWG API Key (get it for free at rawg.io/apidocs)
3. Start querying global gaming data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Gamers & Enthusiasts** — explore game details and discover new titles to play.
- **Gaming Journalists** — quickly pull metadata and release info for reporting.
- **App Developers** — integrate a comprehensive gaming database into custom applications.
- **Researchers** — analyze trends in ratings and platform availability across the industry.


## Available Tools (3)
- **get_video_game_details**: Get detailed info for a video game
- **list_video_game_platforms**: g., PS5, Xbox Series X, PC).

List all available gaming platforms
- **search_video_games**: Search for video games by title


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RAWG Video Games Database** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'The Legend of Zelda' games on RAWG."

**🤖 AI Agent:**
> Searching for Zelda... I've found multiple titles including 'Breath of the Wild' and 'Tears of the Kingdom'. I can provide release dates and ratings for each of them. Which one would you like to explore?

---

**👤 You:**
> "Get details for the game 'Grand Theft Auto V'."

**🤖 AI Agent:**
> Retrieving GTA V data... It's one of the most popular games in the database. Released in 2013, it's available on almost every platform from PC to PS5. It has an average rating of 4.5/5. Would you like to read the description?

---

**👤 You:**
> "List all gaming platforms supported by RAWG."

**🤖 AI Agent:**
> Fetching the platform list... RAWG supports over 50 platforms, including current generation systems like PlayStation 5, Xbox Series S/X, and Nintendo Switch, as well as retro systems like the NES and Commodore 64.


## ❓ FAQ

**Q: Can I search for 'Cyberpunk 2077' and see its platforms?**
Yes! Use the `search_video_games` tool with the query 'Cyberpunk 2077'. The results will show you all platforms where the game is available, such as PC, PlayStation, and Xbox.

**Q: How do I see the average community rating?**
The ratings are included in the game metadata retrieved by the `get_game_details` or `search_video_games` tools. It shows the average score given by RAWG users.

**Q: Is it possible to list all games for a specific platform?**
The current toolset focuses on searching and retrieving specific game details. To explore platforms, you can use the `list_platforms` tool to see all supported systems.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rawg-video-games-database](https://vinkius.com/mcp/rawg-video-games-database)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RAWG Video Games Database** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rawg-video-games-database` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RAWG Video Games Database** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rawg-video-games-database": {
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
