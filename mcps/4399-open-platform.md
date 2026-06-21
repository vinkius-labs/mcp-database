# 4399 Open Platform MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/4399-open-platform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/4399-open-platform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/4399-open-platform-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Manage 4399 Open Platform game distribution — validate logins, query orders, and handle leaderboards directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **4399 Open Platform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the status of 4399 order ID 'order_999888777'."

**🤖 AI Agent:**
> Running order query... I've retrieved the details for transaction 'order_999888777'. The current status is 'completed' for an amount of 50.00 CNY. Would you like me to log this transaction status?

---

**👤 You:**
> "Validate login for 4399 user 'uid_123' with token 'tok_abc'."

**🤖 AI Agent:**
> Connecting to 4399 authentication server... Validation successful! User 'uid_123' is correctly logged in. Session remains valid for the next 2 hours.

---

**👤 You:**
> "Check if the text 'offensive word' is allowed by 4399 policy."

**🤖 AI Agent:**
> Scanning content... The sensitive word filter flagged 1 term in your input. It is recommended to reject this content for role names or public chat.


## Installation & Usage

To install and use the **4399 Open Platform** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/4399-open-platform](https://vinkius.com/mcp/4399-open-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
