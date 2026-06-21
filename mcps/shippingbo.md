# ShippingBo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shippingbo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/shippingbo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/shippingbo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Orchestrate your e-commerce logistics with order management, warehouse operations, and carrier integration for French retailers.

## Description
Connect your **ShippingBo** account to any AI agent and take full control of your e-commerce logistics and fulfillment orchestration through natural conversation. ShippingBo provides a comprehensive platform for centralizing orders, managing multi-warehouse stocks, and orchestrating shipments directly from your chat interface.

### What you can do

- **Order & Fulfillment Orchestration** — List and retrieve detailed metadata for your sales orders to keep your fulfillment pipeline synchronized programmatically.
- **Product & Stock Management** — Access and monitor your product catalog and update stock counts for specific items directly from the AI interface.
- **Shipment Lifecycle Control** — List and monitor shipments and track delivery progress via natural language to ensure customer satisfaction.
- **Warehouse Slot Intelligence** — Access and monitor warehouse slots to maintain a clear overview of your physical storage organization.
- **Operational Monitoring** — Track system activity and monitor packs to ensure your logistics setup is always optimized using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your ShippingBo API User, Token, and Version from your dashboard
3. Start managing your e-commerce logistics from Claude, Cursor, or any MCP-compatible client

No more manual stock checks or order hunting. Your AI acts as a dedicated logistics manager or fulfillment coordinator.

### Who is this for?

- **E-commerce Logistics Managers** — quickly retrieve order details and monitor multi-warehouse stocks without switching apps.
- **Warehouse Operations Teams** — automate the update of stock counts and monitor shipment progress via natural conversation.
- **Customer Success Teams** — streamline the retrieval of shipment metadata and coordinate order fulfillments directly within the chat.


## Available Tools
- **get_order**: Get order details
- **get_product**: Get product details
- **list_orders**: List all orders
- **list_packs**: List packaging options
- **list_products**: List all products
- **list_shipments**: List all shipments
- **list_warehouse_slots**: List warehouse storage slots
- **update_stock**: Update product stock level


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ShippingBo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in my ShippingBo catalog."

**🤖 AI Agent:**
> I've retrieved your product catalog. You have 125 active SKUs including 'Summer T-Shirt (Blue)', 'Wireless Headphones', and 'Eco Water Bottle'. Which one would you like to check stock for?

---

**👤 You:**
> "Update stock for product ID 54321 to 150 units."

**🤖 AI Agent:**
> Stock update processed! Product 54321 now has 150 units in your main warehouse. Should I verify if any pending orders can now be fulfilled?

---

**👤 You:**
> "List the last 5 shipments in ShippingBo."

**🤖 AI Agent:**
> Retrieving shipments... Your last 5 shipments include 'SH-9901' (Delivered), 'SH-9902' (In Transit), and three others. Would you like to see the tracking progress for the one in transit?


## Installation & Usage

To install and use the **ShippingBo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shippingbo](https://vinkius.com/mcp/shippingbo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
