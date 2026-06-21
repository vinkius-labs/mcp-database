# Salesforce Commerce Cloud MCP Server

Manage products, orders, price books, and catalog operations through natural conversation with your Salesforce Commerce data.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/salesforce-commerce-cloud)

## Overview
**Category:** industry-titans
**Tools Count:** 8

## Description
Connect **Salesforce Commerce** to any AI agent.

### What you can do
- **Products** — Search by name/code, filter by family, update catalog items
- **Orders** — Search by number/account, filter by status, view line items
- **Price Books** — List price books and view pricing entries

### Who is this for?
- **E-commerce Managers** — Catalog operations via conversation
- **Order Fulfillment** — Track orders without admin access
- **Product Teams** — Update pricing and status instantly


## Available Tools
- **sf_order_items**: Returns product name, quantity, unit price, total price, and description per line item. Use when the user asks "what is in this order?", needs to review order composition, or wants to verify pricing before activation.

Get all line items of a specific Salesforce order — products, quantities, unit prices, and total prices per item
- **sf_orders_by_status**: Use for order management: "how many draft orders need activation?", "show all activated orders", or for revenue analysis by order status.

Get Salesforce orders filtered by status (Draft or Activated) for order management and fulfillment tracking
- **sf_pricebook_entries**: Returns product name, product code, unit price, currency, and active status. Price book entries define the actual price of a product in a specific context (channel, region, tier). Use to check pricing, compare across price books, or verify product availability in a specific price book.

Get all product price entries within a specific price book — products with their unit prices and active status
- **sf_products_by_family**: Returns products within a category (e.g., "Hardware", "Software", "Services"). Use when the user asks about products in a specific category, wants a category-level view, or needs to browse the catalog by family.

Get all active products within a specific product family for category-level catalog browsing
- **sf_list_pricebooks**: Returns price book name, description, active status, and IsStandard flag. Every Salesforce org has a Standard Price Book. Additional price books allow different pricing for channels, regions, or customer tiers (e.g., "Partner Pricing", "Enterprise Discount"). Use to find price book IDs before viewing entries.

List all price books in Salesforce with name, description, active status, and whether it is the standard price book
- **sf_search_orders**: Returns order number, account name, status (Draft/Activated), total amount, effective date, and order owner. Orders represent confirmed customer transactions. Use when the user asks about customer orders, wants to look up a specific order number, or needs to review order history.

Search Salesforce orders by order number or account name to find transactions with status, total, and dates
- **sf_search_products**: Returns product name, product code (SKU), product family, description, and whether the product is active. Products define what can be sold — they are linked to price books for pricing. Use when the user asks about product catalog, wants to find a specific product, or needs product IDs for orders.

Search the Salesforce product catalog by name or product code to find items with family, description, and active status
- **sf_update_product**: Common operations: set IsActive to false to discontinue a product, change Family to reclassify, update Description, or rename. Only specified fields change.

Update a product in the Salesforce catalog — change name, description, active status, product code, or family


## Installation & Usage

To install and use the **Salesforce Commerce Cloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salesforce-commerce-cloud](https://vinkius.com/mcp/salesforce-commerce-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
