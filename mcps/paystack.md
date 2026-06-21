# Paystack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/paystack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage payments via Paystack — list transactions, verify payments, and manage customers directly from any AI agent.

## Description
Connect your **Paystack** account to any AI agent and take full control of your payment operations through natural conversation.

### What you can do

- **Transaction Management** — List all transactions, retrieve detailed metadata, and verify payment statuses using references.
- **Customer Oversight** — List and inspect customer profiles to understand their payment history and metadata.
- **Subscription Tracking** — Monitor active subscriptions and billing plans to maintain a clear view of recurring revenue.
- **Refunds & Transfers** — List recent refunds and outbound transfers to keep your financial records in sync.
- **Plan Management** — View all configured payment plans and their associated settings.

### How it works

1. Subscribe to this server
2. Enter your Paystack Secret Key (sk_...)
3. Start managing your payments from Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Owners** — quickly verify if a customer has paid for an order without leaving your chat interface.
- **Financial Analysts** — extract transaction lists and refund data for reconciliation tasks.
- **Support Teams** — look up customer payment histories to resolve billing inquiries faster.


## Available Tools
- **get_customer**: Get specific customer details
- **get_subscription**: Get specific subscription details
- **get_transaction**: Get details for a specific transaction
- **list_customers**: List all customers
- **list_plans**: List all payment plans
- **list_refunds**: List all refunds
- **list_subscriptions**: List all subscriptions
- **list_transactions**: List Paystack transactions
- **list_transfers**: List all transfers
- **verify_transaction**: Verify a transaction status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paystack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the status of transaction reference 'ref_789456'."

**🤖 AI Agent:**
> Transaction 'ref_789456' was successful. The customer paid 5,000 NGN on Oct 24, 2026.

---

**👤 You:**
> "List the last 5 customers registered in our Paystack account."

**🤖 AI Agent:**
> I've retrieved the latest customers. Here are the 5 most recent signups, including their names, emails, and Paystack customer codes.

---

**👤 You:**
> "How many active subscriptions do we currently have?"

**🤖 AI Agent:**
> You currently have 124 active subscriptions across various plans. Would you like a breakdown by plan type?


## ❓ FAQ

**Q: Can I verify if a payment was successful?**
Yes! Use the `verify_transaction` tool with the transaction reference. It will return the current status (e.g., success, failed, abandoned) and the amount paid.

**Q: How do I find a customer by their email?**
You can use the `get_customer` tool and provide the customer's email address as the identifier. It will fetch their profile, customer code, and associated metadata.

**Q: Does this support checking recurring subscriptions?**
Absolutely. Use the `list_subscriptions` and `get_subscription` tools to manage and monitor recurring billing for your customers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/paystack](https://vinkius.com/mcp/paystack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paystack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `paystack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paystack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paystack": {
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
