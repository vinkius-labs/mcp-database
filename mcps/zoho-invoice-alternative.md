# Zoho Invoice MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-invoice-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Create and send professional invoices, track payments, and manage expenses with free invoicing software that scales with your business.

## Description
Connect your **Zoho Invoice** account to any AI agent and simplify how you manage your professional billing, customer directory, and payment tracking through natural conversation.

### What you can do

- **Invoice Management** — Create, list, and send professional invoices, and retrieve detailed status (DRAFT, SENT, PAID).
- **Customer Directory** — Manage your client base, update contact details, and check outstanding balances or credit limits.
- **Payment Tracking** — Monitor received payments and track overdue invoices in real-time to keep your cash flow healthy.
- **Estimate Control** — Query and manage price estimates sent to clients before they become invoices.
- **Expense Monitoring** — List and track business expenses associated with specific projects or customers.
- **Operational Insight** — Retrieve high-level summaries of your billing activity directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Zoho Invoice Authtoken or OAuth credentials
3. Start invoicing directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Freelancers & Small Business Owners** — quickly create invoices and check client balances via simple AI commands.
- **Finance Teams** — monitor overdue payments and track expense records directly from the workspace.
- **Accountants** — retrieve transaction histories and verify customer metadata via the AI assistant.


## Available Tools (12)
- **check_zoho_invoice_status**: Returns a status indicator and organization metadata to confirm valid credentials.

Verify Zoho Invoice API connectivity
- **create_contact**: The contact name is required. Optionally provide company name, email, and phone.

Create a new contact (customer) in Zoho Invoice
- **create_invoice**: Requires the customer_id and at least one line_item with name and rate. The invoice is created in DRAFT status by default.

Create a new invoice in Zoho Invoice
- **get_contact**: Get full details of a specific contact
- **get_invoice**: Get full details of a specific invoice
- **get_item**: Get full details of a specific item
- **list_contacts**: Optionally search by name. Returns contact names, IDs, emails, outstanding balances, and unused credits.

List all contacts (customers) in Zoho Invoice
- **list_estimates**: Optionally filter by status such as "draft", "sent", "invoiced", "accepted", or "declined".

List all estimates (quotes) in Zoho Invoice
- **list_expenses**: Returns expense dates, categories, amounts, vendors, and associated projects or customers.

List all tracked expenses
- **list_invoices**: Optionally filter by status such as "sent", "draft", "overdue", "paid", or "void". Returns invoice numbers, amounts, dates, and customer information.

List all invoices in Zoho Invoice
- **list_items**: List all items (products/services) in Zoho Invoice
- **list_payments**: Useful for tracking cash flow and reconciliation.

List all customer payments received


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho Invoice** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my unpaid invoices and verify the contact details for 'Acme Corp'."

**🤖 AI Agent:**
> I found 3 unpaid invoices, totaling $4,500. For 'Acme Corp', the contact ID is 84029. Their primary email is 'billing@acme.com' and they currently have an outstanding balance of $1,200. Would you like me to send them a payment reminder?

---

**👤 You:**
> "Create a new invoice for client 'cust_8823' for 'Consulting Services' at $150.00, and include a note thanking them for their business."

**🤖 AI Agent:**
> Success! Invoice #INV-99023 has been created for $150.00 and assigned to client cust_8823. The note 'Thank you for your business' was added. It is currently in 'DRAFT' status. Shall I send it now?

---

**👤 You:**
> "List all business expenses recorded this month and fetch the full details for the highest one."

**🤖 AI Agent:**
> I retrieved 12 business expenses for this month. The highest expense is $850.00 for 'Software Subscriptions' (Expense ID: 40392). It was billed by 'TechCloud' and is assigned to the 'Internal IT' project.


## ❓ FAQ

**Q: Can I check the status of a specific invoice via AI?**
Yes! Use the `get_invoice` tool and provide the Invoice ID. Your agent will retrieve the real-time status to see if it has been viewed, paid, or is overdue.

**Q: How do I add a new customer to my Zoho Invoice directory?**
Use the `create_customer` action. Provide the company name and contact details. The agent will instantly register the new profile in your account.

**Q: Is it possible to list all unpaid invoices via AI?**
Absolutely. Use the `list_invoices` query. The agent will retrieve all your billing documents, and you can then ask the AI to identify or filter those with an unpaid or overdue status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-invoice-alternative](https://vinkius.com/mcp/zoho-invoice-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zoho Invoice** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zoho-invoice-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zoho Invoice** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zoho-invoice-alternative": {
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
