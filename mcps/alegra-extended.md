# Alegra MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/alegra-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Handle your Latin American business accounting with electronic invoicing, expense tracking, and tax-ready financial reports.

## Description
Connect your **Alegra** account to any AI agent and simplify how you manage your professional billing, customer directory, and inventory through natural conversation.

### What you can do

- **Billing Management** — Create, list, and inspect sales invoices with detailed status tracking (open, paid, overdue).
- **Customer & Supplier CRM** — Manage your contacts, update profile data, and check individual transaction histories.
- **Inventory Control** — Query your product and service catalog to monitor stock levels and pricing metadata.
- **Financial Oversight** — Monitor received payments and track sales estimates/quotes sent to potential clients.
- **Organization Insights** — Retrieve company metadata and verify account configurations directly from the agent.
- **Operational Monitoring** — Check connectivity and manage your commercial ecosystem without leaving your workspace.

### How it works

1. Subscribe to this server
2. Enter your Alegra Email and API Token (found in your account settings)
3. Start managing your business finances from Claude, Cursor, or any MCP client

### Who is this for?

- **Small Business Owners** — quickly create invoices and check client balances via simple AI commands.
- **Finance & Admin Teams** — monitor payments and manage the contact directory directly from the workspace.
- **Operations Managers** — track inventory levels and verify service availability via the AI assistant.


## Available Tools
- **create_contact**: Create a new contact in Alegra
- **create_invoice**: Create a new sales invoice
- **get_contact_details**: Get details of a specific contact
- **get_invoice_details**: Get details of a specific invoice
- **get_item_details**: Get details of an inventory item
- **get_company_info**: Get Alegra company information
- **list_contacts**: List Alegra contacts (clients and suppliers)
- **list_estimates**: List estimates/quotes
- **list_invoices**: List sales invoices in Alegra
- **list_inventory_items**: List products and services
- **list_payments**: List recorded payments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Alegra** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active invoices in my Alegra account."

**🤖 AI Agent:**
> I've retrieved your invoices. You have 3 active sales documents: #INV-001 ($150.00, Paid), #INV-002 ($450.00, Open), and #INV-003 ($1,200.00, Overdue). Which one would you like more details on?

---

**👤 You:**
> "Show me the details for contact 'John Doe' (ID: 10293)."

**🤖 AI Agent:**
> I've fetched John Doe's profile. He is a 'Client' and has an outstanding balance of $450.00 from invoice #INV-002. Shall I retrieve his full contact history?

---

**👤 You:**
> "What is the stock level for 'Professional Desk'?"

**🤖 AI Agent:**
> Checking inventory... The 'Professional Desk' (ID: item_8823) currently has 15 units in stock. The unit price is $250.00. Would you like to create an invoice for this item?


## ❓ FAQ

**Q: Can I check the stock level of an item via AI?**
Yes! Use the `get_item_details` tool and provide the Item ID. Your agent will retrieve the complete metadata, including current stock levels for that product.

**Q: How do I create a new invoice for a client?**
Use the `create_invoice` action. You'll need to provide the Contact ID, date, due date, and a JSON string of items to register the new sale in Alegra.

**Q: Is it possible to list all my recent payments?**
Absolutely. Use the `list_payments` query. The agent will retrieve a list of all recorded income payments received in your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alegra-extended](https://vinkius.com/mcp/alegra-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Alegra** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `alegra-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Alegra** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "alegra-extended": {
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
