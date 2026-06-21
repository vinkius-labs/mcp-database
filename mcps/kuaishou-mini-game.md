# Kuaishou Mini-Game MCP Server

Kuaishou mini-game developer API — manage cloud storage, leaderboards, analytics, and content moderation for casual games.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/kuaishou-mini-game)

## Overview
**Category:** industry-titans
**Tools Count:** 10

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


## Available Tools
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


## Installation & Usage

To install and use the **Kuaishou Mini-Game** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kuaishou-mini-game](https://vinkius.com/mcp/kuaishou-mini-game)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
