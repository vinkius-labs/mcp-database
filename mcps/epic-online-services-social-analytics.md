# Epic Online Services & Social Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/epic-online-services-social-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

The definitive server for Epic Games social intelligence — track player profiles, friends, and achievements via AI.

## Description
Equip your AI agent with the power of the **Epic Online Services (EOS)** ecosystem. This advanced MCP server provides deep access to official player metadata, social connections, and cross-platform achievement statistics. Your agent can instantly resolve display names into unique AccountIDs, audit global and personal achievement rarities, and monitor real-time presence to see what your contacts are playing. Whether you are performing technical scouting for professional rosters or analyzing social networks within the Epic ecosystem, your agent acts as a dedicated social data engineer through natural conversation.

### What you can do

- **Player Profiling** — Resolve display names and retrieve unique AccountIDs and public biographical metadata
- **Social Intelligence** — Fetch official friend lists and analyze community connections between profiles
- **Performance Auditing** — Track player achievements and technical stats for specific titles including Fortnite and Indie hits
- **Presence Monitoring** — Retrieve real-time online status and active game session data for any target account

### How it works

1. Subscribe to this server
2. Enter your Epic Client ID and Secret (from the Epic Developer Portal)
3. Start managing your Epic social intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-sports Scouts** — perform deep audits of player profiles and social connections for recruitment
- **Community Managers** — monitor active player counts and social engagement trends within your community
- **Analytical Gamers** — track your achievement progress and friend activity with micro-metric precision


## Available Tools
- **get_account_details**: Get full profile for an Epic account by ID
- **get_achievement_definitions**: List all achievements available in a game
- **get_blocked_users**: List blocked users for an account
- **get_friend_list**: List friends for an Epic account
- **get_game_leaderboard**: Get leaderboard rankings for a game
- **get_player_achievements**: Get achievement progress for a player in a game
- **get_player_presence**: Check if a player is online or in-game
- **search_account_by_display_name**: Find an Epic account ID by display name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Epic Online Services & Social Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the AccountID for the Epic user 'Ninja'."

**🤖 AI Agent:**
> Resolving display name... I've found the account for 'Ninja'. His unique AccountID is `0002...`. I also identified his public biographical metadata. Would you like to check his friend list or current presence status?

---

**👤 You:**
> "Check the live status and game for AccountID 'ID_12345'."

**🤖 AI Agent:**
> Running presence check... The user is currently 'Online' and playing 'Fortnite'. The session has been active for 45 minutes. Would you like to see their recent performance stats for this season?

---

**👤 You:**
> "Analyze the rarity of achievements for 'Alan Wake 2' on my account."

**🤖 AI Agent:**
> Inspecting achievement logs... You have unlocked 15 out of 60 achievements. Your rarest unlock is 'The Final Chapter', which only 4.2% of the community possesses. Shall I list the technical requirements for the remaining locked achievements?


## ❓ FAQ

**Q: Can my AI automatically resolve an Epic Display Name into an AccountID?**
Yes! Use the `search_account_by_display_name` tool. Your agent will query the EOS database and return the unique identifier required for all other social and performance tools.

**Q: How do I check if a player is currently in an active game session?**
The `get_player_presence` tool retrieves real-time data from the Epic servers, indicating whether the player is 'Online', 'Away', or in a specific 'Game Session' with the associated AppID.

**Q: Does the integration permit tracking achievement rarity across the entire Epic community?**
Yes. The `get_achievement_definitions` action retrieves the percentage of all Epic players who have unlocked a specific achievement, allowing the agent to quantify the difficulty of technical milestones.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/epic-online-services-social-analytics](https://vinkius.com/mcp/epic-online-services-social-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Epic Online Services & Social Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `epic-online-services-social-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Epic Online Services & Social Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "epic-online-services-social-analytics": {
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
