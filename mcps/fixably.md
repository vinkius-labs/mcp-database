# Fixably MCP Server

Manage repair orders, track inventory, and handle customer data via AI agents with Fixably.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fixably)

## Overview
**Category:** erp-operations
**Tools Count:** 12

## Description
Connect your **Fixably** instance to any AI agent and automate your repair management workflows through the Model Context Protocol (MCP). Fixably provides a comprehensive platform for handling the entire repair lifecycle, from initial order creation to final dispatch. Now, you can manage your service center operations directly through natural conversation.

### What you can do

- **Order Management** — List all repair orders, fetch detailed order metadata, and create or update orders instantly.
- **Customer Oversight** — Access your customer database, retrieve specific profiles, and search for accounts by name or email.
- **Inventory Tracking** — List all stock locations and monitor product availability at specific inventory sites.
- **Operational Updates** — Post internal notes to orders and update the internal location of devices (e.g., from SERVICE to STORE).
- **Document Access** — List all files and attachments associated with a repair order for quick reference.
- **Real-time Monitoring** — Fetch specific order statuses or device locations to keep your service team and customers informed.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Fixably Subdomain and API Token (found in User Settings > Integrations)
3. Start managing your repair operations from Claude, Cursor, or any MCP client

### Who is this for?

- **Service Technicians** — quickly check order details or add repair notes without leaving your primary workspace.
- **Store Managers** — get a real-time overview of inventory across locations and update order statuses via simple AI commands.
- **Customer Support** — automate the retrieval of order updates and customer history to provide faster resolutions.


## Available Tools
- **add_order_note**: Add note to order
- **change_internal_location**: g. SERVICE, STORE).

Change device location
- **create_order**: Create a new order
- **get_customer**: Get customer details
- **get_order**: Get order details
- **get_stock**: Get stock details
- **list_customers**: List customers
- **list_order_files**: List files for order
- **list_orders**: List repair orders
- **list_stock_products**: List products in stock
- **list_stocks**: List inventory locations
- **update_order**: Update an order


## Installation & Usage

To install and use the **Fixably** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fixably](https://vinkius.com/mcp/fixably)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
