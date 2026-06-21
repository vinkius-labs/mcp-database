# Wave Accounting MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wave-accounting)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wave-accounting-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wave-accounting-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage customers, invoices, and accounting workflows on Wave — the money management tool for small businesses.

## Description
Connect your **Wave Accounting** account to any AI agent and manage your business finances through natural conversation.

### What you can do

- **Customer Management** — List all registered customers, create new profiles, and update contact information directly from your agent
- **Invoice Lifecycle** — Create draft invoices, approve them for sending, and monitor their payment status (DRAFT, SAVED, PAID)
- **Deep Invoicing** — Retrieve full details for any invoice, including line items, taxes, totals, and public payment URLs
- **Financial Auditing** — Browse your customer base and billing activity to stay on top of your accounts receivable
- **Data Integrity** — Safely delete unfinalized draft invoices or obsolete customer records through simple chat commands
- **Business Insights** — Quickly find unique customer and invoice IDs required for complex accounting workflows

### How it works

1. Subscribe to this server
2. Enter your Wave Business ID and Access Token
3. Start managing your customers and invoices through Claude, Cursor, or any MCP-compatible client

No more manual data entry into complex accounting dashboards. Your AI agent becomes your financial assistant.

### Who is this for?

- **Small Business Owners** — automate invoice creation and manage customer lists without manual navigation
- **Freelancers & Solo-preneurs** — quickly check payment status and draft new billing documents through chat
- **Accountants & Bookkeepers** — audit customer records and monitor invoice statuses across different businesses
- **Sales Teams** — lookup customer details and verify billing information before closing deals


## Available Tools
- **approve_draft_invoice**: Finalizes a draft invoice, moving it to an unpaid/saved status
- **create_accounting_customer**: Provide name and email.

Creates a new customer record in Wave
- **create_draft_invoice**: Provide a customer ID and a JSON array of items.

Creates a new draft invoice in Wave
- **delete_accounting_customer**: This action is irreversible.

Permanently deletes a customer record
- **delete_draft_invoice**: Saved or paid invoices cannot be deleted via this endpoint.

Permanently deletes an unfinalized draft invoice
- **get_customer_details**: Retrieves details for a specific customer in Wave
- **get_invoice_details**: Retrieves full details for a specific Wave invoice
- **list_accounting_customers**: Lists customers registered in the Wave Accounting business
- **list_accounting_invoices**: ).

Lists invoices issued by the Wave business
- **update_customer_profile**: Provide the unique customer ID.

Updates the profile of an existing customer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wave Accounting** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my customers in Wave Accounting."

**🤖 AI Agent:**
> I found 5 customers: 'Acme Corp' (ID: Y3VzdC0x), 'Global Tech' (ID: Y3VzdC0y), 'Jane Smith' (ID: Y3VzdC0z), and 2 others. Which one would you like to see details for?

---

**👤 You:**
> "Create a new customer for 'John Doe' with email 'john@example.com'."

**🤖 AI Agent:**
> Success! I've created a new customer record for John Doe (ID: Y3VzdC00OTk=) in Wave. You can now issue invoices to this customer.

---

**👤 You:**
> "What is the status of my latest invoices?"

**🤖 AI Agent:**
> Here are your 3 most recent invoices: 1. Inv #101 (PAID, 500 USD), 2. Inv #102 (SAVED, 1200 USD - Overdue), and 3. Inv #103 (DRAFT, 300 USD). Would you like to see the details for the overdue invoice?


## Installation & Usage

To install and use the **Wave Accounting** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wave-accounting](https://vinkius.com/mcp/wave-accounting)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
