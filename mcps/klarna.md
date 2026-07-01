# Klarna MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/klarna)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage payment sessions, orders, and fulfillment via the Klarna REST API.

## Description
Connect your **Klarna** merchant account to any AI agent to automate your e-commerce payment and order management workflows. This MCP server enables your agent to interact with both the Klarna Payments API (checkout phase) and the Order Management API (post-purchase phase) directly from natural language.

### What you can do

- **Session Control** — Create and manage checkout sessions to obtain client tokens for your frontend
- **Order Placement** — Formally place orders using authorization tokens from your checkout widget
- **Payment Ingestion** — Capture authorized orders to trigger the actual payment from the customer
- **Financial Resolution** — Process full or partial refunds and cancel authorized but uncaptured orders
- **Logistics Integration** — Update shipping information and tracking numbers for existing orders
- **Data Oversight** — Retrieve detailed status, financial totals, and metadata for any Klarna order

### How it works

1. Subscribe to this server
2. Enter your Klarna API Key (Username), Shared Secret, and Region Domain
3. Start managing your payments and orders from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Operations** — Monitor order statuses and process captures/refunds via simple natural language commands
- **Financial Controllers** — Quickly audit payment sessions and transaction totals without logging into the portal
- **Developers** — Integrate Klarna's complex two-phase payment logic and status monitoring into your custom applications


## Available Tools (8)
- **capture_klarna_order**: Capture a formal order to trigger payment
- **create_payment_session**: Requires order amount, currency, and order lines (items).

Create a new Klarna payment session
- **get_order_details**: Get details for a specific Klarna order
- **get_payment_session**: Get details for an existing payment session
- **create_klarna_order**: Requires an authorization token.

Place a formal order using an authorization token
- **refund_klarna_order**: Refund a captured order
- **update_order_shipping**: Update shipping information for an order
- **cancel_authorized_order**: Cancel an authorized but uncaptured order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Klarna** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a Klarna payment session for $150.00 in USD."

**🤖 AI Agent:**
> I've initialized the session. The order amount is 15000 (cents). Here is your session ID: 'abc-123' and the client token for your frontend widget.

---

**👤 You:**
> "Show details for Klarna order ID '98765-XYZ'."

**🤖 AI Agent:**
> I've retrieved order 98765-XYZ. The current status is 'AUTHORIZED' and it has not been captured yet. The total amount is $150.00 USD.

---

**👤 You:**
> "Capture order '98765-XYZ' for the full amount of $150.00."

**🤖 AI Agent:**
> Successfully triggered capture for order 98765-XYZ. Klarna has processed the payment, and the status has been updated to 'CAPTURED'.


## ❓ FAQ

**Q: How do I determine my Klarna Region Domain?**
Use `api.klarna.com` for Europe, `api-na.klarna.com` for North America, or `api.playground.klarna.com` for testing/sandbox environments.

**Q: What is the difference between authorizing and capturing an order?**
Authorizing only reserves the funds. You must use the `capture_klarna_order` tool (typically when shipping) to actually move the money from the customer to your account.

**Q: Can I process partial refunds?**
Yes, the `refund_klarna_order` tool accepts a JSON object where you can specify the exact amount and the specific items being refunded.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/klarna](https://vinkius.com/mcp/klarna)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Klarna** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `klarna` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Klarna** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "klarna": {
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
