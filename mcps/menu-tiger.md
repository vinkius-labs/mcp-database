# MENU TIGER MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/menu-tiger)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/menu-tiger-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/menu-tiger-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Create digital restaurant menus with QR code ordering, table management, and payment integration that modernize the dining experience.

## Description
Connect your **MENU TIGER** account to any AI agent and take full control of your digital restaurant menus and automated order orchestration through natural conversation.

### What you can do

- **Menu Portfolio Orchestration** â€” List and manage your entire portfolio of digital menus programmatically, retrieving detailed item metadata and prices
- **Order & Customer Intelligence** â€” Programmatically retrieve directories of incoming restaurant orders and access complete customer profiles in real-time
- **Store & Layout Architecture** â€” Access your complete directory of store locations and QR menu layouts to coordinate your organizational presence
- **Operational Monitoring** â€” Access real-time status updates for orders (e.g., 'Preparing', 'Served') and track store performance directly through your agent
- **Infrastructure Verification** â€” Verify account-level API connectivity and monitor transaction volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your MENU TIGER dashboard (Settings > API)
3. Start orchestrating your restaurant growth from Claude, Cursor, or any MCP client

No more manual updating of individual menu items or missing critical order statuses. Your AI acts as your dedicated restaurant coordinator and menu architect.

### Who is this for?

- **Restaurant Managers** â€” instantly retrieve menu performance recaps and monitor order volume using natural language commands
- **F&B Directors** â€” verify individual item metadata and track store-wide updates without leaving your creative workspace
- **Developers** â€” integrate high-speed MENU TIGER data into custom kitchen display and BI systems through simple AI queries


## Available Tools
- **check_menutiger_status**: Verify MenuTiger API connectivity
- **get_account**: Get account info
- **get_item**: Get item details
- **get_menu**: Get menu details
- **get_order**: Get order details
- **list_categories**: List menu categories
- **list_items**: List menu items
- **list_menus**: List all menus
- **list_orders**: List all orders
- **update_order_status**: g., preparing, ready, completed, cancelled).

Update order status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MENU TIGER** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all pending orders in my restaurant."

**🤖 AI Agent:**
> You have 8 pending orders. Table 4 has a large order (3 items, ) placed 12 minutes ago. Table 7 has a single drink order. Would you like to update any order status?

---

**👤 You:**
> "Mark order ORD-421 as ready for pickup."

**🤖 AI Agent:**
> Order ORD-421 updated to 'ready'. The customer at Table 4 will be notified. Total: . Would you like to view the next pending order?

---

**👤 You:**
> "List all items in my lunch menu."

**🤖 AI Agent:**
> Your lunch menu has 14 items across 3 categories. Most popular: 'Grilled Chicken Bowl' (). 2 items are currently out of stock. Would you like to see allergen details?


## Installation & Usage

To install and use the **MENU TIGER** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/menu-tiger](https://vinkius.com/mcp/menu-tiger)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
