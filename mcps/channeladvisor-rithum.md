# ChannelAdvisor (Rithum) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/channeladvisor-rithum)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/channeladvisor-rithum-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/channeladvisor-rithum-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage multi-channel commerce via ChannelAdvisor — track products, inventory, and orders across global marketplaces directly from any AI agent.

## Description
Connect your **ChannelAdvisor (Rithum)** account to any AI agent and take full control of your e-commerce operations across Amazon, Walmart, eBay, and more through natural conversation. Streamline multi-channel selling and fulfillment.

### What you can do

- **Catalog Oversight** — List and retrieve details for products in your global catalog natively
- **Order Fulfillment** — Access and monitor customer orders across all connected marketplaces flawlessly
- **Inventory Synchronization** — Update stock levels and manage distribution center quantities securely
- **Shipment Management** — List fulfillments and tracking numbers to monitor delivery progress in real-time
- **Label Control** — Access and manage product labels for easier organization and classification flawlessly
- **Distribution Intelligence** — List available distribution centers and retrieve core account profile metadata directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your ChannelAdvisor Access Token and Profile ID
3. Start managing your multi-channel sales from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Directors** — monitor sales and inventory health across global channels using natural language
- **Operations Managers** — update stock levels and audit fulfillments without opening the complex dashboard
- **Marketplace Analysts** — quickly look up product details and order statuses straight from their chat interface
- **Logistics Specialists** — verify tracking information and distribution center availability for multi-channel orders


## Available Tools
- **get_ca_order_details**: Get detailed information for a specific order
- **get_ca_product_details**: Get detailed information for a specific product
- **list_distribution_centers**: List available distribution centers
- **list_ca_fulfillments**: List order fulfillments and tracking
- **list_ca_labels**: List configured product labels
- **list_ca_orders**: List customer orders
- **list_ca_products**: List products in the ChannelAdvisor catalog
- **update_ca_inventory**: Update inventory levels for a product


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ChannelAdvisor (Rithum)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 10 orders across all marketplaces."

**🤖 AI Agent:**
> Retrieving your recent orders... I found 10 items including Order #98765 (Walmart), #54321 (Amazon), and #12345 (eBay). Would you like to see the items for any of these?

---

**👤 You:**
> "What is the total quantity available for SKU 'WIDGET-001'?"

**🤖 AI Agent:**
> Checking inventory for 'WIDGET-001'... You have 45 units available across 2 distribution centers (30 in East DC, 15 in West DC).

---

**👤 You:**
> "Search for products with 'Smartphone' in the title."

**🤖 AI Agent:**
> Searching for 'Smartphone'... I found 3 products: 'Smartphone X1', 'Smartphone Pro Max', and 'Refurbished Smartphone'. Would you like the details for one of them?


## Installation & Usage

To install and use the **ChannelAdvisor (Rithum)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/channeladvisor-rithum](https://vinkius.com/mcp/channeladvisor-rithum)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
