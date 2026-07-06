# Clash of Clans Strategy & War Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clash-of-clans-strategy-war-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

The definitive server for Clash of Clans — track clan wars, player progress, and global rankings via AI.

## Description
Equip your AI agent with professional-grade strategic intelligence for **Clash of Clans**. This high-performance server provides deep access to the official Supercell database, allowing your agent to instantly audit clan war logs, monitor real-time war status (stars, destruction), and analyze detailed player profiles including hero levels and troop progress. Whether you are a clan leader orchestrating a War League (CWL) strategy or a competitive player tracking global leaderboards, your agent acts as a dedicated tactical advisor through natural conversation.

### What you can do

- **War Intelligence** — Retrieve real-time updates for ongoing wars and analyze historical win/loss streaks via the war log
- **Player Scouting** — Fetch granular statistics for any player tag including Town Hall level, trophy counts, and donation ratios
- **Clan Management** — Search for top-tier clans and audit member rosters, roles, and entry requirements
- **Seasonal Oversight** — Access current Gold Pass rewards and monitor Legend League rankings across different regions

### How it works

1. Subscribe to this server
2. Enter your Clash of Clans API Key (JWT) from the [**Developer Portal**](https://developer.clashofclans.com/)
3. Start managing your clan intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Clan Leaders & Co-leaders** — automate the auditing of member performance and war participation for better coordination
- **Competitive Players** — monitor your own progress and compare technical stats with top global players
- **Strategy Enthusiasts** — analyze war histories and opponent compositions to optimize attack plans


## Available Tools (14)
- **get_cwl_group**: Get Clan War League group status
- **get_capital_raid_seasons**: Get Clan Capital raid history
- **get_clan_details**: Use the clan tag with #.

Get full profile for a Clash of Clans clan
- **get_gold_pass_season**: Get current Gold Pass season info
- **get_clan_members**: List all members of a clan with roles and stats
- **get_current_war**: Get live status of an ongoing clan war
- **get_player_profile**: Get detailed stats for a Clash of Clans player
- **get_location_rankings**: Use locationId 32000006 for International. Type: clans or players.

Get top players or clans for a location
- **get_clan_war_log**: Get war history for a clan
- **list_official_labels**: Type: clans or players.

List official clan or player labels/tags
- **list_trophy_leagues**: List all trophy league tiers
- **list_locations**: List all available location/country IDs
- **list_war_leagues**: List all CWL league tiers
- **search_clans**: Search for clans by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clash of Clans Strategy & War Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the current war status for clan tag '#2PP' and show the current score."

**🤖 AI Agent:**
> Retrieving live war data... Clan '#2PP' is currently in war against 'Opponent Clan'. The score is 45-42 in your favor, with 15 attacks remaining. Your destruction percentage is at 92.5%. Would you like to see which members still have attacks left?

---

**👤 You:**
> "Get the hero levels and war stars for player tag '#PUUID123'."

**🤖 AI Agent:**
> Inspecting player profile... Player '#PUUID123' has a Barbarian King at Level 85, Archer Queen at Level 90, and Grand Warden at Level 65. They have earned a total of 1,540 War Stars. Would you like to see their troop levels for specific war compositions?

---

**👤 You:**
> "Show the top 5 clans in Brazil based on current trophy rankings."

**🤖 AI Agent:**
> Running the location audit for Brazil... The top 5 clans are currently 'Clan A', 'Clan B', 'Clan C', 'Clan D', and 'Clan E'. 'Clan A' leads with over 65,000 trophies. Shall I provide the requirements to join the number one ranked clan?


## ❓ FAQ

**Q: Can my AI automatically find the remaining attacks in our current clan war?**
Yes! Use the `get_current_war` tool with your clan tag. Your agent will retrieve the real-time war state, including current stars, destruction percentage, and how many attacks each team has already used.

**Q: How do I check the hero levels and troop progress for a potential new member?**
Simply provide the Player Tag to the agent and ask for player info. It will run the `get_player_profile` action to retrieve the full technical breakdown of their Town Hall level, hero levels, and troop levels directly from the track.

**Q: Does the integration allow auditing the historical performance of an opponent clan?**
Yes. If the target clan has a public war log, the `get_clan_war_log` tool allows your agent to fetch their last 50 wars, providing data on their win/loss ratio and common destruction percentages.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clash-of-clans-strategy-war-analytics](https://vinkius.com/mcp/clash-of-clans-strategy-war-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clash of Clans Strategy & War Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clash-of-clans-strategy-war-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clash of Clans Strategy & War Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clash-of-clans-strategy-war-analytics": {
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
