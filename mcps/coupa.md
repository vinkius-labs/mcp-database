# Coupa MCP Server

Manage purchase orders, invoices, suppliers, and procurement workflows on Coupa — the enterprise procurement platform.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/coupa)

## Overview
**Category:** industry-titans
**Tools Count:** 10

## Description
Connect your **Coupa** instance to any AI agent and manage procurement operations through natural conversation.

### What you can do

- **Purchase Orders** — Create, approve, and query POs with line-item detail, status tracking, and budget validation
- **Supplier Management** — Search and manage supplier records, compliance status, and performance scorecards
- **Invoices** — Process, query, and match invoices against POs with tolerance checks
- **Requisitions** — Submit and track purchase requisitions through approval chains
- **Contracts** — Query contract terms, expiration dates, and spend against contract limits
- **Expense Reports** — View and approve employee expense submissions
- **Budgets** — Check budget availability and spend analytics by cost center or department

### How it works

1. Subscribe to this server
2. Enter your Coupa instance URL and OAuth 2.0 credentials
3. Start managing procurement through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Procurement Officers** — create POs and manage supplier relationships through chat
- **AP Teams** — process and match invoices without navigating the Coupa UI
- **Finance Controllers** — monitor budget utilization and spend analytics by conversation
- **Category Managers** — query contracts and supplier performance scorecards rapidly


## Available Tools
- **approve_purchase_order**: Touches workflow and authorization boundary states.

Approve a pending purchase order
- **create_purchase_order**: Resolves supplier links, line items, and accounting allocations from the provided JSON payload.

Create a new purchase order
- **get_purchase_order**: Touches financial, supplier, and shipping boundary data.

Get details for a specific purchase order
- **get_supplier_details**: Get full profile for a specific supplier
- **list_contracts**: Resolves contract terms, validity periods, and associated suppliers.

List active procurement contracts
- **list_invoices**: Resolves invoice numbers, vendor names, payment statuses, and due dates.

List invoices and their payment status
- **list_purchase_orders**: Resolves PO numbers, supplier names, total amounts, and statuses (e.g., draft, ordered).

List purchase orders
- **list_requisitions**: Resolves requestor names, requested items, and current approval step in the workflow.

List purchase requisitions and their approval state
- **list_suppliers**: Resolves supplier legal names, tax IDs, contact information, and payment terms.

List or search for suppliers
- **query_coupa_resource**: Resolves raw JSON data from the specified API boundary.

Access any Coupa REST API resource directly


## Installation & Usage

To install and use the **Coupa** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coupa](https://vinkius.com/mcp/coupa)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
