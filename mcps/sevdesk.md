# sevDesk MCP Server

Empower your AI with direct read and write access to sevDesk to autonomously manage invoices, CRM contacts, sales orders, vouchers, and accounting records.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sevdesk)

## Overview
**Category:** customer-relationship-management
**Tools Count:** 15

## Description
Grant your conversational AI (like Claude or Cursor) the power of a dedicated German accounting clerk. The **sevDesk MCP** transforms your LLM into a sophisticated financial nexus capable of creating invoices, querying past-due credit notes, recording vouchers, and tracking your CRM endpoints dynamically. Stop wrestling with browser-based accounting dashboards and let your AI manage your bookkeeping automatically.

### What you can do

- **Client & Supplier CRM Mastery** — Read the entire client database via `list_contacts`, retrieve detailed metadata for specific IDs (`get_contact`), or seamlessly register brand new vendors via `create_contact`
- **Autonomous Invoicing & Orders** — Fetch paginated ledger lists using `list_invoices` or `list_orders`, and delve deep into line items, calculated taxes, and due statuses directly using `get_invoice` and `get_order`
- **Inventory & Service Architecture** — Monitor available billable components via `list_parts`, inspect standard pricing, and introduce novel catalog options autonomously via `create_part`
- **Accounting Governance** — Keep strict tabs on your chart of accounts with `list_accounting_types` while verifying associated business inlets securely using `list_bank_accounts`
- **Voucher & Credit Auditing** — Consolidate physical receipts through `list_vouchers` and trace structural adjustments flawlessly by scanning `list_credit_notes`

### How it works

1. Install this module directly into your MCP-compatible IDE or conversational context
2. Establish the secure connection effortlessly by injecting your 32-character hexadecimal `sevDesk API Token`
3. Engage your AI explicitly: "What's the net total on invoice #392911, and who is the attached client?"

### Who is this for?

- **Freelancers & Solopreneurs** — quickly ask your agent to draft new customer records and extract pending invoice tallies without leaving the editor
- **Financial Auditors** — instruct the AI to cross-reference registered parts and orders against generated credit notes natively
- **Agency Managers** — effortlessly check current bank configuration parameters and available accounting categories entirely via conversational prompts


## Available Tools
- **list_contacts**: Lists all contacts (customers, suppliers) in sevDesk
- **get_contact**: Retrieves details for a specific contact
- **create_contact**: Category 3 for customers, 4 for suppliers.

Creates a new contact (customer or supplier) in sevDesk
- **list_invoices**: Lists all invoices with embedded contact data
- **get_invoice**: Retrieves details for a specific invoice, including line items and tax
- **list_credit_notes**: Lists all credit notes
- **get_credit_note**: Retrieves details for a specific credit note
- **list_orders**: Lists all sales orders
- **get_order**: Retrieves details for a specific order
- **list_vouchers**: Lists all vouchers (incoming/outgoing receipts)
- **list_parts**: Lists all parts (products and services) in the catalog
- **get_part**: Retrieves details for a specific part
- **create_part**: Creates a new part or service in the catalog
- **list_accounting_types**: Lists all accounting types (Chart of Accounts)
- **list_bank_accounts**: Lists company bank accounts


## Installation & Usage

To install and use the **sevDesk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sevdesk](https://vinkius.com/mcp/sevdesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
