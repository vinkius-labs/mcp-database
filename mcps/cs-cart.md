# CS-Cart MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cs-cart)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cs-cart-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cs-cart-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage e-commerce and marketplaces via CS-Cart — track products and orders, handle customer data, audit vendors, and monitor taxes directly from any AI agent.

## Description
Connect your **CS-Cart** or **Multi-Vendor** store to any AI agent and take full control of your e-commerce platform and marketplace operations through natural conversation.

### What you can do

- **Product Orchestration** — List products and retrieve intricate details including precise pricing, feature combinations, and stock options limitlessly
- **Order Monitoring** — Get an overview of recent incoming orders or detailed line-item lookups including billing/shipping addresses and payment details
- **Marketplace Management** — Retrieve active seller companies (Vendors) operating on your Multi-Vendor platform and verify their operational limits
- **Customer Oversight** — List and search registered customers, administrators, and vendor users to manage organizational permissions natively
- **Tax & Shipping Audit** — Lookup configured delivery options and carrier rates, and retrieve VAT/Tax configurations from the platform strictly
- **Taxonomy & Statuses** — Identify global category trees and monitor custom order state mappings (e.g., Paid, Shipped) to verify workflow consistency

### How it works

1. Subscribe to this server
2. Enter your CS-Cart Store URL, Admin Email, and API Key (found in your User Profile under the API Access tab)
3. Start managing your e-commerce store from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Store Owners** — monitor sales volume and audit inventory levels without navigating complex PHP-based admin panels
- **Marketplace Operators** — manage vendor lists and verify seller statuses across thousands of storefronts using natural language
- **Customer Support** — look up order details and shipping methods to resolve billing and delivery inquiries faster
- **Accounting Teams** — verify tax rules and reconcile order totals directly from the workspace


## Available Tools
- **list_products**: Resolves product IDs, names, prices, stock levels, and associated vendor identifiers.

List CS-Cart products. CS-Cart is a popular multi-vendor B2B/B2C marketplace platform
- **get_product**: Touches feature combinations, tax rules, delivery options, and multi-vendor pricing boundary data.

Get CS-Cart product by ID. Returns full details: price, features, options
- **list_orders**: Resolves order totals, payment statuses, shipping methods, and timestamps for recent transactions.

List CS-Cart orders. Returns order details, totals, statuses, and vendor mappings
- **get_order**: Touches line-item details, applied taxes, shipping costs, and customer billing boundary data.

Get CS-Cart order by ID. Returns line items, billing/shipping addresses
- **list_users**: Resolves user roles (Customer, Admin, Vendor), email addresses, and account creation dates.

List CS-Cart users/customers
- **list_categories**: Resolves category names, IDs, parent-child relationships, and SEO identifiers.

List CS-Cart product categories
- **list_vendors**: Resolves vendor names, company profiles, contact info, and current status boundaries.

List CS-Cart vendors/companies (for Multi-Vendor edition)
- **list_shippings**: Resolves shipping carrier names, configured rates, and supported delivery regions.

List CS-Cart shipping methods
- **list_taxes**: Resolves tax names, percentage rates, and geographic application rules boundary data.

List CS-Cart tax rules and rates
- **list_statuses**: Resolves human-readable status names and their internal system codes.

List CS-Cart order statuses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CS-Cart** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 products added to my store"

**🤖 AI Agent:**
> I found 5 recent products. Highlights include 'Modern Desk Lamp' ($45.00) and 'Ergonomic Office Chair' ($299.00). Would you like to see the full inventory details for any of these?

---

**👤 You:**
> "What is the status of order #987?"

**🤖 AI Agent:**
> Order #987 is currently 'Paid' (Status Code: P). It contains 2 items for a total of $120.00. The shipping method selected is 'FedEx Ground'.

---

**👤 You:**
> "List all active vendors in my marketplace"

**🤖 AI Agent:**
> I found 3 active vendors: 'TechWorld Solutions', 'Green Garden Supplies', and 'Fashion Hub'. Each vendor has their own storefront and product catalog on your platform.


## Installation & Usage

To install and use the **CS-Cart** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cs-cart](https://vinkius.com/mcp/cs-cart)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
