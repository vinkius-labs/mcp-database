# Alegra MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/alegra-extended)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/alegra-extended-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/alegra-extended-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Handle your Latin American business accounting with electronic invoicing, expense tracking, and tax-ready financial reports.

## Description
Connect your **Alegra** account to any AI agent and simplify how you manage your professional billing, customer directory, and inventory through natural conversation.

### What you can do

- **Billing Management** — Create, list, and inspect sales invoices with detailed status tracking (open, paid, overdue).
- **Customer & Supplier CRM** — Manage your contacts, update profile data, and check individual transaction histories.
- **Inventory Control** — Query your product and service catalog to monitor stock levels and pricing metadata.
- **Financial Oversight** — Monitor received payments and track sales estimates/quotes sent to potential clients.
- **Organization Insights** — Retrieve company metadata and verify account configurations directly from the agent.
- **Operational Monitoring** — Check connectivity and manage your commercial ecosystem without leaving your workspace.

### How it works

1. Subscribe to this server
2. Enter your Alegra Email and API Token (found in your account settings)
3. Start managing your business finances from Claude, Cursor, or any MCP client

### Who is this for?

- **Small Business Owners** — quickly create invoices and check client balances via simple AI commands.
- **Finance & Admin Teams** — monitor payments and manage the contact directory directly from the workspace.
- **Operations Managers** — track inventory levels and verify service availability via the AI assistant.


## Available Tools
- **create_contact**: Create a new contact in Alegra
- **create_invoice**: Create a new sales invoice
- **get_contact_details**: Get details of a specific contact
- **get_invoice_details**: Get details of a specific invoice
- **get_item_details**: Get details of an inventory item
- **get_company_info**: Get Alegra company information
- **list_contacts**: List Alegra contacts (clients and suppliers)
- **list_estimates**: List estimates/quotes
- **list_invoices**: List sales invoices in Alegra
- **list_inventory_items**: List products and services
- **list_payments**: List recorded payments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Alegra** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active invoices in my Alegra account."

**🤖 AI Agent:**
> I've retrieved your invoices. You have 3 active sales documents: #INV-001 ($150.00, Paid), #INV-002 ($450.00, Open), and #INV-003 ($1,200.00, Overdue). Which one would you like more details on?

---

**👤 You:**
> "Show me the details for contact 'John Doe' (ID: 10293)."

**🤖 AI Agent:**
> I've fetched John Doe's profile. He is a 'Client' and has an outstanding balance of $450.00 from invoice #INV-002. Shall I retrieve his full contact history?

---

**👤 You:**
> "What is the stock level for 'Professional Desk'?"

**🤖 AI Agent:**
> Checking inventory... The 'Professional Desk' (ID: item_8823) currently has 15 units in stock. The unit price is $250.00. Would you like to create an invoice for this item?


## Installation & Usage

To install and use the **Alegra** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alegra-extended](https://vinkius.com/mcp/alegra-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
