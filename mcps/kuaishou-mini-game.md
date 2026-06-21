# Kuaishou Mini-Game MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kuaishou-mini-game)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Kuaishou mini-game developer API — manage cloud storage, leaderboards, analytics, and content moderation for casual games.

## Description
Connect your **Kuaishou Mini-Game** (快手小游戏) developer account to any AI agent and manage your casual game backend through natural conversation. Built on Kuaishou's open platform for mini-games with IAA/IAP monetization.

### What you can do
- **User Authentication** — Exchange login codes for session tokens
- **Cloud Storage** — Save/load user game data via key-value storage
- **Leaderboards** — Submit scores and retrieve rankings
- **Analytics** — Track DAU, retention, and engagement metrics
- **Content Moderation** — Check user-generated text for policy violations
- **Custom Events** — Report game-specific analytics events
- **Remote Config** — Fetch game configuration for feature flags and balancing

### How it works
1. Subscribe to this server
2. Enter your Kuaishou Mini-Game App ID and App Secret
3. Start managing your game backend from Claude, Cursor, or any MCP client

### Who is this for?
- **Game Developers** — Manage cloud saves, leaderboards, and user data
- **Analytics Teams** — Monitor retention and player engagement
- **Moderators** — Check user-generated content for policy compliance


## Available Tools (10)
- **check_content**: Essential for games with user-generated content.

Check user-generated content for policy violations
- **code2session**: This is the standard Kuaishou login flow: the mini-game client calls ks.login() to get a code, then the server exchanges it for the user session.

Exchange login code for Kuaishou user session
- **get_analytics**: Get game analytics data (DAU, retention, etc.)
- **get_game_config**: Useful for remote config, feature flags, and game balancing parameters.

Get game configuration settings
- **get_leaderboard**: Returns player rankings, scores, and basic profile info.

Get leaderboard rankings from Kuaishou game
- **get_user_info**: Requires the access token and openid obtained from code2session.

Get Kuaishou user profile information
- **get_user_storage**: Specify keys to fetch specific fields, or omit to fetch all.

Retrieve user game data from Kuaishou cloud storage
- **report_event**: Report a custom analytics event for game tracking
- **set_user_storage**: Use this to save game progress, settings, high scores, or user preferences.

Save user game data to Kuaishou cloud storage
- **submit_score**: The score is a numeric value. The leaderboard_id identifies which leaderboard to submit to.

Submit a game score to the Kuaishou leaderboard


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kuaishou Mini-Game** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Exchange login code 'abc123' for a user session."

**🤖 AI Agent:**
> ✅ Login code exchanged! User openid: ks_user_123. Session established.

---

**👤 You:**
> "Save game data: level 10, score 3000 for user ks_user_123."

**🤖 AI Agent:**
> ✅ Game data saved! Level 10, score 3000 stored in cloud storage.

---

**👤 You:**
> "Show me the top 10 players on the 'main' leaderboard."

**🤖 AI Agent:**
> 🏆 Top 10 Leaderboard: 1) PlayerA - 9850, 2) PlayerB - 8720, 3) PlayerC - 7650...


## ❓ FAQ

**Q: How do I get my Kuaishou Mini-Game credentials?**
Register at the [Kuaishou Open Platform](https://open.kuaishou.com/), create a mini-game application, and find your App ID and App Secret in the application settings.

**Q: What monetization models are supported?**
Kuaishou supports IAA (In-App Advertising) with rewarded videos and interstitial ads, as well as IAP (In-App Purchases). Revenue split is 89% for paid traffic and 30% for organic traffic.

**Q: How does cloud storage work?**
Cloud storage saves user game data as key-value pairs. Each user gets their own storage space. Use set_user_storage to save and get_user_storage to load data. Essential for cross-device game continuity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kuaishou-mini-game](https://vinkius.com/mcp/kuaishou-mini-game)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kuaishou Mini-Game** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kuaishou-mini-game` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kuaishou Mini-Game** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kuaishou-mini-game": {
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
