# Pipedrive Products MCP Server

Manage your product catalog, attach products to deals, and track recurring revenue subscriptions in Pipedrive.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pipedrive-products)

## Overview
**Category:** productivity
**Tools Count:** 8

## Description
Connect **Pipedrive CRM** to any AI agent — manage your entire sales pipeline without switching tabs.

### What you can do
- **Deals** — Search, create, and update deals with pipeline tracking
- **Contacts** — Find and create persons with email, phone, and organization
- **Organizations** — Search companies linked to deals and contacts
- **Activities** — Create calls, meetings, tasks, and emails
- **Notes** — Attach notes to deals, persons, or organizations
- **Pipelines** — View all pipeline stages and deal flow

### Who is this for?
- **Sales Reps** — Manage your pipeline without leaving your AI assistant
- **SDRs** — Quickly create leads, contacts, and activities
- **Sales Managers** — Pipeline overview and deal insights through conversation
- **RevOps** — Full CRM visibility and reporting


## Available Tools
- **pd_add_product_to_deal**: Requires the deal ID, product ID (use pd_search_products or pd_list_products to find), unit price, and quantity. The line-item total is calculated automatically. Use when the user wants to add a product to a deal, build a quote, or track what is being sold.

Attach a product from the catalog to a deal with a specific quantity and unit price for line-item tracking
- **pd_create_product**: Name is required. Code serves as the internal SKU/reference. Unit defines how the product is measured (piece, hour, kg, etc.). Tax is the default tax percentage. Products in the catalog can be attached to deals using pd_add_product_to_deal.

Create a new product in the Pipedrive catalog with name, code (SKU), unit type, and tax rate
- **pd_deal_products**: Returns product name, quantity, item price, discount percentage, and total value per line. Use when the user asks "what products are on this deal?", needs to check line-item pricing, or wants to review the deal composition before closing.

Get all products attached to a specific deal with quantities, prices, and line-item totals
- **pd_deal_subscriptions**: Returns subscription details including recurring amount, billing cycle, and dates. Subscriptions track ongoing revenue tied to a deal for SaaS/recurring revenue businesses. Use when the user asks about recurring revenue, MRR/ARR, or subscription details on a deal.

Get recurring revenue subscriptions linked to a deal — MRR/ARR tracking for subscription-based businesses
- **pd_get_product**: Returns full product data including name, prices per currency, code, unit, tax, and custom fields. Use after searching to drill into a specific product for complete details.

Get complete details of a specific Pipedrive product by ID including all pricing, tax, and custom fields
- **pd_list_products**: Returns product name, unit price, code (SKU), unit type, and whether it is active. Use for product catalog browsing, inventory auditing, or when the user wants to see all available products.

List all products in the Pipedrive product catalog with names, prices, codes, and unit information
- **pd_search_products**: Returns product name, unit price, product code (SKU), unit type, and tax percentage. Use when the user wants to find a product, check pricing, or needs a product ID before attaching it to a deal.

Search Pipedrive products by name to find items in the product catalog with prices, codes, and unit types
- **pd_update_product**: Only specified fields change. Use when the user wants to rename a product, update its SKU code, or change pricing information.

Update an existing Pipedrive product — change name, code, pricing, or other catalog properties


## Installation & Usage

To install and use the **Pipedrive Products** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pipedrive-products](https://vinkius.com/mcp/pipedrive-products)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
