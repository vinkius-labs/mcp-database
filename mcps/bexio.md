# Bexio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bexio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage your business via Bexio — list contacts, invoices, and projects directly from any AI agent.

## Description
Connect your **Bexio** account to any AI agent and orchestrate your business workflows, including CRM, accounting, and project management, through natural conversation.

### What you can do

- **Contact Management** — List, create, and retrieve detailed information for customers, suppliers, and partners.
- **Invoicing & Sales** — Query invoices, offers, and orders to stay on top of your sales pipeline and receivables.
- **Project Oversight** — List all business projects and monitor their status and progress.
- **Inventory & Items** — Access your product catalog and list items with pricing and stock metadata.
- **Team Collaboration** — Retrieve lists of users within your Bexio organization for better task coordination.

### How it works

1. Subscribe to this server
2. Enter your Bexio Personal Access Token
3. Start managing your business from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Small Business Owners** — quickly check invoice statuses and client details without manual dashboard navigation.
- **Accountants & Bookkeepers** — retrieve financial documents and contact data straight from their workflow.
- **Sales Reps** — verify offer details and create new contacts using natural language.


## Available Tools
- **create_contact**: Create a new contact
- **get_contact**: Get specific contact details
- **get_invoice**: Get specific invoice details
- **list_contacts**: List all contacts
- **list_invoices**: List all invoices
- **list_items**: List all products/items
- **list_offers**: List all offers
- **list_orders**: List all orders
- **list_projects**: List all projects
- **list_users**: List all Bexio users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bexio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in Bexio."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active projects: 'Q2 Marketing' (ID: proj_1), 'Website Overhaul' (ID: proj_2), and 'Customer Feedback Survey' (ID: proj_3).

---

**👤 You:**
> "Find the contact details for 'Acme Corp'."

**🤖 AI Agent:**
> I found one matching company: 'Acme Corporation' (ID: con_992). Their primary contact is John Smith, and their email is info@acme.com.

---

**👤 You:**
> "Show my last 5 invoices."

**🤖 AI Agent:**
> Retrieving invoices... Your 5 most recent invoices include 'INV-2024-001' (Status: Paid) and 'INV-2024-005' (Status: Draft). Would you like the details for any of these?


## ❓ FAQ

**Q: Can I check the payment status of an invoice using the agent?**
Yes! Use the `get_invoice` tool with the Invoice ID. Your agent will fetch the latest status, showing if it is draft, issued, or paid.

**Q: How do I list all my customers in Bexio?**
Simply ask the agent to `list_contacts`. It will retrieve the directory of all companies and persons registered in your Bexio account.

**Q: Does the integration allow me to create a new invoice?**
Currently, the toolset is focused on querying and management (listing contacts, checking projects, auditing invoices). For creating complex financial documents like invoices with multiple line items, we recommend using the Bexio platform directly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bexio](https://vinkius.com/mcp/bexio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bexio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bexio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bexio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bexio": {
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
