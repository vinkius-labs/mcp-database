# Rappi API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rappi-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate LatAm's largest super-app via Rappi — track active deliveries, request support, and manage logistics from your agent.

## Description
Empower your intelligent agents directly with **Rappi API**, the dominant delivery and logistics super-app bridging Latin America. Bypass chaotic consumer screens and deploy 10 robust tools natively automating restaurant queries, massive localized delivery management, and real-time courier tracking through any AI system magically.

### What you can do

- **Logistics Control** — Trace geographic rider coordinates, predict dynamic delivery fees, and seamlessly tip couriers natively without touching mobile interfaces.
- **Order Placement** — Query menu endpoints securely, push nested orders to specific merchant ID endpoints, and execute transactions automatically in the background.
- **Customer Care Automation** — Dispute missing items securely opening help tickets and communicating automatically via Support endpoints.
- **Market Analysis** — Poll local 'Turbo' supermarkets or pharmacies parsing active stock pricing to feed comparative database dashboards.

### How it works

1. Secure developer approval connecting via the [Rappi Developer Hub](https://dev.rappi.com/)
2. Abstract your regional operations extracting your core **Client ID** alongside its heavy **Client Secret**
3. Plug those core variables explicitly below overriding local setups
4. Trigger commands! Vurb absorbs the intensive REST endpoints securely wrapping responses in natural text formats.

### Who is this for?

- **Office Coordinators** — schedule and manage multiple large corporate food deliveries across various departments passively tracking arrivals live blindly.
- **Urban Planners** — scrap real-world geographic delivery timelines crossing traffic bottlenecks estimating true logistic costs precisely in heavy hubs.
- **LatAm SaaS Integrators** — build consolidated order aggregators unifying local Rappi merchant data with alternative distribution networks strictly under one hood.


## Available Tools (10)
- **get_order_detail**: Get full details for a specific order
- **list_new_orders**: List new incoming orders awaiting acceptance
- **list_stores**: List all registered stores under your account
- **mark_ready_for_pickup**: Signal that an order is ready for courier pickup
- **reject_order**: Reject an incoming order with a reason
- **take_order**: Accept and start preparing an incoming order
- **update_store_status**: Open or close a store for receiving orders
- **get_store_availability**: Check availability status of a store
- **get_order_handoff**: Get handoff confirmation codes for an order
- **get_store_menu**: Retrieve the full menu of a store


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rappi API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List nearby stores in the 'pharmacy' category around coordinates 4.6097, -74.0817."

**🤖 AI Agent:**
> Grid scanned! I found 3 pharmacies capable of delivering to that specific coordinate set within ETA windows of under 30 minutes. Farmatodo (Store ID: f_91) has the lowest dynamic delivery fee. Should I extract their painkiller catalog next?

---

**👤 You:**
> "Check the delivery state and ETA for my active order number 8812920."

**🤖 AI Agent:**
> Tracking ping dispatched... Order 8812920 is currently in the 'Out for Delivery' state. The courier is 1.2 kilometers away, moving smoothly. Adjusted ETA sits exactly at 6 minutes from now without delays. Need me to authorize a tip?

---

**👤 You:**
> "Cancel the active order 88910 immediately citing missing items from the receipt."

**🤖 AI Agent:**
> Order cancellation request dispatched forcing priority queue... Order 88910 has been successfully aborted and zeroed out. The refund algorithm triggered automatically citing error 'Items Missing against receipt'. The credits should append to your vault safely. Want me to draft an escalated complaint?


## ❓ FAQ

**Q: Does order placement via the API bypass the normal Rappi checkout security rules?**
No. The `place_order` tool uses your pre-authenticated method securely. Bank validations, anti-fraud algorithms, and location checks apply exactly as they would natively in the application avoiding compliance breaches entirely.

**Q: Can I explicitly track multiple concurrent active orders dynamically simultaneously?**
Yes! Your agent can iterate over an array of active Order IDs using the `get_order_status` tool consistently. It parses coordinate updates and ETA drops, outputting a consolidated table summing up your entire inbound fleet seamlessly.

**Q: Are the store identifiers (storeId) universally stable across regions?**
Store IDs are fundamentally unique keys generated explicitly by Rappi's catalog backend. They remain static for the lifetime of that specific branch location. Searching via `list_nearby_stores` initially is recommended to cache the correct target IDs dynamically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rappi-api](https://vinkius.com/mcp/rappi-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rappi API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rappi-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rappi API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rappi-api": {
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
