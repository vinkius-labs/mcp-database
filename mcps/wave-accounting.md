# Wave Accounting MCP Server

Manage customers, invoices, and accounting workflows on Wave — the money management tool for small businesses.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/wave-accounting)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **Wave Accounting** account to any AI agent and manage your business finances through natural conversation.

### What you can do

- **Customer Management** — List all registered customers, create new profiles, and update contact information directly from your agent
- **Invoice Lifecycle** — Create draft invoices, approve them for sending, and monitor their payment status (DRAFT, SAVED, PAID)
- **Deep Invoicing** — Retrieve full details for any invoice, including line items, taxes, totals, and public payment URLs
- **Financial Auditing** — Browse your customer base and billing activity to stay on top of your accounts receivable
- **Data Integrity** — Safely delete unfinalized draft invoices or obsolete customer records through simple chat commands
- **Business Insights** — Quickly find unique customer and invoice IDs required for complex accounting workflows

### How it works

1. Subscribe to this server
2. Enter your Wave Business ID and Access Token
3. Start managing your customers and invoices through Claude, Cursor, or any MCP-compatible client

No more manual data entry into complex accounting dashboards. Your AI agent becomes your financial assistant.

### Who is this for?

- **Small Business Owners** — automate invoice creation and manage customer lists without manual navigation
- **Freelancers & Solo-preneurs** — quickly check payment status and draft new billing documents through chat
- **Accountants & Bookkeepers** — audit customer records and monitor invoice statuses across different businesses
- **Sales Teams** — lookup customer details and verify billing information before closing deals


## Available Tools
- **approve_draft_invoice**: Finalizes a draft invoice, moving it to an unpaid/saved status
- **create_accounting_customer**: Provide name and email.

Creates a new customer record in Wave
- **create_draft_invoice**: Provide a customer ID and a JSON array of items.

Creates a new draft invoice in Wave
- **delete_accounting_customer**: This action is irreversible.

Permanently deletes a customer record
- **delete_draft_invoice**: Saved or paid invoices cannot be deleted via this endpoint.

Permanently deletes an unfinalized draft invoice
- **get_customer_details**: Retrieves details for a specific customer in Wave
- **get_invoice_details**: Retrieves full details for a specific Wave invoice
- **list_accounting_customers**: Lists customers registered in the Wave Accounting business
- **list_accounting_invoices**: ).

Lists invoices issued by the Wave business
- **update_customer_profile**: Provide the unique customer ID.

Updates the profile of an existing customer


## Installation & Usage

To install and use the **Wave Accounting** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wave-accounting](https://vinkius.com/mcp/wave-accounting)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
