# Dynamic (Web3 Auth) MCP Server

Manage Web3 authentication and user data via Dynamic — fetch user profiles, check wallet sanctions, and manage sessions directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dynamic-web3-auth)

## Overview
**Category:** security-compliance
**Tools Count:** 8

## Description
Connect your **Dynamic** environment to any AI agent to streamline Web3 user management and security workflows through natural conversation.

### What you can do

- **User Management** — Fetch detailed user profiles or permanently delete users from specific environments using `get_user` and `delete_user`.
- **Security & Compliance** — Use `check_sanctions` to verify if specific wallet addresses are sanctioned across multiple chains (ETH, SOL, EVM, etc.).
- **Session Control** — Instantly terminate active user sessions with `revoke_session` to maintain environment security.
- **Infrastructure Monitoring** — List active embedded wallet versions and configured webhooks to audit your auth setup.
- **Financial Insights** — Retrieve real-time token balances for users across different networks using `get_token_balances`.

### How it works

1. Subscribe to this server
2. Enter your Dynamic API Token
3. Start managing your Web3 auth layer from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug user profiles and check token balances directly from your code editor.
- **Security & Ops Teams** — Audit wallet sanctions and revoke suspicious sessions instantly without opening the dashboard.
- **Product Managers** — Monitor webhook configurations and available event types to coordinate feature releases.


## Available Tools
- **check_sanctions**: Check wallet sanctions
- **delete_user**: Delete a user from an environment
- **get_embedded_wallet_versions**: Get active embedded wallet versions
- **get_event_types**: Get available event types
- **get_token_balances**: Get token balances for a user
- **get_user**: Get a user by ID in an environment
- **get_webhooks**: Get configured webhooks
- **revoke_session**: Revoke an active user session


## Installation & Usage

To install and use the **Dynamic (Web3 Auth)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dynamic-web3-auth](https://vinkius.com/mcp/dynamic-web3-auth)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
