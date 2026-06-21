# 4399 Open Platform MCP Server

Manage 4399 Open Platform game distribution — validate logins, query orders, and handle leaderboards directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/4399-open-platform)

## Overview
**Category:** security
**Tools Count:** 9

## Description
Connect your AI agents to the **4399 Open Platform** (4399开放平台), the leading ecosystem for game distribution in China. This MCP provides 10 tools to automate server-side validation, payment tracking, and community features for H5 and mobile games.

### What you can do

- **Authentication** — Validate user sessions and access tokens returned by the client-side SDK
- **Payment Tracking** — Query real-time status for recharge orders and transaction details
- **User Profiling** — Retrieve basic player information and registration metadata for specific UIDs
- **Game Integrity** — Use the sensitive words API to filter prohibited content in role names and chat
- **Social & Competitive** — Manage global leaderboards, submit scores, and list user social circles

### How it works

1. Subscribe to this server
2. Log in to the [**4399 Open Platform Console**](http://open.4399.cn/)
3. Navigate to **Game Management** and select your active project
4. Copy your **AppKey (GameID)** and **Secret**
5. Insert your credentials into the fields below to start orchestrating your game distribution backend.

### Who is this for?

- **Game Developers** — automate server-to-server validation and payment reconciliation
- **Live Ops Teams** — monitor leaderboard integrity and player social trends
- **Backend Engineers** — integrate 4399 platform features into custom management dashboards


## Available Tools
- **check_sensitive_words**: Filter content for prohibited or sensitive terms
- **get_game_status**: Check current operational status of the game
- **get_leaderboard**: Fetch the top players list
- **get_server_time**: Get the current 4399 server timestamp
- **get_user_info**: Retrieve basic profile for a user
- **list_friends**: List friends for a 4399 user
- **query_order**: Check the status of a payment order
- **submit_score**: Submit a new record to a leaderboard
- **validate_login**: Verify a user login session


## Installation & Usage

To install and use the **4399 Open Platform** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/4399-open-platform](https://vinkius.com/mcp/4399-open-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
