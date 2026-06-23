# Fortnite Player Stats & News Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fortnite-player-stats-news-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

The definitive server for Fortnite player scouting — track wins, K/D ratios, and official game news via AI.

## Description
Equip your AI agent with professional-grade player intelligence for the world's most popular Battle Royale via **Fortnite Player Stats & News**. This high-performance server provides deep access to official player performance metrics and real-time game updates. Your agent can instantly retrieve detailed Battle Royale statistics including win rates, K/D ratios, and seasonal levels, while also monitoring the official news feed for all game modes (BR, Save the World, Creative). Whether you are performing technical scouting for recruitment or analyzing the latest patch notes to understand the meta, your agent acts as a dedicated Fortnite analyst through natural conversation.

### What you can do

- **Player Profiling** — Retrieve comprehensive performance metrics including K/D, total matches, and wins for any Epic account
- **Real-time News Ticker** — Follow official announcements and mission updates for Battle Royale, Save the World, and Creative modes
- **Technical Auditing** — Analyze seasonal progress and level rankings to identify high-performance trends across the community
- **Creator Intelligence** — Verify Support-A-Creator codes and retrieve associated account metadata immediately

### How it works

1. Subscribe to this server
2. Enter your Fortnite-API Key (obtainable via their official dashboard)
3. Start managing your Fortnite player intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-sports Scouts & Coaches** — instantly audit player profiles and technical histories for recruitment and tactical analysis
- **Data Journalists** — retrieve high-integrity player stats and official news for reporting and community updates
- **Competitive Gamers** — monitor your own performance trends and stay updated on the latest meta-shifting news


## Available Tools (11)
- **check_creator_code**: Check if a Support-A-Creator code is active
- **get_aes_keys**: Get encryption keys for Fortnite game files
- **get_battle_royale_news**: Get current Battle Royale news and updates
- **get_banners**: List all profile banners available in Fortnite
- **get_creative_mode_news**: Get current Creative mode news and featured maps
- **get_current_map**: Get the current Fortnite map with POIs
- **get_player_br_stats**: Supports season or lifetime window.

Get Battle Royale stats for a Fortnite player
- **get_playlists**: List all available Fortnite playlists/gamemodes
- **get_save_the_world_news**: Get current Save the World news
- **get_item_shop**: Auto-updated at 00:00 UTC.

Get the current daily and featured item shop
- **search_cosmetics**: Returns images, rarity, introduction date, and set info.

Search for Fortnite cosmetics by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fortnite Player Stats & News Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve the Battle Royale stats for 'Ninja' and show his current seasonal level."

**🤖 AI Agent:**
> Fetching professional stats... Ninja is currently Level 125 in the Battle Pass. He has a 4.5 K/D ratio this season with over 200 wins. Would you like to see his cumulative stats across all seasons?

---

**👤 You:**
> "Compare the seasonal K/D performance of 'UserX' versus 'UserY'."

**🤖 AI Agent:**
> Running the technical comparison... UserX leads with a 3.2 K/D, while UserY has a higher winrate of 15% but a 2.8 K/D. I have the detailed kill counts for both. Shall I provide the full breakdown?

---

**👤 You:**
> "What are the latest news updates for the Fortnite Creative mode today?"

**🤖 AI Agent:**
> Inspecting Creative mode news... 2 new featured maps were highlighted today, including a new 'Zone Wars' experience. I also found an update regarding new assets available for creators. Would you like the island codes?


## ❓ FAQ

**Q: Can my AI automatically find the K/D ratio and winrate for a specific Fortnite player?**
Yes! Use the `get_player_br_stats` tool. Your agent will query the Fortnite-API database and return granular metrics including total kills, deaths, wins, and win percentages for the current season or lifetime.

**Q: How do I check the latest 'Patch Notes' or mission updates for Save the World?**
Simply ask the agent to run the `get_save_the_world_news` tool. It will retrieve official mission briefings and update logs directly from Epic's news feed.

**Q: Does the integration permit comparing the performance of two different users side-by-side?**
Yes. The `get_player_br_stats` action allows your agent to fetch data for multiple usernames and compile a technical comparison of their seasonal performance, allowing for direct skill auditing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fortnite-player-stats-news-intelligence](https://vinkius.com/mcp/fortnite-player-stats-news-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fortnite Player Stats & News Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fortnite-player-stats-news-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fortnite Player Stats & News Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fortnite-player-stats-news-intelligence": {
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
