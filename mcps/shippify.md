# Shippify MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shippify)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/shippify-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/shippify-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [order-management](../categories/order-management.md)

Automate logistics and last-mile delivery via Shippify — manage deliveries, tracking, and warehouses directly from any AI agent.

## Description
Connect your **Shippify** account to any AI agent and simplify your logistics orchestration and last-mile delivery management through natural conversation.

### What you can do

- **Delivery Management** — List all active, scheduled, and completed deliveries, retrieve detailed status and destination metadata
- **Direct Execution** — Create new delivery orders programmatically directly from your agent by providing location and package details
- **Live Tracking** — Access real-time geographic tracking info for active shipments to keep your customers informed
- **Inventory Control** — List available warehouses and pickup points linked to your account
- **Operational Insights** — Monitor your delivery pipeline and fulfillment efficiency directly from your agent

### How it works

1. Subscribe to this server
2. Enter your Shippify API Key and API Secret from your dashboard
3. Start managing your deliveries from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **cancel_delivery**: Cancel a pending delivery
- **get_driver**: Get details for a specific driver
- **get_delivery_quote**: Get a delivery price quote
- **get_tracking**: Get real-time tracking for a delivery
- **list_drivers**: List all available delivery drivers
- **list_routes**: List all delivery routes
- **create_delivery**: Schedule a new delivery
- **get_delivery_details**: Get details for a specific delivery
- **get_delivery_tracking**: Check live tracking info
- **list_deliveries**: List Shippify deliveries
- **list_warehouses**: List available warehouses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shippify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active deliveries in Shippify."

**🤖 AI Agent:**
> I've retrieved your deliveries. You have 5 active shipments, including 'Shipment #123' (In Transit) and 'Shipment #456'.

---

**👤 You:**
> "Show me all active deliveries in progress with real-time tracking and driver assignments."

**🤖 AI Agent:**
> 18 active deliveries. En route (12): Driver Carlos near destination for DEL-8923 (ETA 8 min). Driver Maria picking up DEL-8934 at warehouse. 10 others in transit across 3 zones. Waiting pickup (4): assigned to drivers, avg wait 12 min. Scheduled (2): departing in 1 hour. Today's stats: 45 deliveries completed, avg delivery time 34 min, on-time rate 92%. Fastest today: 18 min (DEL-8901). 2 deliveries had route changes due to traffic. Total active drivers: 14 of 20.

---

**👤 You:**
> "Get a delivery quote for a same-day package from downtown to the airport district."

**🤖 AI Agent:**
> Delivery quote generated. Route: Downtown (pickup) → Airport District (dropoff). Distance: 14.2 km. Estimated time: 28 minutes. Options: Standard (45 min window): $8.50. Express (30 min window): $12.90. Priority (15 min window): $18.50. Package size: Small (up to 5kg). Insurance included up to $100. Real-time tracking: included in all options. Available drivers in area: 6. Recommended: Express at $12.90 (best availability, 2 drivers nearby). Surge: none (normal demand).


## Installation & Usage

To install and use the **Shippify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shippify](https://vinkius.com/mcp/shippify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
