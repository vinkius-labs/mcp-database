# Zoho Invoice MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-invoice-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage customers, create invoices, and automate billing on Zoho Invoice — the clean and simple invoicing software for small business.

## Description
Connect your **Zoho Invoice** account to any AI agent and manage your business billing infrastructure through natural conversation.

### What you can do

- **Invoicing Lifecycle** — Create new draft invoices with line items, retrieve full details for specific IDs, and monitor payment statuses
- **Customer Management** — Browse your entire database of contacts, create new customer profiles, and update contact details directly from your agent
- **Deep Invoicing Audit** — Retrieve comprehensive metadata for any invoice, including detailed line items, taxes, and applied totals
- **Contact Discovery** — List and browse all registered business contacts to find unique IDs required for accurate billing
- **Data Governance** — Safely update invoice line items or permanently delete obsolete customer records and draft invoices through simple commands
- **Tenant Insights** — Quickly find your Organization ID and associated account properties required for automated financial workflows
- **Scalable Billing** — Automate the creation of customer records and draft billing documents through programmatic chat commands

### How it works

1. Subscribe to this server
2. Enter your Zoho API URL, Organization ID, and OAuth Token
3. Start managing your customers and invoices through Claude, Cursor, or any MCP-compatible client

No more manual data entry into complex billing dashboards to create a simple invoice. Your AI agent becomes your invoicing assistant.

### Who is this for?

- **Small Business Owners** — automate invoice drafting and manage customer lists without manual navigation
- **Freelancers & Solo-preneurs** — quickly draft new billing documents and lookup customer IDs through chat
- **Operations Managers** — audit customer records and monitor invoice statuses across the entire organization
- **Finance Teams** — verify billing details and update customer contact information through conversation


## Available Tools (10)
- **create_contact**: Create a new contact
- **create_invoice**: Create a new invoice
- **delete_contact**: Delete a contact
- **delete_invoice**: Delete an invoice
- **get_contact**: Get specific contact details
- **get_invoice**: Get specific invoice details
- **list_contacts**: List Zoho Invoice contacts
- **list_invoices**: List Zoho Invoices
- **update_contact**: Update a contact name
- **update_invoice_items**: Update invoice items


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho Invoice** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 invoices in Zoho Invoice."

**🤖 AI Agent:**
> I found your 5 most recent invoices: 1. #INV-0001 ($450.00, Status: Draft), 2. #INV-0002 ($1,200.00, Status: Paid), 3. #INV-0003 ($890.00, Status: Sent), and 2 others. Which one would you like to see the breakdown for?

---

**👤 You:**
> "Create a new contact named 'Acme Solutions'."

**🤖 AI Agent:**
> Success! I've created a new contact for 'Acme Solutions' (ID: 550e8400-e29b...). You can now generate invoices for this customer. Would you like to create a draft invoice for them now?

---

**👤 You:**
> "Find the details for invoice ID 'INV-0003'."

**🤖 AI Agent:**
> Invoice #INV-0003 Details: Customer: Global Tech, Total: $890.00, Status: Sent. Line items: 1. 'Cloud Hosting' ($700.00), 2. 'Domain Renewal' ($190.00). Would you like to see the public link for this invoice?


## ❓ FAQ

**Q: Can I draft a new invoice by providing a JSON list of items?**
Yes. The `create_invoice` tool allows you to generate a draft invoice for a specific customer. You simply provide the contact ID and a JSON array of line items including names and prices, and the draft will be created in your Zoho account.

**Q: How do I find out the total amount due for a specific customer?**
You can use the `get_invoice_details` tool for each of the customer's invoices. Your AI agent can help you list all invoices for a contact ID and then retrieve the detailed balance due for each one to give you a summary.

**Q: Is it possible to update a customer's company name via chat?**
Absolutely. Using the `update_contact` tool, you can instruct your agent to change the contact name or company name associated with a specific ID, ensuring your CRM data is always accurate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-invoice-1](https://vinkius.com/mcp/zoho-invoice-1)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `zoho-invoice-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zoho Invoice** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zoho-invoice-1": {
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
