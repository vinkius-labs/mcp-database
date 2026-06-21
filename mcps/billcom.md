# Bill.com MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/billcom)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/billcom-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/billcom-mcp)
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


## Installation & Usage

To install and use the **Bill.com** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/billcom](https://vinkius.com/mcp/billcom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
