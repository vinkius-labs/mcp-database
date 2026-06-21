# PrestaShop MCP Server

Bring your PrestaShop store to your AI — orchestrate orders, extract deep product metadata, and track inventory stock levels natively via chat.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/prestashop)

## Overview
**Category:** ecommerce
**Tools Count:** 10

## Description
Empower your AI agents to directly manage and analyze your **PrestaShop** eCommerce operations. Using the official Webservice API, your LLMs can scan live orders, inspect nested product XMLs, and monitor available stock without touching the back-office dashboard.

### What you can do

- **Order Logistics** — Instruct the AI to fetch `list_orders` or dig into a specific cart dropping absolute constraints via `get_order` to understand what was purchased
- **Product Catalog** — Pull arrays containing precise SKU data, category mappings, and pricing logic (`list_products`, `get_product`)
- **Stock Management** — Find out exactly how many units are permitted for checkout operations by retrieving native stock arrays (`list_stock`)
- **CRM & Addresses** — Query your database identifying customer histories (`list_customers`) correlated with absolute dispatch matrices (`list_addresses`)

### How it works

1. Subscribe to this MCP server
2. Provide your PrestaShop URL and your Webservice Key
3. Start mapping your e-commerce operations in Claude, Cursor, or any compatible client

No exporting CSVs or navigating XML trees manually. When a customer complains about an order, ask 'Retrieve Order ID 452 and list its items'. The AI reads the native integration flawlessly.

### Who is this for?

- **E-commerce Managers** — evaluate order volumes, check inventory depths, and read category structures instantly
- **Frontend Developers** — ask the AI to map specific product IDs into JSON arrays when building headless frontends
- **Support Teams** — track physical delivery addresses mapping direct customer disputes without accessing the admin panel


## Available Tools
- **list_products**: Use the `limit` parameter string to bound results (e.g., `0,20`). Native XML responses are parsed and converted to structured arrays.

List PrestaShop products with full details, retrieving items from the open-source eCommerce catalog
- **get_product**: Get an individual PrestaShop product by ID, returning full pricing, descriptions, and category associations
- **list_orders**: Limits response arrays via bounds (e.g., `0,20`). Critical for scanning recent sales history mapped directly against specific customer IDs.

List PrestaShop active orders retrieving order references, current fulfillment statuses, and totals
- **get_order**: Maps raw Webservice XML nodes into consumable arrays.

Get PrestaShop nested order by explicit ID, tracing line items, billing/shipping boundaries, and payment success paths
- **list_customers**: Limits response arrays via bounds (e.g., `0,20`). Maps basic CRM points for subsequent order correlations.

List PrestaShop customers tracking emails, first and last names, and account creation dates
- **list_categories**: List all PrestaShop root and child categories dictating store navigation geometry
- **list_addresses**: Limits response arrays via bounds (e.g., `0,20`). Used to analyze spatial destination data linked implicitly to customers and orders.

List physical PrestaShop customer/order addresses mapping delivery logistics lines
- **list_stock**: Resolves specific stock trace items which dictate the physical inventory logic overriding standard product rules.

List PrestaShop available stock quantities mapping exact units over specific complex item structures
- **get_stock**: Get PrestaShop specific stock quantity node explicitly by constrained resource ID
- **list_currencies**: List all active currencies configured and accepted implicitly within the target store interface


## Installation & Usage

To install and use the **PrestaShop** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prestashop](https://vinkius.com/mcp/prestashop)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
