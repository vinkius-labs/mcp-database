# Uniconta MCP Server

Automate ERP workflows via Uniconta — retrieve debtors, query invoices, manage GL accounts, and list inventory directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/uniconta)

## Overview
**Category:** erp-operations
**Tools Count:** 8

## Description
Connect your **Uniconta ERP** to any AI agent and take full enterprise control over global accounting ledgers, debtor/creditor relationships, and billing tracking securely natively via chat.

### What you can do

- **Client & Debtor Tracking** — List actively registered customers grabbing exact RowIDs or drill down into metadata isolating specific contact profiles via `get_debtor_details`
- **Invoicing & Billing Audits** — Fetch hundreds of active invoices tracking open debtor balances globally without manual filtering through ERP dashboards
- **General Ledger (GL) Supervision** — Query daily journals pulling transaction histories checking if the books map accurately
- **Inventory Verification** — Monitor product catalogs recovering item records, prices, and available stock configurations simultaneously

### How it works

1. Subscribe manually to this core server context
2. Introduce your personal Uniconta `Username`, `Password`, and targeting `Company ID`
3. Start mapping live invoice ledgers directly across Claude or your preferred integrated workspace

No digging into complicated Uniconta visual reports to pull a customer's address. Ask the AI and fetch exact company data natively instantly.

### Who is this for?

- **Financial Auditors** — request the AI to grab 'list_daily_journals' assessing transaction flows within 15 seconds without exporting massive Excel CSVs
- **Sales & Logistics** — swiftly verify stock numbers leveraging 'list_inventory_items' right from a chat window when building orders
- **Account Executives** — call down 'get_debtor_details' immediately before meetings checking exactly if their previous invoices remain unpaid


## Available Tools
- **get_debtor_details**: Retrieves details for a specific debtor
- **list_gl_accounts**: Lists all General Ledger (GL) accounts in Uniconta
- **list_creditors**: Lists all creditors (vendors) registered in the ERP
- **list_debtors**: Lists all debtors (customers) registered in the ERP
- **list_employees**: Lists all employees registered in the Uniconta account
- **list_debtor_invoices**: Lists all debtor invoices issued by the company
- **list_inventory_items**: Lists all inventory items in the product catalog
- **list_daily_journals**: Lists all General Ledger daily journals


## Installation & Usage

To install and use the **Uniconta** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uniconta](https://vinkius.com/mcp/uniconta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
