# Wherefour MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wherefour)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wherefour-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wherefour-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage inventory, traceability, and orders with Wherefour ERP through AI.

## Description
Connect your **Wherefour** account to any AI agent to automate your inventory management, production tracking, and lot traceability. Wherefour provides a specialized ERP platform for manufacturers and producers to maintain end-to-end transparency across their supply chain.

### What you can do

- **Inventory & Catalog Orchestration** — List and search inventory items with detailed metadata, including product codes and manufacturing specifications.
- **Lot Traceability** — Access stock lot details and batch information to maintain comprehensive quality control and compliance.
- **Order Management** — Retrieve and monitor sales orders and production orders to keep your manufacturing workflow on track.
- **Stakeholder Directory** — Access and manage your database of customers, vendors, and suppliers programmatically.
- **Financial Insights** — Retrieve billing invoices and purchase records directly from the AI interface to monitor operational costs.
- **Resource Navigation** — Explore storage locations and manufacturing formulas using natural language commands.

### How it works

1. Subscribe to this server
2. Enter your Wherefour API Key and API Secret from your account settings
3. Select your environment (Production or Sandbox)
4. Start managing your ERP and inventory from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — quickly check stock levels and production order statuses without switching apps.
- **Quality Control Teams** — track lot traceability and batch metadata via natural conversation.
- **Inventory Controllers** — streamline item searches and vendor management through simple AI commands.


## Available Tools
- **get_inventory_item**: Get details of a specific inventory item
- **get_order**: Get details of a specific order
- **list_customers**: List all customers
- **list_formulas**: List production formulas/recipes
- **list_inventory_items**: List all inventory items
- **list_invoices**: List customer invoices
- **list_locations**: List storage locations
- **list_orders**: List all sales and production orders
- **list_purchases**: List purchase records
- **list_stock_lots**: List all stock lots
- **list_vendors**: List all vendors/suppliers
- **search_inventory**: Search for inventory items


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wherefour** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search our inventory for 'Organic Cane Sugar' and pull up the production formula that uses it for the upcoming beverage batch."

**🤖 AI Agent:**
> I found 'Organic Cane Sugar' (Item #8492) in your inventory with 450 lbs currently in stock. It is a primary ingredient in the 'Summer Citrus Kombucha' formula. The formula requires 25 lbs of sugar per production batch. Would you like to view the full recipe?

---

**👤 You:**
> "Check the lot traceability for batch 'L-2024-QT3' of Arabica Coffee Beans and tell me which warehouse location it is currently stored in."

**🤖 AI Agent:**
> I've retrieved the traceability data for lot 'L-2024-QT3'. This batch of Arabica Coffee Beans was received from 'Highland Roasters' on October 12th. It passed quality inspection and is currently stored in 'Warehouse B, Zone 4, Rack 12'. There are 120 units remaining in this lot.

---

**👤 You:**
> "List all pending production orders for 'Acme Supermarkets' and verify if their latest invoice from last month has been paid."

**🤖 AI Agent:**
> There are 2 pending production orders for 'Acme Supermarkets': PO-7381 (Organic Oatmeal) and PO-7389 (Almond Milk), both scheduled for completion this Friday. I also checked their billing records; Invoice #INV-5920 from last month is marked as 'Paid in Full'.


## Installation & Usage

To install and use the **Wherefour** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wherefour](https://vinkius.com/mcp/wherefour)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
