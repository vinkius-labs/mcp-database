# Heybox MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/heybox)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/heybox-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/heybox-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access Heybox (小黑盒) gamer database — track Steam/PUBG/CS2 statistics and monitor community trends directly from any AI agent.

## Description
Connect your AI agents to **Heybox** (小黑盒), the leading PC gaming community and database platform in China. This MCP provides 10 tools to access granular game information, player statistics for competitive titles like PUBG and CS2, and trending community content.

### What you can do

- **Game Insights** — Retrieve ratings, market prices, and community sentiment for any Steam or Heybox game
- **Player Analytics** — Track match history, playtime, and rank progression for linked accounts
- **Community Monitoring** — List top posts and news from the massive Heybox BBS boards
- **Market Trends** — Monitor item prices and active giveaways/lottery events

### How it works

1. Subscribe to this server
2. Log in to the [**Heybox Developer Platform**](https://xiaoheihe.cn/)
3. Apply for official API access to obtain an **API Key**
4. (Optional) Identify your **User ID** from your account profile settings
5. Insert your credentials into the fields below to start automating your gaming market research.

### Who is this for?

- **Game Developers** — monitor player sentiment and competitive rankings in the Chinese market
- **Market Researchers** — track item trading prices and trending titles at scale
- **Gaming Enthusiasts** — automate the retrieval of personal match stats and news updates


## Available Tools
- **get_heybox_app_status**: Get Heybox task and app status
- **get_game_info**: Retrieve detailed information for a game
- **get_market_prices**: g., CS2, PUBG skins).

Check current market prices for game items
- **get_match_history**: Get recent match history for a competitive game
- **get_post_detail**: Get complete content of a community post
- **get_user_stats**: ).

Retrieve gaming statistics for a user
- **list_community_posts**: List trending posts in a community board
- **list_discount_games**: Retrieve the current discounted games
- **list_game_news**: Get the latest gaming industry news
- **list_lotteries**: Retrieve current official lotteries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heybox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the current market prices for CS2 items from Heybox."

**🤖 AI Agent:**
> Retrieving market data... I found current prices for top CS2 skins. For example, 'Butterfly Knife | Lore' is trending at ¥XXXX. Would you like a full list of recent skin transactions?

---

**👤 You:**
> "Show me the top trending posts in the PUBG board."

**🤖 AI Agent:**
> Fetching community feed for PUBG... I found 3 trending posts: 1. 'New Map Leak' (2.5K likes), 2. 'Pro Tips for Sniping' (1.8K likes), 3. 'Tournament Announcement' (1.2K likes).

---

**👤 You:**
> "Get detailed info for Steam game ID '570' (Dota 2)."

**🤖 AI Agent:**
> Querying Heybox game database... Dota 2 (ID: 570) has a community score of 9.5/10. It is currently one of the most played games in the Chinese region. Would you like to see recent news for this title?


## Installation & Usage

To install and use the **Heybox** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heybox](https://vinkius.com/mcp/heybox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
