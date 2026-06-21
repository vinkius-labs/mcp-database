# Zoho Invoice MCP Server

Create and send professional invoices, track payments, and manage expenses with free invoicing software that scales with your business.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-invoice-alternative)

## Overview
**Category:** finance-accounting
**Tools Count:** 12

## Description
Connect your **Zoho Invoice** account to any AI agent and simplify how you manage your professional billing, customer directory, and payment tracking through natural conversation.

### What you can do

- **Invoice Management** — Create, list, and send professional invoices, and retrieve detailed status (DRAFT, SENT, PAID).
- **Customer Directory** — Manage your client base, update contact details, and check outstanding balances or credit limits.
- **Payment Tracking** — Monitor received payments and track overdue invoices in real-time to keep your cash flow healthy.
- **Estimate Control** — Query and manage price estimates sent to clients before they become invoices.
- **Expense Monitoring** — List and track business expenses associated with specific projects or customers.
- **Operational Insight** — Retrieve high-level summaries of your billing activity directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Zoho Invoice Authtoken or OAuth credentials
3. Start invoicing directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Freelancers & Small Business Owners** — quickly create invoices and check client balances via simple AI commands.
- **Finance Teams** — monitor overdue payments and track expense records directly from the workspace.
- **Accountants** — retrieve transaction histories and verify customer metadata via the AI assistant.


## Available Tools
- **check_zoho_invoice_status**: Returns a status indicator and organization metadata to confirm valid credentials.

Verify Zoho Invoice API connectivity
- **create_contact**: The contact name is required. Optionally provide company name, email, and phone.

Create a new contact (customer) in Zoho Invoice
- **create_invoice**: Requires the customer_id and at least one line_item with name and rate. The invoice is created in DRAFT status by default.

Create a new invoice in Zoho Invoice
- **get_contact**: Get full details of a specific contact
- **get_invoice**: Get full details of a specific invoice
- **get_item**: Get full details of a specific item
- **list_contacts**: Optionally search by name. Returns contact names, IDs, emails, outstanding balances, and unused credits.

List all contacts (customers) in Zoho Invoice
- **list_estimates**: Optionally filter by status such as "draft", "sent", "invoiced", "accepted", or "declined".

List all estimates (quotes) in Zoho Invoice
- **list_expenses**: Returns expense dates, categories, amounts, vendors, and associated projects or customers.

List all tracked expenses
- **list_invoices**: Optionally filter by status such as "sent", "draft", "overdue", "paid", or "void". Returns invoice numbers, amounts, dates, and customer information.

List all invoices in Zoho Invoice
- **list_items**: List all items (products/services) in Zoho Invoice
- **list_payments**: Useful for tracking cash flow and reconciliation.

List all customer payments received


## Installation & Usage

To install and use the **Zoho Invoice** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-invoice-alternative](https://vinkius.com/mcp/zoho-invoice-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
