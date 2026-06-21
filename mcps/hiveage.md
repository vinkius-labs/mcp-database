# Hiveage MCP Server

Automate online invoicing via Hiveage — manage invoices, estimates, and payments directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hiveage)

## Overview
**Category:** finance-accounting
**Tools Count:** 12

## Description
Connect your **Hiveage** account to any AI agent and take full control of your online invoicing, estimates, and customer network through natural conversation.

### What you can do

- **Invoicing Oversight** — List all invoices, retrieve detailed billing data using unique hash keys, and monitor payment status.
- **Estimate Management** — Access your quotations and estimates history to stay on top of pending deals.
- **Payment Recording** — Manually record payments against invoices directly from the chat interface.
- **Customer Network** — List and inspect connections (customers/vendors) in your business network.
- **Document Delivery** — Send invoices to your customers via email with a single command.
- **Tax & Item Visibility** — List saved billing items and tax profiles to ensure accurate invoicing.

### How it works

1. Subscribe to this server
2. Enter your Hiveage API Key and Subdomain
3. Start managing your billing from Claude, Cursor, or any MCP-compatible client

No more manual navigating through complex billing tabs. Your AI assistant acts as a dedicated Billing Manager or Accounts Receivable Specialist.

### Who is this for?

- **Freelancers** — instantly retrieve invoice statuses and record payments while working on projects.
- **Small Business Owners** — automate the process of checking for overdue invoices and sending reminders.
- **Accountants** — quickly list tax profiles and billing items for reconciliation.


## Available Tools
- **record_payment**: Pass details as a JSON string in "body_json" (requires amount, date, and payment_method).

Record a manual payment against an invoice
- **send_invoice_email**: Deliver an invoice to the customer via email
- **get_customer_details**: Get detailed profile information for a network connection
- **get_estimate_details**: Get detailed information about a specific estimate
- **get_invoice_details**: Get detailed information about a specific invoice
- **get_api_profile**: Retrieve information about the authenticated account
- **list_estimates**: List all estimates (quotations) in Hiveage
- **list_invoices**: Use this to monitor billing and find hash keys for specific invoice actions.

List all invoices in your Hiveage account
- **list_billing_items**: List saved items and services used for invoicing
- **list_customers**: List all connections (customers/vendors) in your network
- **list_invoice_payments**: List all payments recorded for a specific invoice
- **list_tax_profiles**: List all configured tax profiles


## Installation & Usage

To install and use the **Hiveage** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hiveage](https://vinkius.com/mcp/hiveage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
