# Daftra MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/daftra)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/daftra-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/daftra-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Equip your AI agent to manage your ERP, accounting, and client relations directly via the Daftra API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Daftra** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all unpaid invoices from this month."

**🤖 AI Agent:**
> I've found 5 unpaid invoices for this month, totaling $2,500. The largest is for 'Global Logistics' ($1,200). Would you like to see the details for any of them?

---

**👤 You:**
> "Search for client 'John Smith' and show his contact details."

**🤖 AI Agent:**
> I found John Smith. He is associated with 'Alpha Corp'. His email is john.smith@example.com and his phone number is +1-555-0123. Should I check his recent invoice history?

---

**👤 You:**
> "List all business expenses recorded in the last 7 days."

**🤖 AI Agent:**
> There are 3 expenses recorded this week: 'Office Supplies' ($50), 'Travel - Client Meeting' ($200), and 'Internet Service' ($80). Would you like a breakdown by category?


## Installation & Usage

To install and use the **Daftra** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/daftra](https://vinkius.com/mcp/daftra)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
