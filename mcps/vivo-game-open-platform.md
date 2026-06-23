# Vivo Game Open Platform MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vivo-game-open-platform)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage Vivo Game Open Platform distribution — validate logins, query orders, and report game data directly from any AI agent.

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


## Available Tools (9)
- **get_app_config**: Retrieve application configuration from Vivo platform
- **get_server_time**: Synchronize with Vivo platform server time
- **get_user_info**: Retrieve basic profile data for a Vivo user
- **list_game_servers**: Query the list of game servers
- **list_items**: Query available virtual items for the app
- **query_order**: Check the status of a specific payment order
- **report_game_data**: Submit player progress and scores to Vivo Game Center
- **report_role_info**: Report character or role information
- **validate_login**: Verify a user login token from Vivo SDK


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vivo Game Open Platform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the status of Vivo order ID 'cp_order_555666'."

**🤖 AI Agent:**
> Connecting to Vivo payment servers... I've retrieved the details for order 'cp_order_555666'. The current status is 'success' for an amount of 10.00 CNY. The transaction is ready for virtual item delivery.

---

**👤 You:**
> "Validate the login token 'tok_vivo_abc' from the client."

**🤖 AI Agent:**
> Requesting validation from Vivo Auth... Success! The token is valid and corresponds to OpenID: `user_888999`. You can now proceed with the user's game session.

---

**👤 You:**
> "List all active game servers configured in the Vivo console."

**🤖 AI Agent:**
> Retrieving server list... I found 3 active servers: 1. Asia-East (ID: srv_1), 2. Global-South (ID: srv_2), 3. Test-Net (ID: srv_3). All are currently 'online'.


## ❓ FAQ

**Q: How do I validate a Vivo login token from my backend?**
Use the `validate_login` tool with the user's token provided by the Vivo SDK. The agent will connect to the Vivo verification server and return the `openid` if the session is legitimate.

**Q: Can I automatically query the status of a specific order?**
Yes! Use the `query_order` tool with your CP Order ID. Your agent will retrieve the payment status, amount, and internal transaction reference directly from the Vivo gateway.

**Q: How do I report character role information to the platform?**
Use the `report_role_info` tool with a JSON string containing the character details (name, level, server). This is essential for compliance and social features within the Vivo ecosystem.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vivo-game-open-platform](https://vinkius.com/mcp/vivo-game-open-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vivo Game Open Platform** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vivo-game-open-platform` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vivo Game Open Platform** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vivo-game-open-platform": {
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
