# Altoviz MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/altoviz)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Business management and invoicing — manage customers, invoices, and expenses via AI.

## Description
Connect your **Altoviz** account to your AI agent to unlock professional business management and automated invoicing. From creating and auditing sale invoices to monitoring real-time expenses and managing customer profiles, your agent handles your back-office operations through natural conversation.

### What you can do

- **Invoicing Orchestration** — List, retrieve, and create professional sale invoices and quotes (devis)
- **Accounting Management** — Monitor business receipts (dépenses) and retrieve supplier details
- **Customer Oversight** — List and manage customer profiles, ensuring your business network is always updated
- **Product Management** — List products and retrieve inventory details to manage your catalog
- **Financial Insights** — Quickly identify overdue invoices or retrieve specific transaction details directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Altoviz API Key
3. Start managing your business operations and monitoring performance through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Small Business Owners** — automate invoicing and monitor overall business health effortlessly
- **Finance & Accounting Leads** — audit sales records and manage expenses via simple commands
- **Operations Managers** — check real-time product catalogs and manage customer contacts on the fly
- **Sales Teams** — research customer history and create new quotes without leaving the chat


## Available Tools (10)
- **list_receipts**: List business receipts/expenses
- **list_suppliers**: List suppliers
- **list_products**: List catalog products
- **get_product_details**: Get product metadata
- **list_customers**: List customers
- **get_customer_details**: Get customer metadata
- **list_sale_invoices**: List sale invoices
- **get_sale_invoice_details**: Get invoice metadata
- **list_sale_quotes**: List sale quotes
- **get_sale_quote_details**: Get quote metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Altoviz** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 sale invoices in Altoviz."

**🤖 AI Agent:**
> I've retrieved the latest 5 sale invoices. They total €1,200. Would you like to check the details of a specific invoice?

---

**👤 You:**
> "Show me details for customer 'John Doe'."

**🤖 AI Agent:**
> I've found customer John Doe (ID: 123). His contact email is john@example.com. Would you like to see his latest invoices?

---

**👤 You:**
> "List the products in my catalog."

**🤖 AI Agent:**
> You have 15 products in your catalog. Top items include 'Consulting Service' and 'Software License'. Let me know if you need specific pricing details.


## ❓ FAQ

**Q: How do I find my Altoviz API Key?**
Log in to your Altoviz account, navigate to your account settings or developer section, and generate a new API key. This key will be used as the `X-API-KEY` header.

**Q: Can I retrieve supplier invoices (receipts)?**
Yes! Use the `list_receipts` tool to get a list of expenses/receipts recorded in Altoviz.

**Q: Are sale quotes supported?**
Yes, you can use the `list_sale_quotes` tool to see existing quotes, and `get_sale_quote_details` for specific information.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/altoviz](https://vinkius.com/mcp/altoviz)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Altoviz** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `altoviz` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Altoviz** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "altoviz": {
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
