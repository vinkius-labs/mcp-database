# Zoho Books MCP Server

Manage invoices, estimates, and contacts via the Zoho Books API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-books)

## Overview
**Category:** erp-operations
**Tools Count:** 7

## Description
Connect your **Zoho Books** account to any AI agent to streamline your cloud accounting and billing operations. This MCP server enables your agent to interact with invoices, estimates, and customer contacts directly from natural language interfaces.

### What you can do

- **Invoicing Management** — List, retrieve, and create professional billing invoices for your clients
- **Estimate Tracking** — Access all quotes and proposals generated for your businesses to stay on top of sales
- **Inventory Visibility** — List the catalog of products and services sold across your organizations
- **Contact Oversight** — Manage customer and vendor profiles and retrieve their details instantly
- **Multi-Org Support** — List all businesses associated with your account and manage data by organization ID

### How it works

1. Subscribe to this server
2. Enter your Zoho Client ID, Client Secret, and Data Center Domain
3. Start managing your accounting from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Small Business Owners** — Quickly check invoice statuses and client balances via natural language commands
- **Accountants & Bookkeepers** — Automate the retrieval of financial records and maintain contact hygiene
- **Developers** — Integrate accounting data and billing automation into your daily development workflow


## Available Tools
- **list_books_contacts**: List all contacts (customers/vendors)
- **create_new_invoice**: Requires a JSON body with invoice details.

Create a new invoice
- **list_estimates**: List all estimates (quotes) for an organization
- **get_invoice_details**: Get details for a specific invoice
- **list_invoices**: List all invoices for an organization
- **list_inventory_items**: List all items (products/services)
- **list_organizations**: Use this to identify the organization ID for other calls.

List all Zoho Books organizations


## Installation & Usage

To install and use the **Zoho Books** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-books](https://vinkius.com/mcp/zoho-books)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
