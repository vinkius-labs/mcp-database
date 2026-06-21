# Odoo eCommerce MCP Server

List shop products, manage eCommerce orders, browse categories and customers — Odoo Website & eCommerce through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/odoo-ecommerce)

## Overview
**Category:** industry-titans
**Tools Count:** 6

## Description
Connect **Odoo ERP** to any AI agent — manage your entire business without switching tabs.

### What you can do
- **CRM** — Search and create leads, track opportunities through your pipeline
- **Contacts** — Find individual contacts and companies, create new partners
- **Sales** — List and manage sales orders with full order details
- **Notes** — Add comments and notes to any record in your Odoo instance

### Who is this for?
- **Sales Teams** — CRM pipeline at your fingertips through AI
- **Account Managers** — Quick access to contact and company information
- **Operations** — Monitor sales orders without switching screens
- **Odoo Administrators** — Query any module through natural conversation


## Available Tools
- **odoo_list_product_categories**: category records with full hierarchy path. Use when the user asks about product organization or needs category IDs for product creation.

List the product category tree used to organize products in the Odoo shop and inventory
- **odoo_list_shop_customers**: partner records where customer_rank > 0. Returns name, email, phone, city, country. Use for customer analytics or to find buyer contact info.

List eCommerce customers who have made purchases, with contact details and location
- **odoo_list_ecommerce_orders**: order records where website_id is set — online store orders only. Returns order number, customer, total, status, website, and date. Use when the user asks about online sales or eCommerce revenue.

List orders placed through the Odoo Website storefront with customer, amount, and status
- **odoo_list_shop_products**: template records where sale_ok=true. Returns product name, sale price, category, type, SKU, stock qty, and website publish status. Use when the user asks about the product catalog or shop inventory.

List products available on the Odoo eCommerce shop with prices, stock, and publish status
- **odoo_list_websites**: Returns website name, domain, and creation date. Use when the user asks about available storefronts.

List all Odoo websites configured — useful for multi-website or multi-brand setups
- **odoo_search_shop_products**: template by name where sale_ok=true. Returns matching products with price, category, type, SKU, stock, and publish status. Use to find a specific product in the online shop.

Search the Odoo eCommerce product catalog by name with prices, stock, and category


## Installation & Usage

To install and use the **Odoo eCommerce** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/odoo-ecommerce](https://vinkius.com/mcp/odoo-ecommerce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
