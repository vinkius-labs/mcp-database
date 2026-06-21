# AccelByte MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/accelbyte)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/accelbyte-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/accelbyte-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage game backend services via AccelByte — handle users, achievements, leaderboards, and orders directly from your AI agent.

## Description
Connect your **AccelByte** game backend to any AI agent to streamline player management and live ops through natural conversation.

### What you can do

- **User Management** — Create users, fetch detailed profiles, update account statuses, and manage bans across namespaces.
- **Social & Progress** — List player friends, unlock specific achievements, and retrieve real-time leaderboard rankings.
- **Commerce & Economy** — Manage user wallets, grant item entitlements, and create orders for in-game transactions.
- **IAM & Security** — Generate OAuth2 tokens and manage IAM clients for secure service-to-service communication.

### How it works

1. Subscribe to this server
2. Enter your AccelByte Base URL and Access Token
3. Start managing your game ecosystem from Claude, Cursor, or any MCP-compatible client

No more jumping between different admin dashboards to check player stats or fix entitlement issues. Your AI acts as a dedicated Live Ops assistant.

### Who is this for?

- **Game Developers** — quickly test backend logic or check user data without leaving the IDE
- **Live Ops Teams** — manage player bans, status updates, and entitlements through natural language
- **QA Engineers** — automate user creation and achievement unlocking for rapid testing cycles


## Available Tools
- **ban_user**: Ban a user
- **create_order**: Create a purchase order
- **create_user**: Create a new user in a namespace
- **delete_client**: Delete an IAM client
- **generate_token**: Generate an OAuth2 access token
- **get_leaderboard**: Get leaderboard rankings
- **get_user**: Get user details (Admin)
- **get_user_wallets**: Query user wallet
- **grant_entitlement**: Grant entitlement to user
- **list_friends**: List user friends
- **unlock_achievement**: Unlock an achievement
- **update_user_status**: g., enabling or disabling their account).

Update user status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AccelByte** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new user with email player1@example.com in the 'GameAlpha' namespace."

**🤖 AI Agent:**
> I've created the user in the 'GameAlpha' namespace. The new User ID is 'ab-98765' and the display name is set to 'player1'.

---

**👤 You:**
> "Show me the leaderboard rankings for code 'TOP_PLAYERS_2024' in namespace 'studio-1'."

**🤖 AI Agent:**
> Fetching rankings for 'TOP_PLAYERS_2024'... I've found the top players. 'SpeedyGamer' is currently in 1st place with 15,000 points.

---

**👤 You:**
> "Unlock achievement 'FIRST_BLOOD' for user 'user-777' in namespace 'game-v1'."

**🤖 AI Agent:**
> Processing... The achievement 'FIRST_BLOOD' has been successfully unlocked for user 'user-777'.


## Installation & Usage

To install and use the **AccelByte** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/accelbyte](https://vinkius.com/mcp/accelbyte)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
