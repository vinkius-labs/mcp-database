# Alegra MCP Server

Automate cloud accounting via Alegra — issue invoices, manage contacts, track inventory, and monitor bank accounts from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/alegra-alternative)

## Overview
**Category:** erp-operations
**Tools Count:** 14

## Description
Connect your **Alegra** cloud accounting platform to any AI agent and manage your entire financial operation through natural conversation.

### What you can do

- **Invoice Management** — Create, list, and inspect sales invoices with DIAN electronic invoicing compliance for Colombia, including tax breakdowns and payment tracking
- **Contact Directory** — Manage your complete client and supplier database with NIT/CC identification, fiscal regime classification, and outstanding balances
- **Inventory Control** — Browse products and services, check stock per warehouse, manage pricing, and create new catalog items
- **Expense Tracking** — List supplier bills, purchase invoices, and track payable obligations across your accounting periods
- **Payment Monitoring** — Query received payments, bank account balances, and reconciliation status in real-time
- **Tax Configuration** — Access IVA rates, retention types, ICA taxes, and country-specific tax parameters

### How it works

1. Subscribe to this server
2. Enter your Alegra email and API token
3. Start managing your accounting from Claude, Cursor, or any MCP-compatible client

Your AI becomes a dedicated virtual accountant — instantly answering financial queries that would normally require navigating multiple dashboard screens.

### Who is this for?

- **Small Business Owners** — issue invoices and check cash flow without opening the accounting dashboard
- **Accountants** — query client data, tax configurations, and payment histories programmatically
- **Operations Managers** — track inventory levels and supplier bills across multiple warehouses


## Available Tools
- **create_contact**: For Colombian tax compliance (DIAN), include the identification type (NIT, CC, CE) and number. The contact can be tagged as client, supplier, or both.

Create a new contact (client or supplier)
- **create_invoice**: For Colombian DIAN electronic invoicing compliance, the invoice is automatically validated and stamped. Requires a client ID and at least one line item with the product/service details.

Create a new sales invoice
- **create_item**: The item can be used in future invoices, purchase orders, and inventory tracking. Set the type to "product" for physical goods with stock management or "service" for intangible services.

Create a new inventory item
- **get_contact**: Get full details of a specific contact
- **get_invoice**: Get full details of a specific invoice
- **get_item**: Get full details of a specific inventory item
- **list_bank_accounts**: List all bank accounts
- **list_bills**: List supplier bills and purchase invoices
- **list_contacts**: Each contact includes their legal name, NIT/CC identification, address, phone, email, and whether they are classified as a client, supplier, or both.

List all contacts (clients and suppliers)
- **list_invoices**: List sales invoices
- **list_items**: List all inventory items
- **list_payments**: List received payments
- **list_taxes**: List configured tax rates
- **list_warehouses**: List all warehouses


## Installation & Usage

To install and use the **Alegra** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alegra-alternative](https://vinkius.com/mcp/alegra-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
