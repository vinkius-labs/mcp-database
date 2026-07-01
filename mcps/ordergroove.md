# Ordergroove MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ordergroove)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Subscription management for eCommerce — manage recurring orders and customer loyalty via Ordergroove.

## Description
Connect your **Ordergroove** account to empower your AI agents with advanced subscription management capabilities. This server provides programmatic access to the Ordergroove REST API for managing the full subscription lifecycle.

### What you can do

- **Subscription Control** — List, inspect, update, cancel, or reactivate subscriptions instantly
- **Customer Insights** — Access detailed customer profiles and subscription history
- **Product Catalog** — Monitor synced products and their availability for recurring orders
- **Flexible Scheduling** — Modify quantities, frequencies, and next order dates through simple commands
- **Lifecycle Management** — Automate retention workflows and customer support tasks using natural language

### How it works

1. Subscribe to this server
2. Enter your **Ordergroove API Key** from your settings panel
3. Start managing your recurring revenue from Claude, Cursor, or any MCP client


## Available Tools (9)
- **list_customers**: List Ordergroove customers
- **list_products**: List Ordergroove products
- **list_subscriptions**: You can filter by customer_id or status.

List Ordergroove subscriptions
- **reactivate_subscription**: Reactivate a cancelled subscription
- **update_subscription**: Update subscription details
- **cancel_subscription**: Requires a reason.

Cancel a subscription
- **get_customer**: Get customer details
- **get_product**: Get product details
- **get_subscription**: Get details for a specific subscription


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ordergroove** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List active subscriptions for customer 'cust_123'."

**🤖 AI Agent:**
> Fetching subscriptions... I've found 2 active recurring orders for this customer.

---

**👤 You:**
> "Cancel subscription #sub_abc because the customer requested a refund."

**🤖 AI Agent:**
> Processing cancellation... Success! Subscription #sub_abc is now cancelled with reason: 'Refund Requested'.


## ❓ FAQ

**Q: How do I get an Ordergroove API Key?**
Log in to your Ordergroove Dashboard, navigate to Settings > API Keys, and generate a new key.

**Q: What is the Subscription Public ID?**
It is the unique alphanumeric identifier for a subscription, typically found in the URL or the subscriptions list response.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ordergroove](https://vinkius.com/mcp/ordergroove)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ordergroove** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ordergroove` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ordergroove** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ordergroove": {
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
