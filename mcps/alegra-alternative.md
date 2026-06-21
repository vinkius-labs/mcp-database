# Alegra MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/alegra-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/alegra-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/alegra-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Automate cloud accounting via Alegra — issue invoices, manage contacts, track inventory, and monitor bank accounts from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Alegra** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 invoices and show me which ones are still unpaid."

**🤖 AI Agent:**
> I found 5 recent invoices. 3 are fully paid: #FE-1204 ($2,350,000 COP), #FE-1203 ($890,000 COP), #FE-1200 ($1,560,000 COP). 2 remain unpaid: #FE-1202 ($3,200,000 COP, due in 3 days — client: Tech Solutions SAS) and #FE-1201 ($750,000 COP, overdue by 5 days — client: Distribuidora Norte Ltda). Should I pull the contact details for the overdue client?

---

**👤 You:**
> "Create an invoice for client ID 42 with 3 units of item 15 at $50,000 COP each."

**🤖 AI Agent:**
> Invoice created successfully! Factura Electrónica #FE-1205 has been issued to 'Importadora Global SAS' (NIT: 900.123.456-7) for $150,000 COP + IVA 19% = $178,500 COP total. DIAN electronic validation is pending and will complete within minutes. Would you like to send it by email?

---

**👤 You:**
> "Show me all IVA tax rates configured in my Alegra account."

**🤖 AI Agent:**
> Your account has 5 tax configurations: IVA General (19%), IVA Reducido (5%), IVA Excluido (0%), ReteFuente (3.5% — applied on purchases over $1,165,000 COP), and ReteICA Bogotá (0.414%). All are active and properly mapped to their DIAN codes. Need me to check which items have which taxes assigned?


## Installation & Usage

To install and use the **Alegra** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alegra-alternative](https://vinkius.com/mcp/alegra-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
