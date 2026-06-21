# Enspire Commerce MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/enspire-commerce)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/enspire-commerce-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/enspire-commerce-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to manage omni-channel orders, track inventory, and monitor shipments via the Enspire API.

## Description
Integrate **Enspire Commerce**, the comprehensive omni-channel order management platform, directly into your AI workflow. Manage your commerce orders across all channels, track real-time inventory levels and warehouse stock, monitor shipments and tracking information, and oversee your fulfillment network using natural language.

### What you can do

- **Order Oversight** — List and retrieve detailed information, line items, and fulfillment status for all your omni-channel orders.
- **Inventory Intelligence** — Monitor real-time stock levels across SKUs and fulfillment centers, resolving available-to-promise (ATP) counts.
- **Logistics Management** — Access and monitor shipments, resolving tracking numbers, carriers, and dispatch timestamps.
- **Commerce Auditing** — Retrieve high-level summaries of order volume, shipment activity, and organizational inventory health instantly.

### How it works

1. Connect the Enspire Commerce integration to your AI assistant.
2. Authorize using your Enspire API Key (found in your developer settings).
3. Orchestrate your omni-channel commerce and fulfillment strategy through intuitive conversation.

### Who is this for?

- **E-commerce Managers** — Quickly check order statuses and stock availability on the go.
- **Logistics Coordinators** — Research shipment tracking and warehouse metadata via chat.
- **Operations Teams** — Monitor inventory thresholds and organizational commerce metadata instantly.


## Available Tools
- **get_enspire_account_metadata**: Retrieve metadata and limits for your Enspire account
- **get_order_details**: Get detailed settings and line items for a specific order
- **get_sku_stock_level**: Get real-time stock levels for a specific product SKU
- **quick_commerce_volume_audit**: Retrieve a high-level summary of orders, shipments, and stock
- **list_fulfillment_locations**: List all fulfillment centers and warehouses configured in your network
- **list_inventory_levels**: List inventory levels across all products and locations
- **list_low_inventory_skus**: Identify products that are currently below a safe inventory threshold (mock logic)
- **list_commerce_orders**: List all omni-channel orders in your Enspire account
- **list_latest_commerce_orders**: Identify the most recently placed omni-channel orders
- **list_recent_shipments**: List all shipments and tracking information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enspire Commerce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pending commerce orders."

**🤖 AI Agent:**
> I've found 12 pending orders, including '#ORD-1001' ($250) and '#ORD-1005' ($1,200). 8 are awaiting pick-up and 4 are in backorder. Would you like the details for #ORD-1005?

---

**👤 You:**
> "What is the stock level for SKU 'TSHIRT-BLU-L'?"

**🤖 AI Agent:**
> The SKU 'TSHIRT-BLU-L' has a total ATP (Available-to-Promise) count of 150 units. Breakdown: Warehouse A (85), Warehouse B (45), and Retail Store 1 (20). Should I check for low stock on related SKUs?

---

**👤 You:**
> "Show me recent shipments from today."

**🤖 AI Agent:**
> I've retrieved today's shipments. 45 orders were dispatched via FedEx and 20 via UPS. All tracking numbers have been generated and sent to customers. Would you like a summary of any delayed shipments?


## Installation & Usage

To install and use the **Enspire Commerce** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/enspire-commerce](https://vinkius.com/mcp/enspire-commerce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
