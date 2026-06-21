# GamerPower MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gamerpower)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track live game giveaways, free loot, and beta keys via AI agents with GamerPower.

## Description
Connect your AI agent to the **GamerPower** database to automate your discovery of live gaming giveaways and free loot through the Model Context Protocol (MCP). GamerPower is a dedicated tracker for free-to-keep games, in-game items, and beta access across all major platforms. This MCP server enables you to list active giveaways, filter by platform, and retrieve detailed claiming instructions directly through natural conversation.

### Key Features

- **Real-time Giveaway Discovery** — List all live giveaways across PC, console, and mobile platforms instantly.
- **Platform Filtering** — Retrieve giveaways exclusively for Steam, Epic Games Store, PlayStation 5, Xbox Series X|S, and more.
- **Type Categorization** — Focus on full game downloads, in-game loot/skins, or early access beta keys.
- **Detailed Instructions** — Fetch complete metadata for any giveaway, including the specific steps required to claim the item.
- **Worth Analysis** — Get high-level statistics on the total number of active giveaways and their cumulative USD market value.
- **Popularity Tracking** — Sort results by popularity or value to find the most sought-after gaming deals.
- **No Auth Required** — Access the public GamerPower database immediately without complex API key configurations.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. No credentials required (Public API)
3. Start discovering free games from Claude, Cursor, or any MCP client

### Who is this for?

- **Gamers & Enthusiasts** — quickly check for new free games on your favorite platform without manual site browsing.
- **Content Creators** — get a real-time overview of active loot giveaways to share with your community via simple AI commands.
- **Deal Hunters** — automate the monitoring of high-value game giveaways and beta access opportunities.


## Available Tools
- **get_giveaway_details**: Get giveaway metadata
- **get_giveaway_worth**: Get worth statistics
- **list_all_giveaways**: List all giveaways
- **list_beta_keys**: Filter for beta access
- **list_epic_games_giveaways**: Filter for Epic Games
- **list_ingame_loot**: Filter for loot
- **list_mobile_giveaways**: Filter for Android/iOS
- **list_pc_full_games**: Filter for PC games
- **list_ps5_giveaways**: Filter for PS5
- **list_steam_giveaways**: Filter for Steam
- **list_xbox_giveaways**: Filter for Xbox
- **search_giveaways**: Search by platform/type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GamerPower** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the latest free games on Steam right now?"

**🤖 AI Agent:**
> Checking Steam... I found 3 active giveaways, including 'Content Warning' (Free to keep) and 'The Elder Scrolls Online' (Limited time). Would you like the instructions to claim them?

---

**👤 You:**
> "Show me free loot or skins for 'League of Legends'."

**🤖 AI Agent:**
> Fetching loot... I found an active giveaway for a 'Mystery Emote' via Prime Gaming and a 'Champ Select Pack' via the official site. Which one should I detail?

---

**👤 You:**
> "Get the total worth of all active gaming giveaways."

**🤖 AI Agent:**
> Calculating value... There are currently 85 active giveaways with a total estimated USD worth of $1,245.50. You can save over a thousand dollars by claiming them all!


## ❓ FAQ

**Q: Is authentication required for GamerPower?**
No, this MCP server uses the public GamerPower API which does not require an API key or account registration.

**Q: What types of giveaways are tracked?**
GamerPower tracks free full games, in-game loot (skins, currency), and beta test keys across all major platforms.

**Q: How do I filter for a specific platform?**
You can use specific tools like 'list_steam_giveaways' or use the general 'search_giveaways' tool and provide a platform name (e.g., 'ps5', 'pc').

**Q: Can I see the instructions to claim a giveaway?**
Yes! The 'get_giveaway_details' tool provides step-by-step metadata on how to claim each free item or game.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gamerpower](https://vinkius.com/mcp/gamerpower)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GamerPower** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gamerpower` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GamerPower** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gamerpower": {
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
