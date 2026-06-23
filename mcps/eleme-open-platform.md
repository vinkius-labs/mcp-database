# Ele.me Open Platform / 饿了么 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eleme-open-platform)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

China's massive food delivery API — manage shops, process orders, and track deliveries via AI.

## Description
Empower your AI agent to orchestrate your food delivery business with the **Ele.me Open Platform** (饿了么), one of the largest on-demand delivery networks in the world. By connecting Ele.me to your agent, you transform complex merchant operations, order fulfillment, and delivery tracking into a natural conversation. Your agent can instantly retrieve shop metadata, confirm incoming orders, manage product categories, and audit real-time delivery states without you ever needing to navigate the comprehensive Ele.me Merchant Center. Whether you are automating a busy kitchen or monitoring customer feedback across a retail chain, your agent acts as a real-time digital manager, providing accurate and fast results from a single, authorized source.

### What you can do

- **Shop Orchestration** — Retrieve shop info, open or close stores, and list product categories.
- **Order Management** — Confirm new orders, retrieve detailed metadata, and cancel orders with specific remarks.
- **Delivery Tracking** — Monitor the real-time state of the courier and the delivery progress for any order.
- **Feedback Auditing** — Retrieve and analyze user comments and ratings to maintain service quality.
- **Inventory Control** — Access and browse shop categories to coordinate menu availability.

### How it works

1. Subscribe to this server
2. Enter your Ele.me App Key, App Secret, and Access Token
3. Start managing your delivery business through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Restaurant Owners** — manage order workflows and shop status through natural language queries.
- **Retail Operations** — monitor delivery efficiency and audit merchant performance directly from your AI-powered workspace.
- **Developers** — integrate professional food delivery APIs into your AI-driven daily routines.
- **Ele.me Power Users** — integrate your existing merchant workflows into your AI-driven daily routines.


## Available Tools (10)
- **cancel_order**: Cancel an order
- **close_shop**: Set shop status to closed
- **confirm_order**: Confirm an order
- **get_order_comments**: Get order comments
- **get_order_detail**: Get order details
- **get_shop_info**: Get shop metadata
- **list_recent_orders**: List recent orders
- **list_shop_categories**: List shop product categories
- **open_shop**: Set shop status to open
- **track_delivery**: Track delivery state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ele.me Open Platform / 饿了么** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the metadata for shop 'SHOP_88210934'."

**🤖 AI Agent:**
> I've retrieved the shop metadata. 'Happy Noodles' (ID: `SHOP_88210934`) is currently 'Open' and has a 4.8-star rating. It is located at '123 Main St, Shanghai'. Would you like to see the available product categories for this shop?

---

**👤 You:**
> "List the most recent orders for my shop."

**🤖 AI Agent:**
> I've retrieved your recent orders. You have 5 new orders waiting for confirmation. The most recent is `ORD_9920` for 85.00 CNY. Should I provide the detailed item breakdown for this order?

---

**👤 You:**
> "Track the delivery state for order 'ORD_8821'."

**🤖 AI Agent:**
> The delivery state for order `ORD_8821` is currently 'In Transit'. The courier, 'Li Qiang', is on his way to the customer. He was last located 500 meters from the destination. I'll monitor for the 'Delivered' confirmation.


## ❓ FAQ

**Q: How do I find my Ele.me App Key and Secret?**
Log in to the [Ele.me Open Platform](https://open.shop.ele.me/), register your application, and you will find your App Key and App Secret in the application details overview.

**Q: How do I get an Access Token?**
Ele.me uses OAuth2. You must perform the authorization flow (linking your merchant account to your application) to generate an access token. This token must be provided in the credentials for this server.

**Q: Can I cancel orders through the agent?**
Yes! Use the `cancel_order` tool with the specific order ID and a valid reason code. Note that order cancellation usually requires justification and may be subject to merchant policies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eleme-open-platform](https://vinkius.com/mcp/eleme-open-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ele.me Open Platform / 饿了么** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `eleme-open-platform` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ele.me Open Platform / 饿了么** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eleme-open-platform": {
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
