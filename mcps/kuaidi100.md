# KuaiDi100 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kuaidi100)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Ubiquitous logistics and package tracking platform in China — track shipments via AI.

## Description
Empower your AI agent to orchestrate your logistics and supply chain operations with **KuaiDi100** (快递100), the leading package tracking platform in China. By connecting KuaiDi100 to your agent, you transform complex shipment monitoring and carrier identification into a natural conversation. Your agent can instantly track packages in real-time, identify carriers from tracking numbers, subscribe to delivery updates, and even estimate shipping prices without you ever needing to navigate the comprehensive KuaiDi100 portal. Whether you are managing high-volume e-commerce fulfillment or auditing international shipments, your agent acts as a real-time logistics assistant, keeping your delivery data accurate and your customers informed.

### What you can do

- **Real-time Tracking** — Retrieve current status and complete historical data for any domestic or international package.
- **Carrier Identification** — Automatically identify the likely carrier for a given tracking number to simplify operations.
- **Update Subscriptions** — Set up automated webhooks to receive real-time push notifications when a package status changes.
- **Price Estimation** — Retrieve estimates for shipping costs based on weight and destination across different carriers.
- **Mapping & Routing** — Access map-ready tracking data to visualize the physical journey of a shipment.

### How it works

1. Subscribe to this server
2. Enter your KuaiDi100 Customer ID and API Key
3. Start managing your logistics through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Operations** — monitor hundreds of shipments and automate customer notifications through natural language.
- **Logistics Managers** — coordinate with carriers and audit delivery performance directly from your AI-powered workspace.
- **Customer Success Teams** — provide instant shipping status updates to clients via a unified AI interface.
- **KuaiDi100 Power Users** — integrate your existing logistics workflows into your AI-driven daily routines.


## Available Tools (8)
- **estimate_delivery_time**: Estimate delivery time between locations
- **get_map_tracking**: Get map-based tracking data
- **identify_carrier**: Auto-detect carrier from tracking number
- **query_shipping_price**: Get shipping price estimate
- **submit_shipping_order**: Generates an electronic waybill for printing.

Submit a shipping order (e-waybill)
- **subscribe_tracking**: Subscribe to tracking status updates
- **track_package**: Some carriers (e.g., SF Express) require the recipient phone number.

Track a package in real-time
- **check_carrier_availability**: Check which carriers serve a route


## 💬 Prompt Examples

Here are some examples of how you can interact with the **KuaiDi100** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Track my Shunfeng package with number 'SF123456789'."

**🤖 AI Agent:**
> I've retrieved the status for your SF Express package. It is currently in transit and arrived at the 'Shanghai Logistics Hub' at 10:30 AM today. It is expected to be delivered tomorrow.

---

**👤 You:**
> "Identify which carrier uses number 'YT1234567890'."

**🤖 AI Agent:**
> I've analyzed the tracking number. It most likely belongs to 'YuanTong Express' (yuantong). Would you like me to retrieve the real-time status for this package?

---

**👤 You:**
> "Estimate the shipping cost for a 2kg package from Beijing to Shenzhen."

**🤖 AI Agent:**
> I've retrieved price estimates for you. Shipping 2kg from Beijing to Shenzhen would cost approximately ¥18 via Yunda, ¥22 via ZTO, or ¥35 via SF Express (Standard). Which service would you prefer?


## ❓ FAQ

**Q: How do I find my KuaiDi100 Customer ID and Key?**
Log in to the [KuaiDi100 API Portal](https://api.kuaidi100.com/), register for a developer account, and you will find your Customer Code (customer) and Authentication Key (key) in your account management dashboard.

**Q: Do I need a phone number for tracking?**
Some premium carriers, especially Shunfeng (SF Express) and JD Logistics, require the last 4 digits of the recipient's phone number to retrieve tracking data for security reasons.

**Q: Is international tracking supported?**
Yes! KuaiDi100 supports over 1,000 domestic and international carriers. You can use the `identify_carrier` tool if you are unsure which global company is handling your shipment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kuaidi100](https://vinkius.com/mcp/kuaidi100)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **KuaiDi100** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kuaidi100` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **KuaiDi100** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kuaidi100": {
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
