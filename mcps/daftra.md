# Daftra MCP Server

Equip your AI agent to manage your ERP, accounting, and client relations directly via the Daftra API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/daftra)

## Overview
**Category:** erp-operations
**Tools Count:** 10

## Description
Integrate **Daftra**, the comprehensive cloud-based ERP and accounting software, directly into your AI workflow. Manage your clients, monitor invoices and estimates, and track business expenses using natural language.

### What you can do

- **Client Management** — List, search, and retrieve full profiles and interaction history for your clients.
- **Billing Oversight** — Monitor sales invoices and price estimates to stay on top of your revenue.
- **Expense Tracking** — Track and retrieve recorded business expenses across your organization.
- **Inventory & Services** — List products and services in your inventory directly via chat.

### How it works

1. Connect the Daftra integration to your AI assistant.
2. Authorize using your Daftra API Key and portal Subdomain.
3. Orchestrate your business operations and accounting through intuitive conversation.

### Who is this for?

- **Business Owners** — Quickly check invoice statuses and client details on the go.
- **Accountants** — Audit expenses and monitor billing cycles via chat.
- **Sales Teams** — Research client history and manage new lead profiles during planning.


## Available Tools
- **create_client**: Resolves the newly generated client ID. Mutates the client and contact database state.

Add a new client to the ERP database
- **get_client_details**: Resolves detailed contact info and outstanding balances. Touches the granular CRM boundary.

Get full profile and history for a specific client
- **get_invoice_details**: Resolves line items, tax details, and payment history. Interacts with the detailed billing boundary.

Get full details for a specific sales invoice
- **get_site_metadata**: Resolves site identifiers and organizational settings. Interacts with the system configuration boundary.

Retrieve general settings and metadata for your Daftra site
- **list_clients**: Resolves client IDs, business names, and contact emails. Interacts with the client management boundary.

List all clients in your Daftra account
- **list_estimates**: Resolves estimate IDs, dates, and amounts. Interacts with the sales pipeline and quoting boundary.

List all price estimates and quotes
- **list_expenses**: Resolves expense IDs, categories, and amounts. Touches the accounting and expense tracking boundary.

List all recorded business expenses
- **list_invoices**: Resolves invoice IDs, numbers, totals, and payment statuses. Touches the financial and sales boundary.

List all sales invoices
- **list_inventory_products**: Resolves product IDs, names, and pricing. Interacts with the inventory management boundary.

List all products and services in the inventory
- **search_clients_by_name**: Resolves matching client profiles. Touches the search and discovery boundary.

Search for a client by name keyword


## Installation & Usage

To install and use the **Daftra** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/daftra](https://vinkius.com/mcp/daftra)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
