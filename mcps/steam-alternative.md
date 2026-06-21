# Steam MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/steam-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/steam-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/steam-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access game data, player profiles, and community content from the world largest PC gaming platform and digital storefront.

## Description
Connect your **Steam** account to any AI agent and take full control of your gaming library and community interaction workflows through natural conversation.

### What you can do

- **Library Orchestration** — List and manage your entire high-fidelity game collection programmatically, retrieving detailed playtimes and technical AppIDs
- **Player Intelligence** — Access real-time player status and summaries to coordinate your gaming availability or monitor friends' activities
- **Achievement Architecture** — Programmatically retrieve high-fidelity game achievements and progress for specific apps to maintain a perfectly coordinated gaming record
- **Recent Activity Monitoring** — Access high-fidelity metadata for recently played games and session durations directly through your agent for instant performance reporting
- **Operational Monitoring** — Verify account-level API connectivity and monitor service status directly through your agent for instant technical reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Web API Key** from the Steam Community Dev page (steamcommunity.com/dev/apikey)
3. Start orchestrating your gaming data from Claude, Cursor, or any MCP client

No more manual checking of Steam profiles for playtimes or friend status. Your AI acts as your dedicated gaming coordinator and achievement architect.

### Who is this for?

- **Gamers** — instantly retrieve personal library summaries and track achievements using natural language commands
- **Content Creators** — monitor gaming sessions and verify playtime metadata without leaving your creative workspace
- **Developers** — integrate high-speed Steam Web API data into custom gaming dashboards through simple AI queries


## Available Tools
- **get_global_achievements**: Get global achievement percentages
- **get_friend_list**: Get friend list for a Steam user
- **get_game_news**: Get news for a specific game
- **get_owned_games**: Get games owned by a Steam user
- **get_player_summaries**: Get community profile data for Steam users
- **get_recently_played_games**: Get recently played games
- **resolve_vanity_url**: Resolve a Steam vanity URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steam** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all games in my Steam library and show my total playtime for 'Counter-Strike 2'."

**🤖 AI Agent:**
> I've retrieved your library. You have 150 high-fidelity games. For 'Counter-Strike 2' (AppID: 730), your total playtime is 1,200 hours. Would you like to check your recent achievements for it?

---

**👤 You:**
> "Check which of my friends are currently online and what they are playing."

**🤖 AI Agent:**
> Accessing player summaries... 5 friends are currently online. 'John_Doe' is playing 'Dota 2', and 'Jane_Smith' is Away. I've retrieved the high-fidelity session metadata for your review. Need help joining a lobby?

---

**👤 You:**
> "Show my recent activity for the last 2 weeks."

**🤖 AI Agent:**
> Activity orchestrated! In the last 2 weeks, you've played 3 games, including 'Elden Ring' for 15 high-fidelity hours. Your total gaming time across all apps is 25 hours. Shall I retrieve your progress on recent achievements?


## Installation & Usage

To install and use the **Steam** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/steam-alternative](https://vinkius.com/mcp/steam-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
