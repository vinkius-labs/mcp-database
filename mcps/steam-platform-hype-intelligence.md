# Steam Platform & Hype Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/steam-platform-hype-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/steam-platform-hype-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/steam-platform-hype-intelligence-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Steam Platform & Hype Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/steam-platform-hype-intelligence](https://vinkius.com/mcp/steam-platform-hype-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
