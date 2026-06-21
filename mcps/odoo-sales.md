# Odoo Sales MCP Server

Create quotations, confirm sales orders, manage products and pricelists — Odoo Sales pipeline through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/odoo-sales)

## Overview
**Category:** erp-operations
**Tools Count:** 8

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
- **odoo_confirm_order**: order, transitioning it from "draft"/"sent" to "sale" state. This triggers downstream operations like delivery order creation and inventory reservation. Use when the user says a quote is approved or wants to confirm an order.

Confirm a draft quotation, converting it into an active sales order ready for fulfillment
- **odoo_create_quotation**: order in "draft" state with the specified customer and order lines. The partnerId must be an existing res.partner ID. Lines must be a JSON array where each element has product_id (existing product.template ID), product_uom_qty (quantity), and price_unit (unit price). Example lines: [{"product_id": 5, "product_uom_qty": 2, "price_unit": 100.00}]

Create a new quotation for a customer with product lines, quantities, and unit prices
- **odoo_get_order_lines**: order.line records for the given order. Returns each line with product name, quantity, unit price, and subtotal. Use when the user wants to see what products are in an order, verify quantities, or check line-level pricing.

Get the individual line items (products, quantities, prices) of a specific sales order
- **odoo_get_sales_order**: order record with all key fields: customer, status, amounts, salesperson, dates. Use after finding an order via list/search to drill down into its details. The ID is the numeric Odoo database ID (not the order number like S00042).

Get the complete details of a specific sales order or quotation by its numeric ID
- **odoo_list_pricelists**: pricelist records. Pricelists define pricing rules for different customer segments, currencies, or regions. Returns pricelist name, currency, and whether it is active. Use when the user asks about available pricing tiers or currency-specific pricing.

List all configured pricelists in Odoo with their currencies and active status
- **odoo_list_quotations**: order records in "draft" or "sent" state — these are quotations pending customer acceptance. Returns quotation number, customer name, total amount, salesperson, currency, and creation date. Use when the user asks about pending quotes, proposals awaiting approval, or the current quotation pipeline.

List all draft and sent quotations in Odoo that have not yet been confirmed as sales orders
- **odoo_list_sales_orders**: order records in "sale" or "done" state — these are confirmed orders being fulfilled or already completed. Returns order number, customer, total/untaxed amounts, salesperson, currency, and order date. Use when the user asks about active orders, confirmed sales, or order fulfillment status.

List confirmed and completed sales orders in Odoo with customer, amounts, and fulfillment status
- **odoo_search_products**: template records by name. Returns product name, sale price (list_price), cost price (standard_price), product type (consu/service/product), category, available stock quantity, and internal reference (SKU/code). Use when the user needs to find a product, check prices, or verify stock before creating a quotation.

Search the Odoo product catalog by name, returning prices, cost, category, stock, and SKU


## Installation & Usage

To install and use the **Odoo Sales** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/odoo-sales](https://vinkius.com/mcp/odoo-sales)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
