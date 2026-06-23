# BlueSnap MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bluesnap)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Process and manage payments via BlueSnap — list transactions, subscriptions, and vaulted shoppers directly from any AI agent.

## Description
Connect your **BlueSnap** merchant account to any AI agent and orchestrate your global payment and subscription workflows through natural conversation.

### What you can do

- **Transaction Oversight** — List and retrieve detailed information for recent payments and card authorizations.
- **Subscription Management** — Query and monitor active recurring billing subscriptions and plans.
- **Vaulted Shopper Analysis** — Access saved shopper profiles to understand customer retention and history.
- **Marketplace Coordination** — List and verify vendors managed within your BlueSnap marketplace.
- **Payout Insights** — Check real-time account balances and pending payouts.
- **Detailed Auditing** — Retrieve specific data for any transaction or subscription ID.

### How it works

1. Subscribe to this server
2. Enter your BlueSnap API Username, Password, and Environment (ws or sandbox)
3. Start managing your global payments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Ops** — quickly check transaction statuses and shopper details without manual dashboard searches.
- **Finance Teams** — monitor payout balances and subscription plans straight from their workflow tools.
- **Developers** — verify transaction metadata and sandbox activity using natural language.


## Available Tools (10)
- **get_account_balance**: Check current payout balances
- **get_plan**: Get specific plan details
- **get_subscription**: Get specific subscription details
- **get_transaction**: Get specific transaction details
- **get_vaulted_shopper**: Get specific vaulted shopper details
- **list_plans**: List all recurring billing plans
- **list_subscriptions**: List all active subscriptions
- **list_transactions**: List recent payment transactions
- **list_vaulted_shoppers**: List all vaulted shoppers
- **list_vendors**: List all marketplace vendors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BlueSnap** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 payment transactions."

**🤖 AI Agent:**
> I've retrieved your recent transactions. Notable entries include a $50.00 charge (ID: tx_123) and a €25.00 authorization (ID: tx_456). Which one would you like to inspect?

---

**👤 You:**
> "Check the status of subscription sub_99283."

**🤖 AI Agent:**
> Subscription sub_99283 is currently 'Active'. The next billing date is April 15th for an amount of $19.99.

---

**👤 You:**
> "Show my current account balance."

**🤖 AI Agent:**
> Retrieving balance... Your current payout balance is $1,250.40 USD and €450.00 EUR. There are no pending payout issues.


## ❓ FAQ

**Q: Can I check the status of a specific payment transaction?**
Yes! Use the `get_transaction` tool with the Transaction ID. Your agent will fetch the latest status, including whether it is 'Success', 'Pending', or 'Failed'.

**Q: How do I list all my active subscription plans?**
Simply ask the agent to `list_plans`. It will retrieve all recurring billing plans configured in your BlueSnap account for you to review.

**Q: Does the integration allow processing a new refund?**
Currently, the toolset is focused on querying and monitoring (Read-Only). You can list and inspect transactions, but processing refunds or charges must be done through the BlueSnap portal for financial security.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bluesnap](https://vinkius.com/mcp/bluesnap)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BlueSnap** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bluesnap` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BlueSnap** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bluesnap": {
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
