# Meituan Waimai Open API / 美团外卖 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meituan-waimai-open-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

China's leading food delivery platform — manage store operations, orders, and delivery tracking via AI.

## Description
Empower your AI agent to orchestrate your food delivery operations with **Meituan Waimai** (美团外卖), the dominant delivery platform in China. By connecting Meituan to your agent, you transform complex order management, store status updates, and courier tracking into a natural conversation. Your agent can instantly retrieve store metadata, confirm new orders, browse user comments, and audit delivery progress without you ever needing to navigate the comprehensive Meituan Merchant Portal. Whether you are automating fulfillment or monitoring customer satisfaction across multiple branches, your agent acts as a real-time operations assistant, providing accurate results from a single, unified source.

### What you can do

- **Store Orchestration** — Retrieve store info, update online/offline status, and manage food categories.
- **Order Management** — Confirm new orders, retrieve detailed metadata, and cancel orders with specific reason codes.
- **Delivery Auditing** — Track courier status and real-time delivery progress for any active order.
- **Sentiment Insights** — Browse and analyze user ratings and comments to monitor store performance.
- **Task Automation** — List and filter recent orders across specific time ranges for financial auditing.

### How it works

1. Subscribe to this server
2. Enter your Meituan Client ID and Client Secret
3. Start managing your delivery operations through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Store Managers** — manage order lifecycles and store status through natural language queries.
- **Operations Teams** — monitor delivery efficiency and audit customer feedback directly from your AI-powered workspace.
- **Developers** — integrate professional delivery APIs into your AI-driven daily routines.
- **Meituan Power Users** — integrate your existing merchant workflows into your AI-driven daily routines.


## Available Tools (10)
- **cancel_order**: Cancel an order
- **confirm_order**: Confirm a new order
- **get_order_detail**: Get order details
- **get_store_comments**: Get store reviews
- **get_store_info**: Get store metadata
- **list_categories**: List food categories
- **list_recent_orders**: List recent orders
- **set_store_offline**: Close the store
- **set_store_online**: Open the store
- **track_delivery**: Track delivery status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meituan Waimai Open API / 美团外卖** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the details for order 'ORD_88210934'."

**🤖 AI Agent:**
> I've retrieved the details for order `ORD_88210934`. The total is 45.50 CNY. It includes 2x Beef Noodles and 1x Coke. The customer is located at 'Room 101, Bld 5, Shanghai Garden'. Would you like me to confirm this order now?

---

**👤 You:**
> "Check the delivery status for the active order."

**🤖 AI Agent:**
> I've checked the delivery progress. The courier, 'Zhang Wei', has picked up the order and is currently 1.5 km away from the destination. Estimated delivery time is in 8 minutes.

---

**👤 You:**
> "Open my store 'STORE_8821' for new orders."

**🤖 AI Agent:**
> Done! I've updated the status for store `STORE_8821` to 'Online'. You are now visible on the Meituan app and ready to receive new orders. Would you like me to list any pending orders?


## ❓ FAQ

**Q: How do I find my Meituan Client ID and Secret?**
Log in to the [Meituan Open Platform](https://developer.waimai.meituan.com/), register as a developer, and create an application to receive your unique Client ID and Secret.

**Q: What is an app_poi_code?**
The `app_poi_code` is a unique identifier for your store (Point of Interest) defined within your Meituan application. It is required for all store-specific operations.

**Q: Can I track deliveries in real-time?**
Yes! Use the `track_delivery` tool with a valid order ID to retrieve the courier's current status and predicted arrival information.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meituan-waimai-open-api](https://vinkius.com/mcp/meituan-waimai-open-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meituan Waimai Open API / 美团外卖** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `meituan-waimai-open-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meituan Waimai Open API / 美团外卖** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meituan-waimai-open-api": {
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
