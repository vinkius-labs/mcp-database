# Zoho Invoice MCP Server

Manage billing invoices, estimates, and customer contacts via the Zoho Invoice API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-invoice)

## Overview
**Category:** ecommerce
**Tools Count:** 7

## Description
Connect your **Zoho Invoice** account to any AI agent to streamline your business billing and client management. This MCP server enables your agent to interact with professional invoices, quotes (estimates), and customer data directly from natural language interfaces.

### What you can do

- **Invoicing Control** — List, retrieve, and create professional invoices for your products and services
- **Estimate Oversight** — Access all quotes and price approximations sent to your customers to track sales leads
- **Item Management** — Query your product and service catalog, including pricing and metadata
- **Customer CRM** — Manage detailed customer profiles and retrieve their contact information instantly
- **Multi-Business Support** — List all organizations associated with your account and manage invoicing data by organization ID

### How it works

1. Subscribe to this server
2. Enter your Zoho Client ID, Client Secret, and Data Center Domain
3. Start managing your billing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Freelancers & Small Businesses** — Quickly generate invoices and check payment statuses via natural language
- **Billing Specialists** — Automate the retrieval of estimates and maintain customer records effortlessly
- **Developers** — Integrate professional invoicing data and billing automation into your custom workflows


## Available Tools
- **list_invoice_contacts**: List all contacts (customers)
- **create_new_invoice**: Requires a JSON body with invoice details.

Create a new invoice
- **list_estimates**: List all estimates (quotes) for an organization
- **get_invoice_details**: Get details for a specific invoice
- **list_invoices**: List all invoices for an organization
- **list_invoice_items**: List all items (products/services)
- **list_organizations**: Use this to identify the organization ID for other calls.

List all Zoho Invoice organizations


## Installation & Usage

To install and use the **Zoho Invoice** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-invoice](https://vinkius.com/mcp/zoho-invoice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
