# Epic Games Store Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/epic-games-store-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

The definitive server for the Epic ecosystem — track free games, catalog trends, and store promotions via AI.

## Description
Equip your AI agent with real-time intelligence for the world's most dynamic PC gaming storefront via **Epic Games Store Intelligence**. This server provides deep access to the official Epic GraphQL catalog, allowing your agent to instantly identify the 'Free Games of the Week', monitor major seasonal sales, and audit technical metadata for thousands of titles. From tracking Fortnite news to searching for hidden indie gems, your agent acts as a professional Epic Games consultant through natural conversation.

### What you can do

- **Freebies Monitoring** — Instantly retrieve the list of currently active and upcoming free games to never miss an offer
- **Catalog Auditing** — Search the entire storefront using GraphQL queries to find prices, descriptions, and high-quality banners
- **Trend Intelligence** — Identify new releases and top-selling titles across multiple categories including RPG, Action, and Indie
- **Live Service Status** — Monitor the operational status of Epic Games services and receive official news updates

### How it works

1. Subscribe to this server
2. Enter your Epic Client ID and Secret (obtainable from the Epic Developer Portal)
3. Start managing your Epic intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Bargain Hunters** — instantly audit the best free offers and seasonal discounts directly from your workflow
- **Game Researchers** — perform technical audits of catalog metadata and developer histories
- **Content Creators** — retrieve official news, banners, and trending tags for the latest gaming updates


## Available Tools (8)
- **get_free_games**: List current and upcoming free games
- **get_game_details**: Get detailed product info for a specific game
- **list_new_releases**: List the most recent game releases
- **list_games_on_sale**: List games currently on sale with discounts
- **list_top_sellers**: List current best-selling games
- **search_games_by_category**: Browse games by store category
- **search_games_by_tag**: Common tags: RPG, Action, Adventure, Indie, Survival, Shooter, Puzzle.

Find games by tag or genre
- **search_store_catalog**: Returns titles, prices, descriptions, seller info, and cover images.

Search for games on the Epic Games Store


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Epic Games Store Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which games are free on the Epic Games Store right now?"

**🤖 AI Agent:**
> Checking the freebie vault... I found 2 free games available this week: 'Game Title A' and 'Game Title B'. I also identified that 'Upcoming Title' will be free starting next Thursday. Would you like the direct claim links?

---

**👤 You:**
> "Search for all Batman games in the catalog and show their current prices."

**🤖 AI Agent:**
> Running the GraphQL query for 'Batman'... I found 4 titles including the 'Arkham Trilogy' (currently on sale for $14.99) and 'LEGO Batman'. Would you like to see the full technical metadata for the Arkham bundle?

---

**👤 You:**
> "Analyze the latest news and seasonal events for Fortnite."

**🤖 AI Agent:**
> Inspecting Fortnite updates... A new season started yesterday with significant map changes and a new battle pass. I also found an upcoming live concert event scheduled for Saturday. Shall I provide the detailed patch notes?


## ❓ FAQ

**Q: Can my AI automatically find the next free game even if it hasn't been released yet?**
Yes! The `get_free_games` tool retrieves both the current active free titles and the upcoming freebies announced by Epic, including their scheduled start dates.

**Q: How accurate is the pricing and discount data provided?**
The data is sourced directly from Epic's official GraphQL backend, ensuring 100% accuracy for current prices, original MSRP, and active promotional discounts.

**Q: Does the integration permit tracking official Fortnite seasonal events and news?**
Yes. The `search_store_catalog` tool specifically targets the Fortnite namespace to retrieve the latest updates, patch notes, and seasonal event announcements directly from the track.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/epic-games-store-intelligence](https://vinkius.com/mcp/epic-games-store-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Epic Games Store Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `epic-games-store-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Epic Games Store Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "epic-games-store-intelligence": {
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
