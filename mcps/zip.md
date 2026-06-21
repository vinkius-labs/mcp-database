# Zip MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zip)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage BNPL checkouts, orders, and payments via the Zip (Quadpay) REST API.

## Description
Connect your **Zip** (formerly Quadpay) merchant account to any AI agent to automate your Buy Now, Pay Later (BNPL) workflows. This MCP server enables your agent to initiate checkouts, manage order authorizations, and process captures or refunds directly from natural language interfaces.

### What you can do

- **Checkout Initiation** — Create new checkout sessions and retrieve redirect URLs for customers
- **Order Management** — Authorize and confirm orders across US and Global gateway environments
- **Payment Ingestion** — Capture authorized funds once goods are shipped to finalize transactions
- **Financial Resolution** — Process full or partial refunds and void authorized but uncaptured payments
- **Status Monitoring** — Retrieve real-time status and lifecycle updates for any Zip order
- **Account Insight** — Access merchant configuration, currency limits, and account-level settings

### How it works

1. Subscribe to this server
2. Enter your Zip Merchant API Key, Region, and Environment (Sandbox/Production)
3. Start managing your BNPL payments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Operations** — Monitor order lifecycles and process captures/refunds via simple natural language commands
- **Financial Controllers** — Quickly audit transaction statuses and merchant configurations without opening the portal
- **Developers** — Integrate BNPL checkout logic and status monitoring into your custom applications


## Available Tools (8)
- **authorize_zip_order**: Typically used in US gateway integrations.

Authorize a payment order
- **capture_zip_payment**: Capture funds for an authorized order
- **confirm_zip_order**: Finalize an authorized order
- **create_zip_checkout**: Requires amount, currency, and redirect URLs.

Initialize a new Zip checkout session
- **get_zip_merchant_config**: Retrieve merchant account configuration
- **get_zip_order_status**: g., Authorized, Captured, Cancelled) for a target order.

Check the status of a Zip order
- **refund_zip_payment**: Process a refund for an order
- **void_zip_payment**: Void an authorized but uncaptured payment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zip** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a Zip checkout for $100.00 USD."

**🤖 AI Agent:**
> I've initialized the Zip checkout for $100.00. Here is your checkout ID: 'chk-abc-123' and the redirect URL for the customer to complete payment.

---

**👤 You:**
> "Check the status of Zip order ID '98765'."

**🤖 AI Agent:**
> I've retrieved the status for order 98765. It is currently in the 'Authorized' state and is awaiting capture. The total amount is $100.00 USD.

---

**👤 You:**
> "Capture payment for authorized order '98765'."

**🤖 AI Agent:**
> Successfully triggered the capture for order 98765. The funds have been processed, and the order state has been updated to 'Captured'.


## ❓ FAQ

**Q: What is the difference between Authorize and Confirm in Zip?**
Authorize initiates the transaction and checks for customer funds. Confirm (used in some regions) finalizes the checkout intent before capture.

**Q: Can I process partial captures via the agent?**
Yes, the `capture_zip_payment` tool accepts an optional JSON body where you can specify a partial amount to capture if only part of the order is shipping.

**Q: How do I handle different regions like US and AU?**
Specify your account region ('US' or 'AU') in the configuration settings. The MCP server automatically routes requests to the correct Zip gateway URL.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zip](https://vinkius.com/mcp/zip)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zip** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zip` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zip** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zip": {
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
