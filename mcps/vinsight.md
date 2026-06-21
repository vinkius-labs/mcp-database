# Vinsight MCP Server

Manage wine, beer, and spirits production — inventory, sales orders, batches, vessels, and lab results for your Vinsight operation through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/vinsight)

## Overview
**Category:** erp-operations
**Tools Count:** 12

## Description
Connect your **Vinsight** operation to any AI agent and manage your entire beverage production business through natural conversation.

### What you can do

- **Stock Items** — Search your product catalog: wines, beers, spirits, and raw materials with pricing and compliance codes
- **Sales Orders** — Track orders: customer, items, totals, status, and shipping across all channels
- **Production Orders** — Monitor production runs: input materials, output products, vessel assignments
- **Batches** — Track individual lots through the production lifecycle with batch codes and vintage
- **Vessels** — Monitor tanks, fermenters, barrels, and bright tanks with capacity and fill levels
- **Lab Results** — View QC analyses: pH, TA, alcohol, SO₂, dissolved oxygen, and residual sugar
- **Inventory** — Real-time stock levels across all warehouses: available, committed, and on-order
- **Contacts** — Manage customers, suppliers, and distributors
- **Purchase Orders** — Track incoming materials: grapes, bottles, corks, chemicals

### Who is this for?

- **Winemakers & Brewmasters** — Production tracking, batch management, and quality control
- **Operations Managers** — Inventory visibility, warehouse management, and supply chain tracking
- **Sales Teams** — Order status, customer insights, and available stock queries
- **Finance** — Revenue tracking, purchase costs, and margin analysis


## Available Tools
- **search_stock_items**: Returns product details including SKU, description, unit of measure, price, tax code, and current stock level. Works for wine, beer, spirits, and raw materials.

Search wine/beer/spirit products
- **list_stock_levels**: Critical for fulfillment and reorder decisions.

List current inventory
- **list_lab_results**: Sorted by date. For quality control and compliance monitoring.

List lab analysis results
- **list_warehouses**: For multi-site inventory management.

List warehouses
- **get_stock_item**: The definitive product record.

Get product details
- **list_sales_orders**: Core revenue tracking for wineries and breweries.

List sales orders
- **get_sales_order**: Get order details
- **search_contacts**: Returns contact profile, type, addresses, payment terms, and order history.

Search contacts
- **list_purchase_orders**: Supply chain tracking for production inputs.

List purchase orders
- **list_production_orders**: Tracks the winemaking or brewing process.

List production orders
- **list_batches**: Track individual lots through the production lifecycle.

List production batches
- **list_vessels**: With capacity, current contents, fill level, and location. For cellar space planning.

List tanks and barrels


## Installation & Usage

To install and use the **Vinsight** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vinsight](https://vinkius.com/mcp/vinsight)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
