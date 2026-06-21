# Mercado Livre Orders MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mercado-livre-orders)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mercado-livre-orders-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mercado-livre-orders-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search sales, manage shipments, track packages, and handle cancellations on Mercado Livre.

## Description
Connect **Mercado Livre Orders** to any AI agent and take full control of your order management system — search sales, track shipments, register invoices, and handle cancellations through natural conversation.

### What you can do
- **Order Search** — Find sales by status (paid, shipping, delivered, cancelled)
- **Order Details** — Get full info on buyer, items, and totals for a specific sale
- **Shipping Management** — View shipping status, carrier info, and tracking codes
- **Tracking Updates** — Set tracking numbers for shipments handled outside Mercado Envios
- **Buyer Feedback** — Check ratings and comments left by buyers
- **Order Cancellation** — Cancel sales when necessary (requires valid reason)

### How it works
1. Subscribe to this server
2. Enter your Mercado Livre OAuth2 Access Token
3. Start managing orders from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Sellers** — Monitor sales activity and shipping status without manual dashboard checks
- **Customer Support** — Quickly access order details and tracking info to answer buyer queries
- **Logistics Teams** — Register invoices and update tracking codes in bulk via AI


## Available Tools
- **cancel_order**: Requires a valid reason.

Cancel a sale
- **get_feedback**: Get buyer feedback/reputation for a sale
- **get_order**: Get details of a specific sale
- **search_orders**: Search for sales/orders
- **get_shipments**: List shipments associated with an order
- **get_shipping_info**: Get shipping details for an order
- **set_tracking**: Set tracking number for a shipment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mercado Livre Orders** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all orders that need shipping."

**🤖 AI Agent:**
> Found 3 orders ready for shipping: 1. MLB-Order123 (R$150.00). 2. MLB-Order456 (R$89.90). 3. MLB-Order789 (R$210.00).

---

**👤 You:**
> "Get details for order MLB-Order123."

**🤖 AI Agent:**
> Order MLB-Order123: Status: Paid. Buyer: João Silva. Total: R$150.00. Item: Wireless Headphones.

---

**👤 You:**
> "Register invoice 9999 for shipment 12345 with tracking XYZ."

**🤖 AI Agent:**
> Invoice registered successfully! Tracking code XYZ set for shipment 12345.


## Installation & Usage

To install and use the **Mercado Livre Orders** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mercado-livre-orders](https://vinkius.com/mcp/mercado-livre-orders)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
