# Zenedu MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zenedu)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage messenger bots, funnels, and subscribers via Zenedu.

## Description
Connect your **Zenedu** account to any AI agent to automate your messenger marketing and sales funnels. This MCP server enables your agent to interact with bots, products, offers, and subscriber data directly.

### What you can do

- **Bot Oversight** — List all your messenger bots and their associated metadata
- **Funnel Tracking** — List and monitor sales funnels and automation flows for specific bots
- **Commerce Management** — Access product catalogs and marketing offers synchronized with your bots
- **Order Visibility** — Retrieve recent customer orders and transaction statuses
- **Audience Insight** — List and query subscribers to track growth and engagement

### How it works

1. Subscribe to this server
2. Enter your Zenedu API Token
3. Start managing your messenger marketing from Claude, Cursor, or any MCP client

### Who is this for?

- **Digital Marketers** — Monitor bot performance and funnel statuses on the fly
- **E-commerce Owners** — Quickly check recent orders and product offerings via natural language
- **Customer Success Teams** — Retrieve subscriber information and bot interactions effortlessly


## Available Tools
- **list_bots**: List all messenger bots
- **list_bot_funnels**: List all funnels for a specific bot
- **list_bot_offers**: List all offers for a specific bot
- **list_bot_orders**: List all orders for a specific bot
- **list_bot_products**: List all products for a specific bot
- **list_bot_subscribers**: List all subscribers for a specific bot


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zenedu** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all messenger bots in my Zenedu account."

**🤖 AI Agent:**
> I've retrieved your bots. You have 3 active bots: 'Main Funnel', 'Support Bot', and 'Flash Sale Assistant'. Would you like to see the funnels for any of them?

---

**👤 You:**
> "Show me the funnels for bot ID '12345'."

**🤖 AI Agent:**
> For bot 12345, I found 2 active funnels: 'Welcome Flow' and 'Abandoned Cart Recovery'.

---

**👤 You:**
> "List recent orders for my 'Main Funnel' bot."

**🤖 AI Agent:**
> I've fetched the orders. There are 5 recent transactions, including Order #ZEN-987 for $49.00 and Order #ZEN-986 for $25.50.


## ❓ FAQ

**Q: How do I find my Bot ID?**
Use the `list_bots` tool to see a comprehensive list of all bots in your account along with their unique IDs.

**Q: Can I see recent orders for a specific bot?**
Yes, the `list_bot_orders` tool retrieves recent customer transactions and their current status for a target bot.

**Q: Is it possible to list subscribers via the agent?**
Absolutely. Use the `list_bot_subscribers` tool with a bot ID to see the users who have interacted with your messenger bot.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zenedu](https://vinkius.com/mcp/zenedu)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zenedu** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zenedu` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zenedu** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zenedu": {
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
