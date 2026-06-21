# Bill.com MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/billcom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Equip your AI agent with direct access to BILL — manage invoices, approve payments, and track vendor bills without opening the AP dashboard.

## Description
Connect **BILL (Bill.com)** to your AI agent and streamline your accounts payable and receivable workflows conversationally.

### What you can do

- **Invoice Management** — List, create, and review vendor invoices with line-item details, due dates, and approval statuses.
- **Payment Approvals** — Check pending approvals, review payment runs, and track sent payments across your organization.
- **Vendor Directory** — Query your vendor database, view payment history, and manage vendor contacts.
- **AP/AR Analytics** — Get instant insights into outstanding payables, overdue invoices, and cash flow projections.

### How it works

1. Subscribe to the BILL integration on the marketplace.
2. Generate a Developer Key from your BILL account (Settings → Sync & Integrations → Manage Developer Keys).
3. Ask your AI agent to list invoices, check payment statuses, or review vendor bills.

### Who is this for?

- **AP/AR Managers** — Approve invoices and track payment runs without switching between email and the BILL dashboard.
- **Controllers & CFOs** — Get instant answers about outstanding payables and cash flow commitments during financial reviews.
- **Bookkeepers** — Reconcile vendor payments and review invoice details directly from your workflow.


## Available Tools
- **list_vendors**: List all vendors
- **get_company_profile**: Get company profile
- **get_vendor**: Get vendor details
- **create_vendor**: Create a new vendor
- **list_bills**: List all bills
- **get_bill**: Get bill details
- **create_bill**: Create a new bill
- **list_invoices**: List all invoices
- **list_payments**: List all payments
- **list_customers**: List all customers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bill.com** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all unpaid invoices from this month."

**🤖 AI Agent:**
> I found 7 unpaid invoices totaling $34,200. The largest is from Acme Consulting ($12,500, due in 3 days). Two invoices are overdue by more than 15 days.

---

**👤 You:**
> "What payments are pending approval?"

**🤖 AI Agent:**
> There are 3 payments pending your approval: SaaS Vendor ($4,500), Office Supplies Co ($890), and Cloud Hosting Inc ($7,200). Total pending: $12,590.

---

**👤 You:**
> "List all vendors we've paid more than $10,000 this quarter."

**🤖 AI Agent:**
> I found 5 vendors with payments exceeding $10,000 this quarter: AWS ($38,400), Gusto ($112,000), WeWork ($24,000), HubSpot ($15,600), and Notion ($11,200).


## ❓ FAQ

**Q: How do I get my BILL Developer Key?**
Log in to your BILL account as an administrator at **app.bill.com**. Navigate to **Settings → Sync & Integrations → Manage Developer Keys**. Click **Generate developer key**, accept the Terms of Service, and click **Generate key**. You will also find your **Organization ID** (starts with '008') on this same page. Copy both values and paste them into the configuration below.

**Q: Can my AI agent approve invoices and trigger payment runs?**
Yes. Your AI agent can list pending invoices, review line-item details, and update approval statuses — all through natural conversation. It follows the same approval workflow rules configured in your BILL account, so no invoice gets paid without proper authorization. Payment operations respect your existing role-based permissions.

**Q: How do I quickly check which invoices are overdue during a financial review?**
Just ask your AI agent 'Show me all overdue invoices.' It pulls your invoice list filtered by past-due status, showing vendor name, amount, due date, and days overdue — giving you actionable data in seconds without generating reports or exporting spreadsheets.

**Q: Can multiple team members use this with different permission levels?**
Yes. BILL supports up to four developer keys per account. Each key inherits the permissions of the user who generated it. Finance managers can have full read-write access while auditors operate in read-only mode — ideal for growing companies, accounting firms, and multi-entity organizations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/billcom](https://vinkius.com/mcp/billcom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bill.com** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `billcom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bill.com** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "billcom": {
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
