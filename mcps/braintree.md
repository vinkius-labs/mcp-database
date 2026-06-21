# Braintree MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/braintree)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Process and manage payments via Braintree GraphQL API — search transactions, manage customers, and issue refunds directly from any AI agent.

## Description
Connect your **Braintree** gateway account to any AI agent and orchestrate your global payment and checkout workflows through natural conversation.

### What you can do

- **Transaction Oversight** — Search and list recent transactions or retrieve detailed metadata for specific payments.
- **Payment Lifecycle Management** — Charge payment methods, capture authorized funds, void pending transactions, and issue full or partial refunds.
- **Customer Data Orchestration** — Search your customer vault by email and retrieve detailed billing profiles and saved payment methods.
- **GraphQL Power** — Leverage the flexibility of Braintree's modern GraphQL API for precise data retrieval.

### How it works

1. Subscribe to this server
2. Enter your Braintree Public Key, Private Key, and Environment (sandbox or production)
3. Start managing your payments from Claude, Cursor, or any MCP-compatible client


## Available Tools (8)
- **capture_transaction**: Capture an authorized transaction
- **charge_payment_method**: Charge a payment method
- **get_customer**: Get details of a specific customer
- **get_transaction**: Get details of a specific transaction
- **refund_transaction**: Optionally provide a partial amount.

Refund a settled transaction
- **search_customers**: Search for customers
- **search_transactions**: Search for recent transactions
- **void_transaction**: Void an authorized transaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Braintree** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for recent transactions in Braintree."

**🤖 AI Agent:**
> I've retrieved your recent transactions. Notable entries include a $45.00 charge (Status: SETTLED) and a $120.00 authorization (Status: AUTHORIZED). Would you like to capture the authorized one?

---

**👤 You:**
> "Find the customer profile for john@example.com."

**🤖 AI Agent:**
> I found the customer. Name: John Doe. Legacy ID: 554321. The profile is active in your Braintree vault.

---

**👤 You:**
> "Refund $20.00 for transaction ID TX_NODE_123."

**🤖 AI Agent:**
> I've successfully initiated a partial refund of $20.00 for transaction TX_NODE_123. The refund status is currently 'SUBMITTED_FOR_SETTLEMENT'.


## ❓ FAQ

**Q: Can I process a refund for a transaction using the agent?**
Yes! Use the `refund_transaction` tool with the Transaction Node ID. You can also specify a partial amount if you don't want to refund the full charge.

**Q: How do I capture a previously authorized transaction?**
Simply ask the agent to `capture_transaction` and provide the Transaction Node ID. The funds will be captured and the status updated in your Braintree account.

**Q: Does the integration allow searching for a customer by email?**
Yes. Use the `search_customers` tool and provide the exact email address. The agent will execute a GraphQL query to find the matching customer profile.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/braintree](https://vinkius.com/mcp/braintree)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Braintree** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `braintree` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Braintree** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "braintree": {
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
