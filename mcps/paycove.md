# Paycove MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/paycove)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/paycove-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/paycove-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Automate smart quotes, invoice generation, and CPQ workflows directly from your CRM using AI agents.

## Description
Transform how your organization handles billing by giving your AI agent full control over Paycove's CPQ engine. Instead of manually moving deals from your CRM to accounting, your agent can instantly draft custom quotes, send automated invoices, and monitor payment statuses in real-time.

### What you can do
- Full CRUD for invoices and CPQ quotes
- Filter invoices by status (draft, sent, paid, overdue)
- Convert accepted quotes directly into invoices
- Manage product catalog and pricing
- Handle client billing profiles and track payments

### How it works
1. Log in to your Paycove account
2. Navigate to Settings > API & Integrations to generate a key
3. Let your AI agents start managing your Paycove billing operations directly via Vinkius

### Who is it for?
Ideal for finance teams, sales operations, and account managers needing instant, conversational access to Paycove billing data.


## Available Tools
- **check_paycove_status**: Verify connectivity
- **convert_quote_to_invoice**: Convert quote to invoice
- **create_client**: Create a client
- **create_invoice**: Create an invoice
- **create_product**: Create a product
- **create_quote**: Create a quote
- **get_client**: Get client details
- **get_invoice**: Get invoice details
- **get_product**: Get product details
- **get_quote**: Get quote details
- **list_clients**: List clients
- **list_invoices_by_status**: Filter invoices by status
- **list_invoices**: List all invoices
- **list_overdue_invoices**: List overdue invoices
- **list_payments**: List payments
- **list_products**: List products
- **list_quotes**: List all quotes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paycove** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all overdue invoices in Paycove"

**🤖 AI Agent:**
> You have 3 overdue invoices totaling $4,200. The oldest one is Invoice #INV-102 for Acme Corp. Should I prepare a follow-up email?

---

**👤 You:**
> "Convert quote Q-881 to an invoice"

**🤖 AI Agent:**
> I've successfully converted Quote Q-881 into Invoice INV-882. The invoice has been created in draft status. Do you want to review the line items before sending?

---

**👤 You:**
> "Check the payment status for client TechStart"

**🤖 AI Agent:**
> TechStart has 2 paid invoices and 1 sent invoice awaiting payment. Their last payment of $1,500 was received 2 days ago.


## Installation & Usage

To install and use the **Paycove** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/paycove](https://vinkius.com/mcp/paycove)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
