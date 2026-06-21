# OpenCart MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opencart)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-operations](../categories/business-operations.md)

Connect your OpenCart store to AI agents — browse products, manage orders, track customers, and update fulfillment status through natural conversation.

## Description
Turn your **OpenCart** e-commerce backend into an AI-powered command center. Browse your product catalog, check order details, look up customers, and push status updates — without logging into the admin panel.

### What you can do

- **Product Catalog** — List all products or fetch a specific product with pricing, stock status, SEO tags, and linked categories
- **Order Management** — Browse orders with totals, payment methods, and shipping addresses. Get detailed line-items for any order by ID
- **Order Status Updates** — Push status transitions (Processing, Shipped, Complete, Cancelled) with comments via the order history endpoint
- **Customer Profiles** — List registered customers or fetch full details including addresses, custom fields, and newsletter status
- **Categories** — View your product category hierarchy and navigation structure
- **Cart Inspection** — Check the current API session cart contents for programmatic checkout workflows

### How it works

1. Subscribe to this server
2. Enter your OpenCart Store URL, API Username, and API Key
3. Start managing your store from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Store owners** — check daily orders and revenue without opening the admin panel
- **Support teams** — look up customer orders instantly during live chat support
- **Fulfillment ops** — update order statuses in bulk by talking to your AI agent instead of clicking through forms


## Available Tools
- **list_products**: Fetches active products, retrieving metadata such as prices, stock status, and basic SEO tags mapped inside the OpenCart product repository.

List OpenCart products using the native OpenCart API
- **get_product**: Get OpenCart product by ID. Returns full details
- **list_orders**: List OpenCart orders using the native API
- **get_order**: Get OpenCart order details by explicit ID
- **get_order_history**: g., Pending, Processing, Shipped). Use to verify tracking logic or administrative fulfillment changes.

Get OpenCart order status history by ID
- **list_customers**: List OpenCart registered customers
- **get_customer**: Get OpenCart customer full details by explicit ID
- **list_categories**: List OpenCart product category schemas
- **add_order_history**: Push updates like marking a shipment Complete or Canceled.

Add OpenCart order history / mutate order active status
- **get_cart**: Primarily used to verify product mapping prior to custom order creation logic.

Get current API session cart contents in OpenCart


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenCart** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all orders placed this week with their totals."

**🤖 AI Agent:**
> Found 23 orders this week totaling $4,850. Top order: #1247 — $620 (3 items, paid via Stripe, status: Processing). 18 orders are Complete, 3 Processing, and 2 Pending. Want me to pull the details for the pending ones?

---

**👤 You:**
> "Mark order #1052 as shipped with tracking number TRK-9876."

**🤖 AI Agent:**
> Done. Order #1052 status updated to 'Shipped' with comment: 'Tracking: TRK-9876'. The customer will receive an email notification if your store has that enabled. Want me to check the other pending orders?

---

**👤 You:**
> "Look up customer #42 and show me their full profile."

**🤖 AI Agent:**
> Customer #42: Sarah Johnson (sarah@example.com). Registered: Jan 15, 2024. Newsletter: subscribed. Default address: 456 Oak Ave, Portland, OR 97201. 12 orders placed, total lifetime value: $2,340. Last order: March 28 (#1241). Want me to pull that order's details?


## ❓ FAQ

**Q: Can my AI agent update order statuses — like marking an order as shipped?**
Yes. The add_order_history tool pushes a new status entry to any order. Provide the order ID, the OpenCart status ID (e.g., 3 for Shipped), and an optional comment. The status change appears immediately in the admin panel and triggers any configured email notifications.

**Q: Does it work with any OpenCart version?**
This integration uses the native OpenCart REST API available in OpenCart 2.x and later. If your store is running OpenCart 1.x, the API endpoints won't be available. For OpenCart 3.x and 4.x, the API user setup is the same — just ensure the API user is enabled in System > Users > API.

**Q: What about IP restrictions — will the API reject requests?**
OpenCart's API enforces an IP whitelist by default. When creating your API user, add the IP address of your server to the 'IP Addresses' tab. If you're running through a cloud proxy, add that proxy's IP. Without this step, all API requests will be rejected with a permission error.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opencart](https://vinkius.com/mcp/opencart)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenCart** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `opencart` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenCart** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opencart": {
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
