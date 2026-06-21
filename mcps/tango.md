# Tango MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tango)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Document any process by recording your screen clicks and turning them into step-by-step guides with annotated screenshots.

## Description
Connect your **Tango (formerly Tango Card)** reward platform account to any AI agent and simplify how you distribute digital gift cards, manage customers, and monitor funding accounts through natural conversation.

### What you can do

- **Catalog Discovery** — Browse the full global catalog of brands, including gift cards, prepaid cards, and non-profit donations.
- **Reward Distribution** — Place and automate orders for digital rewards delivered via email instantly.
- **Customer & Account Management** — List, create, and manage customer groups and their associated funding accounts.
- **Financial Oversight** — Check real-time account balances, list funding sources, and retrieve current exchange rates.
- **Order Tracking** — Monitor your reward history and fetch detailed status and credentials for specific order IDs.
- **Scalable Rewards** — Coordinate bulk payouts and loyalty incentives directly from Claude, Cursor, or any MCP client.

### How it works

1. Subscribe to this server
2. Enter your Tango Platform Name and Platform Key
3. Start managing your digital reward ecosystem from your favorite AI assistant

### Who is this for?

- **HR & Culture Managers** — quickly send employee recognition rewards and verify account balances via simple AI commands.
- **Marketing & Loyalty Teams** — automate the distribution of campaign incentives and browse brand availability directly from the workspace.
- **Operations Leads** — monitor order histories and manage customer group funding via the AI assistant.


## Available Tools (12)
- **create_account**: Create a new funding account
- **create_customer**: Create a new customer
- **create_order**: Place a reward order
- **get_account**: Get account balance
- **get_catalog**: List available reward brands
- **get_customer**: Get customer details
- **get_exchange_rates**: Get currency exchange rates
- **get_order**: Get order status
- **list_accounts**: List accounts for a customer
- **list_customers**: List all customers
- **list_funding_sources**: List funding sources
- **list_orders**: List recent orders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tango** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all available gift card brands in the catalog."

**🤖 AI Agent:**
> I've retrieved the global catalog. You have access to hundreds of brands including Amazon, Starbucks, Apple, and Target. Which country or category are you interested in?

---

**👤 You:**
> "What is the current balance of account 'acc_10293'?"

**🤖 AI Agent:**
> Fetching balance... The account 'acc_10293' currently has a balance of $1,250.00 USD. You have sufficient funds for your upcoming reward distributions.

---

**👤 You:**
> "Send a $25 Amazon gift card (UTID: AMZN-US-2500) to 'john.doe@example.com'."

**🤖 AI Agent:**
> Order initiated! I've triggered the delivery of a $25.00 Amazon reward to john.doe@example.com. The order ID is ord_88231. I'll let you know once the status shows it's successfully delivered.


## ❓ FAQ

**Q: Can I see my current account balance via AI?**
Yes! Use the `get_account` tool and provide the Account Identifier. Your agent will retrieve the current balance and available funds for that specific funding account.

**Q: How do I find the correct ID (UTID) for a specific gift card brand?**
Run the `get_catalog` query. The agent will retrieve the full list of available brands and items, each with its unique UTID required for placing orders.

**Q: Is it possible to track if a reward has been delivered?**
Absolutely. Use the `get_order` tool and provide the Order ID. The agent will retrieve the status, delivery details, and even the credentials if the reward is ready.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tango](https://vinkius.com/mcp/tango)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tango** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tango` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tango** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tango": {
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
