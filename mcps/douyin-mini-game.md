# Douyin Mini-Game MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/douyin-mini-game)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/douyin-mini-game-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/douyin-mini-game-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Douyin mini-game developer API — manage cloud storage, leaderboards, user sessions, and content moderation for casual games.

## Description
Connect your **Douyin Mini-Game** (抖音小游戏) developer account to any AI agent and manage your casual game backend through natural conversation. Access cloud storage, leaderboards, analytics, and content moderation — all via the Douyin Open Platform API.

### What you can do
- **User Authentication** — Exchange login codes for session tokens (openid/session_key)
- **Cloud Storage** — Save and load user game data (progress, settings, scores) via key-value cloud storage
- **Leaderboards** — Submit scores and check player rankings across different game modes
- **Analytics** — Track DAU, retention rates, and engagement metrics
- **Content Moderation** — Check user-generated text for policy violations before publishing
- **User Profiles** — Retrieve player nicknames, avatars, and account details

### How it works
1. Subscribe to this server
2. Enter your Douyin Mini-Game App ID and App Secret
3. Start managing your game backend from Claude, Cursor, or any MCP client

### Who is this for?
- **Game Developers** — Manage cloud saves, leaderboards, and user data
- **Analytics Teams** — Monitor retention, DAU trends, and player engagement
- **Moderators** — Check user-generated content for policy compliance


## Available Tools
- **check_content_security**: ) against Douyin's content policies. Returns whether the content is safe or contains prohibited material. Essential for games with user-generated content features.

Check user-generated content for policy violations
- **code2session**: This is the standard Douyin login flow: the mini-game client calls tt.login() to get a code, then the server exchanges it for the user session.

Exchange login code for user session (openid/session_key)
- **get_access_token**: This token is required for all subsequent API calls including user authentication, cloud storage, analytics, and game features. Tokens expire after a set period (typically 2 hours) and must be refreshed.

Get server access token for Douyin mini-game API
- **get_analytics**: Useful for tracking game performance, understanding player retention, and identifying trends.

Get game analytics data (DAU, retention, etc.)
- **get_game_rank**: Supports different rank scenes (different leaderboards). Useful for showing players their standing and competitive position.

Get user's game rank and leaderboard data
- **get_user_info**: Requires the access token and openid obtained from code2session. Note: Some fields require explicit user authorization.

Get Douyin user profile information
- **get_user_storage**: Specify keys to fetch specific fields, or omit keys to fetch all stored data. Useful for loading saved game progress, settings, or user preferences.

Retrieve user data from Douyin cloud storage
- **remove_user_storage**: Use this to reset game progress, clear saved data, or remove outdated entries. Requires comma-separated list of keys to remove.

Remove specific keys from user cloud storage
- **set_user_storage**: Each key-value pair is a string. Max storage per user is limited. Use this to save game progress, settings, high scores, or user preferences. Requires user login signature for security.

Save user data to Douyin cloud storage (key-value)
- **submit_score**: The score is a numeric value. The rank_scene parameter identifies which leaderboard (default 1001). Scores are used for ranking and competitive features.

Submit a game score to the leaderboard


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Douyin Mini-Game** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get an access token and exchange login code 'abc123' for a user session."

**🤖 AI Agent:**
> ✅ Access token obtained. Login code exchanged successfully! User openid: tt_user_123. Session established.

---

**👤 You:**
> "Save game progress: level 15, score 5000, coins 200 for user tt_user_123."

**🤖 AI Agent:**
> ✅ Game data saved! Level 15, score 5000, coins 200 stored in cloud storage for tt_user_123. Data will persist across sessions.

---

**👤 You:**
> "Check if the nickname 'TestUser123' passes content moderation."

**🤖 AI Agent:**
> ✅ Content check passed! 'TestUser123' is safe to use as a nickname. No policy violations detected.


## Installation & Usage

To install and use the **Douyin Mini-Game** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/douyin-mini-game](https://vinkius.com/mcp/douyin-mini-game)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
