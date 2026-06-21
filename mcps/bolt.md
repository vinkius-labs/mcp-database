# Bolt MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bolt)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage your one-click checkout and payments via Bolt — track transactions, manage orders, and process refunds directly from any AI agent.

## Description
Connect your **Bolt Merchant** account to any AI agent and orchestrate your checkout and payment workflows through natural conversation.

### What you can do

- **Transaction Oversight** — List recent Bolt transactions and retrieve detailed metadata for individual payments.
- **Payment Lifecycle Management** — Capture authorized transactions, void pending ones, and issue full or partial refunds.
- **Order Token Generation** — Create order tokens to initiate secure one-click checkout sessions.
- **Shopper Intelligence** — Retrieve account details and order history for authenticated shoppers.
- **Webhook Monitoring** — List and audit configured webhooks to ensure real-time data sync.
- **Merchant Health Check** — Retrieve the current status and configuration of your merchant account.

### How it works

1. Subscribe to this server
2. Enter your Bolt Private API Key and Environment (api or api-sandbox)
3. Start managing your checkout experience from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Operations** — quickly check payment statuses and process refunds without manual dashboard work.
- **Customer Support** — retrieve transaction details and order history straight from their workflow tools.
- **Developers** — verify API integrations and order token generation using natural language.


## Available Tools
- **capture_transaction**: Capture a previously authorized transaction
- **create_order_token**: Create an order token to initiate checkout
- **get_account_details**: Get current account details
- **get_merchant_status**: Check the current merchant account status
- **get_order_details**: Get details of a specific order
- **get_transaction**: Get details of a specific transaction
- **list_transactions**: List recent Bolt transactions
- **list_webhooks**: List configured webhooks
- **refund_transaction**: Issue a refund for a completed transaction
- **void_transaction**: Void an authorized but uncaptured transaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bolt** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 transactions in my Bolt account."

**🤖 AI Agent:**
> I've retrieved your recent transactions. Notable entries include a $45.00 charge (Ref: ABC-123) and a $120.00 authorization (Ref: XYZ-789). Would you like full details for any of them?

---

**👤 You:**
> "Refund $20.00 for transaction reference ABC-123."

**🤖 AI Agent:**
> I've initiated a partial refund of $20.00 (2000 cents) for transaction ABC-123. The credit process has started in your Bolt merchant account.

---

**👤 You:**
> "Check the status of my Bolt merchant account."

**🤖 AI Agent:**
> Your merchant account is currently 'Active' and all configurations are valid. Your publishable key ends in '...xyz' and your division ID is 'div_123'.


## ❓ FAQ

**Q: Can I process a refund for a transaction using the agent?**
Yes! Use the `refund_transaction` tool with the Bolt reference ID and the amount in cents. Your agent will initiate the credit transaction in your Bolt account.

**Q: How do I check the status of a specific Bolt transaction?**
Simply ask the agent to `get_transaction` and provide the reference ID. It will retrieve the latest status, such as 'Authorized', 'Completed', or 'Failed', directly from Bolt.

**Q: Can I use this to generate a checkout session token?**
Yes. Use the `create_order_token` tool and provide the cart details in JSON format. This will return a token that can be used on your frontend to open the Bolt checkout modal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bolt](https://vinkius.com/mcp/bolt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bolt** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bolt` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bolt** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bolt": {
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
