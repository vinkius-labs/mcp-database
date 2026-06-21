# OpenCritic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opencritic)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Unified video game review platform — access scores, critic reviews, and rankings via AI.

## Description
Equip your AI agent with the most reliable video game intelligence available via **OpenCritic**. This unified server provides your agent with instant access to aggregate review scores, detailed critic snippets, and historical rankings for thousands of games. Your agent can instantly search for specific titles, audit recent review trends, and retrieve the Hall of Fame for any given year without you ever needing to browse a review site. Whether you are identifying the best games of the year or auditing individual critic opinions, your agent acts as a dedicated gaming analyst through natural conversation.

### What you can do

- **Game Discovery** — Search for thousands of video games by title and retrieve their OpenCritic rating and tier.
- **Review Auditing** — Fetch detailed snippets and scores from individual critics and publications for any game.
- **Market Trends** — Retrieve lists of upcoming releases and currently popular/trending games on the platform.
- **Historical Rankings** — Access the 'Hall of Fame' to identify the top-rated games for a specific year.
- **Critic Intelligence** — List and inspect recognized critics and publications to understand the source of reviews.

### How it works

1. Subscribe to this server
2. Enter your OpenCritic RapidAPI Key
3. Start managing your gaming intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Gamers & Enthusiasts** — instantly find out if a new release is worth their time and money.
- **Content Creators** — retrieve aggregate scores and recent reviews for game analysis and commentary.
- **Game Developers & Publishers** — monitor review trends and critic feedback for their titles in real-time.
- **Market Researchers** — analyze historical performance and popularity of games across different genres.


## Available Tools
- **get_game_details**: Get game details
- **get_game_reviews**: Get game reviews
- **get_hall_of_fame**: Get Hall of Fame games
- **list_critics**: List critics
- **get_popular_games**: Get popular games
- **get_recent_reviews**: Get recent reviews
- **search_games**: Search for video games
- **get_upcoming_games**: Get upcoming games


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenCritic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the OpenCritic score for 'Elden Ring'?"

**🤖 AI Agent:**
> Searching OpenCritic for 'Elden Ring'... It has an outstanding Top Critic Average of 95 and is rated as 'Mighty'. 98% of critics recommend this game. Would you like to read some specific review snippets?

---

**👤 You:**
> "List the top games from 2023."

**🤖 AI Agent:**
> Retrieving the 2023 Hall of Fame... The top-rated titles include 'Baldur's Gate 3', 'The Legend of Zelda: Tears of the Kingdom', and 'Alan Wake 2'. Shall I give you the exact scores for each?

---

**👤 You:**
> "Show me upcoming games on OpenCritic."

**🤖 AI Agent:**
> Fetching upcoming releases... I see several highly anticipated titles coming soon, such as 'Dragon's Dogma 2' and 'Hades II'. I can track their review status for you as they get closer to launch.


## ❓ FAQ

**Q: What is the difference between 'Top Critic Average' and 'OpenCritic Rating'?**
The 'Top Critic Average' is the simple numeric mean of scores, while the 'OpenCritic Rating' (Tier) categorizes the game into levels like Mighty, Strong, Fair, or Weak based on its performance relative to other games.

**Q: Can I see reviews from a specific publication like IGN or GameSpot?**
Yes! Use the `get_game_reviews` tool with the Game ID. The response will include a list of individual reviews, identifying the critic and their publication for each snippet.

**Q: How do I find the best games released in a specific year?**
Use the `get_hall_of_fame` tool and provide the target year. Your agent will retrieve the highest-rated games for that period according to OpenCritic's aggregate scores.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opencritic](https://vinkius.com/mcp/opencritic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenCritic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `opencritic` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenCritic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opencritic": {
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
