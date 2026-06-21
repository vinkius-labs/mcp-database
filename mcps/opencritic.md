# OpenCritic MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opencritic)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/opencritic-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/opencritic-mcp)
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


## Installation & Usage

To install and use the **OpenCritic** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opencritic](https://vinkius.com/mcp/opencritic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
