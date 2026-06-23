# Clash Royale Tactical Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clash-royale-tactical-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

The definitive server for Clash Royale — track chest rotations, analyze battle decks, and monitor clan wars via AI.

## Description
Equip your AI agent with professional-grade tactical intelligence for **Clash Royale**. This high-performance server provides deep access to the official Supercell database, allowing your agent to instantly retrieve player battle logs, analyze current deck compositions, and monitor upcoming chest rotations with sub-second precision. Whether you are a clan leader orchestrating a River Race strategy or a competitive player tracking your technical win/loss metrics, your agent acts as a dedicated tactical coach through natural conversation.

### What you can do

- **Tactical Auditing** — Retrieve detailed battle logs including crowns won, opponent decks, and tactical performance metrics
- **Economy Intelligence** — Track your upcoming chest rotation to optimize your rewards and progression strategy
- **Clan War Oversight** — Monitor real-time River Race progress, fame accumulation, and clan rankings
- **Global Benchmarking** — Fetch official leaderboards and player rankings across different regions and leagues

### How it works

1. Subscribe to this server
2. Enter your Clash Royale API Key from the [**Developer Portal**](https://developer.clashroyale.com/)
3. Start managing your royale intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Clan Leaders & Strategists** — automate the auditing of member participation and war progress for better coordination
- **Competitive Players** — monitor your recent match history and identify deck weaknesses with analytical precision
- **Data Enthusiasts** — perform deep audits of global card usage and player rankings directly from your workflow


## Available Tools (13)
- **get_battle_log**: Get recent match history for a player
- **get_upcoming_chests**: Get the next chests in a player's rotation
- **get_clan_details**: Get full profile for a Clash Royale clan
- **get_clan_members**: List all members of a clan
- **get_player_profile**: Get detailed profile and deck for a Clash Royale player
- **get_location_rankings**: locationId 57000038 = International. Type: players, clans, or clanwars.

Get top players, clans, or war clans for a location
- **get_current_river_race**: Get real-time River Race (Clan War) status
- **get_river_race_history**: Get past River Race results for a clan
- **list_global_seasons**: List all past global seasons
- **get_global_tournaments**: Get current global tournaments
- **list_all_cards**: List all available cards in the game
- **list_locations**: List all available country/location IDs
- **search_clans**: Search for clans by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clash Royale Tactical Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze my last 5 battles and show the decks my opponents used."

**🤖 AI Agent:**
> Retrieving battle logs... I've analyzed your last 5 matches. Most opponents are using 'Log Bait' or 'Pekka Bridge Spam' variations. I have the full card list for each opponent. Would you like to see the levels of their win conditions?

---

**👤 You:**
> "What are the next 10 chests in my rotation for tag '#PUUID123'?"

**🤖 AI Agent:**
> Inspecting chest cycle... For player '#PUUID123', the next 10 chests are mostly Silver and Gold, but you have a Giant Chest coming in +4 slots and a Magical Chest in +22. Shall I monitor for your next Legendary drop?

---

**👤 You:**
> "Show the current River Race standings and fame for my clan '#CLANTAG'."

**🤖 AI Agent:**
> Running war audit... Your clan '#CLANTAG' is currently in 2nd place with 8,450 fame points. You are trailing the leader by 500 points. 15 members have already completed their attacks today. Would you like the list of members who haven't participated yet?


## ❓ FAQ

**Q: Can my AI automatically predict which chest I will get next in my rotation?**
Yes! Use the `get_upcoming_chests` tool with your player tag. Your agent will respond with the next 10 chests in your specific sequence, including rare variants like Mega Lightning or Legendary chests.

**Q: How do I analyze the deck of an opponent I just lost to?**
The `get_battle_log` action retrieves your most recent matches. The agent can extract the exact card list and levels used by your opponent, helping you identify tactical counters for future encounters.

**Q: Does the integration permit tracking real-time progress in the Clan River Race?**
Yes. The `get_current_river_race` tool provides live fame points, rankings, and active participant data for your clan's current war, allowing for precise coordination during the competitive weekend.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clash-royale-tactical-intelligence](https://vinkius.com/mcp/clash-royale-tactical-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clash Royale Tactical Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clash-royale-tactical-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clash Royale Tactical Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clash-royale-tactical-intelligence": {
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
