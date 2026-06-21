# Booqable MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/booqable)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/booqable-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/booqable-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your rentals via Booqable — track orders, check availability, and manage inventory directly from any AI agent.

## Description
Connect your **Booqable** rental management account to any AI agent and orchestrate your inventory and order workflows through natural conversation.

### What you can do

- **Order Lifecycle Management** — List, retrieve, and transition orders from concepts to started and stopped states.
- **Inventory Oversight** — Access your product groups and technical product details to ensure accurate catalog management.
- **Real-time Availability** — Check if items are rentable for specific dates and times to prevent double-bookings.
- **Customer Coordination** — Access and manage your customer directory and individual profiles.
- **Operational Control** — Mark orders as picked up (started) or returned (stopped) directly from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Booqable API Key and Subdomain
3. Start managing your rental operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Rental Business Owners** — quickly check for today's pickups and returns without opening the dashboard.
- **Operations Leads** — monitor stock levels and customer details straight from their workflow tools.
- **Support Teams** — verify order statuses and availability using natural language.


## Available Tools
- **check_availability**: Check item availability for specific dates
- **create_order**: Create a new rental order
- **get_customer**: Get details of a specific customer
- **get_order**: Get details of a specific order
- **get_product_group**: Get details of a specific product group
- **list_customers**: List all customers
- **list_orders**: List all rental orders
- **list_product_groups**: List all rental product groups (catalog)
- **start_order**: Mark an order as started (picked up)
- **stop_order**: Mark an order as stopped (returned)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Booqable** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active rental orders in Booqable."

**🤖 AI Agent:**
> I've retrieved your orders. You have 5 active rentals, including Order #1001 (Status: Started) and Order #1005 (Status: Reserved). Would you like to check the items for any of these?

---

**👤 You:**
> "Check if 'Camera Kit' is available from June 10th to June 12th."

**🤖 AI Agent:**
> Checking availability... Yes, the 'Camera Kit' group has 3 units available for those dates. Would you like me to create a concept order?

---

**👤 You:**
> "Mark order #1001 as returned."

**🤖 AI Agent:**
> Order #1001 has been successfully marked as 'Stopped' (returned). The items are now back in your available inventory.


## Installation & Usage

To install and use the **Booqable** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/booqable](https://vinkius.com/mcp/booqable)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
