# Steam Platform & Hype Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/steam-platform-hype-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

The definitive server for Steam platform insights — track trending games, player counts, and social connections via AI.

## Description
Equip your AI agent with the pulse of the world's largest PC gaming platform via **Steam Platform & Hype Intelligence**. This server provides deep access to real-time market trends, social metadata, and community activity. Your agent can instantly identify trending titles, monitor live player counts, audit public wishlists, and analyze social connections between profiles. Whether you are a community manager tracking hype or a gamer looking for the next big hit like Deadlock, your agent acts as a professional Steam analyst through natural conversation.

### What you can do

- **Trend Monitoring** — Identify top-selling and most-played games on the platform in real-time
- **Hype Auditing** — Retrieve live player counts and news updates to quantify the momentum of any title
- **Social Intelligence** — Resolve custom vanity URLs and analyze public friend lists and group memberships
- **User Insights** — Audit recently played games and public wishlists to understand gaming habits

### How it works

1. Subscribe to this server
2. Enter your Steam Web API Key
3. Start managing your Steam intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Community Managers** — instantly monitor the hype and player base of your games
- **Influencers & Curators** — identify trending titles and patch notes for content creation
- **Analytical Gamers** — track your social connections and wishlist opportunities with precision


## Available Tools (11)
- **get_app_details**: Get full store page details for a game
- **search_all_steam_apps**: Get the full list of apps on Steam
- **get_app_news**: Get latest news and patch notes for a game
- **get_featured_categories**: Get current Steam Store featured categories
- **get_friend_list**: Requires public profile.

List friends for a Steam user
- **get_owned_games**: List all games owned by a player
- **get_current_player_count**: Get live player count for a game
- **get_player_summary**: Get basic player profile details
- **get_recently_played**: List games played in the last 2 weeks
- **list_featured_games**: List featured and trending games on Steam
- **resolve_vanity_url**: g., /id/gaben) into a 64-bit Steam ID.

Resolve a custom Steam URL to SteamID64


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steam Platform & Hype Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Identify the top trending games on Steam right now."

**🤖 AI Agent:**
> Retrieving trending titles... I've identified the current top games including 'Deadlock' and 'Black Myth: Wukong'. I have their current sales ranking and featured banners. Would you like to see the live player count for these titles?

---

**👤 You:**
> "Resolve the vanity URL 'faker' and show his public profile summary."

**🤖 AI Agent:**
> Resolving URL... Custom ID 'faker' corresponds to SteamID64 `765611980345...`. His profile shows he is currently 'Online' and his primary game is League of Legends. I also have his avatar and profile link. Shall I check his recently played games?

---

**👤 You:**
> "Analyze the latest patch notes for Counter-Strike 2 (AppID 730)."

**🤖 AI Agent:**
> Inspecting latest updates... I found a significant patch from today regarding map adjustments on Mirage and sub-tick networking improvements. I have the full summary of technical changes. Would you like the details on weapon balance adjustments?


## ❓ FAQ

**Q: Can my AI automatically find the AppID of a game using only its name?**
Yes! Use the `search_all_steam_apps` tool. Your agent will scan the Steam database and return matching AppIDs, which are required for all other technical tools.

**Q: Is it possible to monitor the live player count for a new game like Deadlock?**
Absolutely. The `get_current_player_count` tool provides real-time data from Steam servers, allowing you to quantify the hype and player base of any specific title at any moment.

**Q: How do I find a user's SteamID64 if I only have their profile URL?**
Use the `resolve_vanity_url` tool with the custom part of the URL. The agent will return the unique 64-bit identifier required for all user-specific statistical queries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/steam-platform-hype-intelligence](https://vinkius.com/mcp/steam-platform-hype-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steam Platform & Hype Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steam-platform-hype-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steam Platform & Hype Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steam-platform-hype-intelligence": {
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
