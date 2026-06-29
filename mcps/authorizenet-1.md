# Authorize.net MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/authorizenet-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage payments, transactions, and customer profiles via Authorize.net — the trusted payment gateway directly via AI.

## Description
Connect your **Authorize.net** merchant account to any AI agent and manage your entire payment lifecycle through natural conversation.

### What you can do

- **Transaction Management** — Authorize, capture, refund, and void transactions with full audit trails and security
- **Financial Reporting** — List transactions from settled batches, unsettled queues, and analyze processing performance
- **Customer Profiles** — Retrieve and manage secure customer payment information and subscription profiles
- **Batch Insights** — Monitor daily settlement statistics and high-level performance metrics for your merchant account

### How it works

1. Subscribe to this server
2. Enter your Authorize.net API Login ID and Transaction Key
3. Start managing your payments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance Teams** — audit recent transactions, check settlement statuses, and process refunds without manual dashboard navigation
- **E-commerce Managers** — monitor payment health and manage customer billing profiles directly from their workspace
- **Developers** — test payment flows in sandbox and audit transaction metadata through natural language commands


## Available Tools (10)
- **get_batch_statistics**: Get statistics for a specific batch
- **create_transaction**: You must provide the transaction type (e.g., authCaptureTransaction) and the request body.

Create a new payment transaction
- **get_customer_profile**: Retrieve a customer profile by ID
- **get_settled_batch_list**: Retrieve a list of settled batches for a date range
- **get_transaction_details**: Get complete information for a specific transaction
- **get_transaction_list**: List transactions for a specific settled batch
- **get_unsettled_transaction_list**: List the most recent unsettled transactions
- **list_customer_profiles**: Retrieve a list of all customer profile IDs
- **refund_transaction**: Refund a settled transaction
- **void_transaction**: Void an unsettled transaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Authorize.net** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent unsettled transactions."

**🤖 AI Agent:**
> I've scanned your unsettled queue. I found 3 transactions waiting for settlement, including an authCapture for $120.00 (ID: 6012345678) and a refund for $45.00. Would you like the full details for any of these?

---

**👤 You:**
> "Refund $50.00 for transaction ID '123456789'."

**🤖 AI Agent:**
> Processing refund... Success! The transaction '123456789' has been partially refunded for $50.00. The reference ID for this refund is 6022345679.

---

**👤 You:**
> "Show the settlement statistics for the last closed batch."

**🤖 AI Agent:**
> Retrieving batch stats... The last closed batch (ID: 12345) had 45 transactions totaling $5,240.50 settled. There were 2 voids and 1 refund processed in this period.


## ❓ FAQ

**Q: Can the AI automatically process a refund for a specific transaction ID?**
Yes! Use the `create_transaction` tool with the 'refundTransaction' type. You'll need to provide the original transaction ID and the amount to be credited back to the customer.

**Q: How do I check for transactions that have not yet been settled?**
Simply ask the agent to run the `get_unsettled_transaction_list` tool. It will return all transactions currently sitting in your unsettled queue for review.

**Q: Is it possible to manage customer payment profiles securely through the AI?**
Yes. The `get_customer_profile` tool allows the agent to retrieve stored profiles (without exposing full sensitive card data), enabling you to manage recurring billing and saved information securely.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/authorizenet-1](https://vinkius.com/mcp/authorizenet-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Authorize.net** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `authorizenet-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Authorize.net** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "authorizenet-1": {
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
