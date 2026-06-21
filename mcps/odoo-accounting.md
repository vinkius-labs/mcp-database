# Odoo Accounting MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/odoo-accounting)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/odoo-accounting-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/odoo-accounting-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

List invoices, bills, payments, journal entries, and chart of accounts — Odoo Accounting through natural conversation.

## Description
Connect **Odoo ERP** to any AI agent — manage your entire business without switching tabs.

### What you can do
- **CRM** — Search and create leads, track opportunities through your pipeline
- **Contacts** — Find individual contacts and companies, create new partners
- **Sales** — List and manage sales orders with full order details
- **Notes** — Add comments and notes to any record in your Odoo instance

### Who is this for?
- **Sales Teams** — CRM pipeline at your fingertips through AI
- **Account Managers** — Quick access to contact and company information
- **Operations** — Monitor sales orders without switching screens
- **Odoo Administrators** — Query any module through natural conversation


## Available Tools
- **odoo_list_accounts**: account records ordered by code — the full General Ledger account structure. Returns account code + name (e.g., "1100 - Accounts Receivable"), account type (asset_receivable, liability_payable, income, expense, etc.), and whether the account supports reconciliation. Use when the user asks about the GL structure, needs an account code, or wants to understand the financial reporting hierarchy.

List the Chart of Accounts in Odoo showing account codes, names, types, and reconciliation settings
- **odoo_list_bills**: move records of type "in_invoice" (vendor bills). Returns bill number, vendor name, state, payment status, total amount, remaining balance, journal, and bill date. Use when the user asks about accounts payable, unpaid vendor bills, supplier invoices, or outstanding amounts owed to vendors.

List vendor bills (supplier invoices) in Odoo with amounts owed, payment status, and due dates
- **odoo_list_invoices**: move records of type "out_invoice" (customer invoices). Returns invoice number, customer name, state (draft/posted/cancel), payment status (not_paid/in_payment/paid), total amount, residual (remaining balance), journal, reference, and invoice date. Use when the user asks about outstanding invoices, accounts receivable, billing history, or unpaid customer balances.

List customer invoices in Odoo with amounts, payment status, journal, and due dates
- **odoo_list_journal_entries**: move records of type "entry" — these are manual accounting entries, not invoices or bills. Returns entry number, partner (if any), state (draft/posted), total, journal, reference, and date. Use when the user asks about accounting adjustments, depreciation entries, accruals, or manual GL postings.

List manual journal entries (accounting adjustments) in Odoo with amounts, journals, and posting dates
- **odoo_list_journals**: journal records — the logical groupings for accounting entries. Returns journal name, type (sale/purchase/bank/cash/general), short code, and currency. Use when the user asks about available journals, needs journal codes for entries, or wants to understand the accounting structure.

List all accounting journals (Sales, Purchase, Bank, Cash, Miscellaneous) configured in Odoo
- **odoo_list_payments**: payment records ordered by date. Returns payment reference, partner, state (draft/posted/sent/reconciled/cancelled), amount, journal (bank/cash), payment type (inbound=customer payment, outbound=vendor payment), and date. Use when the user asks about recent payments, cash flow activity, bank transactions, or payment reconciliation status.

List payment transactions in Odoo showing amounts, payment method, type (inbound/outbound), and reconciliation status
- **odoo_list_taxes**: tax records. Returns tax name, percentage amount, usage scope (sale/purchase/none), and active status. Use when the user asks about applicable tax rates, VAT/GST configurations, or needs to verify tax setups for invoicing.

List all tax configurations in Odoo showing tax name, rate, and whether it applies to sales or purchases


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Odoo Accounting** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for leads from the website"

**🤖 AI Agent:**
> 👥 **CRM Leads — Website**
| Name | Email | Stage | Revenue |
|---|---|---|---|
| Acme Corp | info@acme.com | Qualification | $15,000 |
| Beta Inc | hello@beta.io | Proposition | $8,500 |

---

**👤 You:**
> "Show recent sales orders"

**🤖 AI Agent:**
> 📋 **Sales Orders**
| SO# | Customer | Amount | Status |
|---|---|---|---|
| S00042 | Acme Corp | $12,500 | Confirmed |
| S00041 | Beta Inc | $3,200 | Draft |


## Installation & Usage

To install and use the **Odoo Accounting** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/odoo-accounting](https://vinkius.com/mcp/odoo-accounting)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
