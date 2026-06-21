# Vivo Game Open Platform MCP Server

Manage Vivo Game Open Platform distribution — validate logins, query orders, and report game data directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/vivo-game-open-platform)

## Overview
**Category:** industry-titans
**Tools Count:** 9

## Description
Connect your AI agents to the **Vivo Game Open Platform** (vivo 开放平台), the primary ecosystem for game distribution on Vivo mobile devices. This MCP provides 9 tools to automate server-to-server validation, payment tracking, and player data reporting for high-performance mobile and mini-games.

### What you can do

- **Authentication** — Validate user tokens and retrieve unique `openid` identifiers from the Vivo account service
- **Payment Orchestration** — Query real-time status for payment orders and reconcile transactions programmatically
- **Game Analytics** — Report player progress, high scores, and level data to the Vivo Game Center rankings
- **Role Management** — Update character/role information including names, levels, and server assignments
- **App Configuration** — Fetch current application settings and list active game servers from the developer console

### How it works

1. Subscribe to this server
2. Log in to the [**Vivo Developer Console**](https://dev.vivo.com.cn/)
3. Navigate to **Game Management** and select your active project
4. Copy your **AppID**, **AppKey**, and **AppSecret** from the basic information page
5. Insert your credentials into the fields below to start managing your Vivo gaming distribution backend.

### Who is this for?

- **Mobile Game Developers** — automate server-side login verification and payment delivery logic
- **Live Operations Teams** — monitor order statuses and player ranking integrity in the Vivo ecosystem
- **Backend Engineers** — integrate Vivo platform features into centralized game management dashboards


## Available Tools
- **get_app_config**: Retrieve application configuration from Vivo platform
- **get_server_time**: Synchronize with Vivo platform server time
- **get_user_info**: Retrieve basic profile data for a Vivo user
- **list_game_servers**: Query the list of game servers
- **list_items**: Query available virtual items for the app
- **query_order**: Check the status of a specific payment order
- **report_game_data**: Submit player progress and scores to Vivo Game Center
- **report_role_info**: Report character or role information
- **validate_login**: Verify a user login token from Vivo SDK


## Installation & Usage

To install and use the **Vivo Game Open Platform** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vivo-game-open-platform](https://vinkius.com/mcp/vivo-game-open-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
