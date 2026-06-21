# Moneybird MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moneybird-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Handle Dutch and European accounting with automated invoicing, bank reconciliation, and tax-ready financial reports.

## Description
Connect your **Moneybird** administration to any AI agent and manage Dutch accounting through natural conversation.

### What you can do

- **Sales Invoices** — Create, list, and send invoices to clients
- **Contacts** — Browse customers and suppliers
- **Products** — List product and service catalog
- **Financial Mutations** — Track bank transactions for reconciliation
- **Purchase Invoices** — List supplier invoices received
- **Recurring Invoices** — View automated recurring templates
- **Receipts** — List uploaded expense receipts
- **Ledger Accounts** — Browse accounting categories
- **Tax Rates** — List configured VAT/tax rates

### How it works

1. Subscribe to this server
2. Enter your Moneybird API Key and Administration ID
3. Start managing your books from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Freelancers** — automate invoice creation and sending
- **Accountants** — reconcile transactions and manage ledgers
- **Small Businesses** — track expenses and VAT


## Available Tools
- **check_api_health**: Verify Moneybird API connectivity
- **create_sales_invoice**: Requires a contact ID and line items.

Create a new draft invoice
- **list_crm_contacts**: List customers and suppliers
- **list_sales_invoices**: Can be filtered by status (e.g., draft, open, paid).

List sales invoices
- **list_ledger_accounts**: List accounting ledger categories
- **list_financial_mutations**: List bank transactions
- **list_catalog_products**: List products and services
- **list_purchase_invoices**: List received purchase invoices
- **list_expense_receipts**: List uploaded receipts
- **list_recurring_invoices**: List recurring invoice templates
- **list_tax_rates**: List configured tax/VAT rates
- **send_sales_invoice**: Send an invoice to the customer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moneybird** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List recent sales invoices and their statuses."

**🤖 AI Agent:**
> Sales Invoices: 5. 1) INV-2024-045 — Acme Corp, €1,200.00 (Status: Paid ✅). 2) INV-2024-046 — Beta Ltd, €450.00 (Status: Open, Due: Apr 30). 3) INV-2024-047 — Gamma Inc, €2,800.00 (Status: Draft). 4) INV-2024-048 — Delta BV, €89.00 (Status: Paid ✅). 5) INV-2024-049 — Epsilon, €340.00 (Status: Late ⚠️, Overdue 5 days).

---

**👤 You:**
> "Create a draft invoice for Beta Ltd with 2 line items."

**🤖 AI Agent:**
> Invoice created! ✅ ID: 890123456. Number: INV-2024-050. Contact: Beta Ltd. Items: 1) 'Consulting Hours' (10x €75.00 = €750.00). 2) 'Travel Expenses' (1x €120.00). Subtotal: €870.00. VAT 21%: €182.70. Total: €1,052.70. Status: Draft. Ready to send?

---

**👤 You:**
> "Show unreconciled bank transactions."

**🤖 AI Agent:**
> Financial Mutations (Unreconciled): 3. 1) +€1,200.00 from Acme Corp (Apr 20, Matches: INV-2024-045). 2) -€45.00 Office Supplies (Apr 18, No match ⚠️). 3) +€89.00 from Delta BV (Apr 15, Matches: INV-2024-048). Want to auto-reconcile the matched items?


## ❓ FAQ

**Q: Can I create and send invoices?**
Yes. Create draft invoices with contact ID and line items, then send them directly to the customer via the API.

**Q: How does Moneybird authentication work?**
Moneybird requires a Bearer **API Key** and an **Administration ID** against `moneybird.com/api/v2/{administrationId}/`.

**Q: Can I list bank transactions?**
Yes. Financial mutations (bank transactions) can be listed for reconciliation purposes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moneybird-alternative](https://vinkius.com/mcp/moneybird-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moneybird** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `moneybird-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moneybird** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moneybird-alternative": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
