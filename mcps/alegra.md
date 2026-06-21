# Alegra MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/alegra)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Business management and e-invoicing — manage invoices, inventory, and contacts via AI.

## Description
Connect your **Alegra** account to your AI agent to unlock professional business management and automated invoicing. From creating and auditing sales invoices to monitoring real-time inventory levels and managing client/provider contact profiles, your agent handles your back-office operations through natural conversation.

### What you can do

- **Invoicing Orchestration** — List, retrieve, and create professional sales invoices with tax compliance
- **Inventory Management** — Monitor stock levels for products and services and retrieve technical metadata for items
- **Contact Oversight** — List and manage client and provider profiles, ensuring your business network is always updated
- **Payment & Estimates** — List payments and retrieve business estimates (cotizaciones) to track your revenue pipeline
- **Financial Insights** — Quickly identify overdue invoices or low-stock items directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Alegra Email and API Token
3. Start managing your business operations and monitoring performance through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Small Business Owners** — automate invoicing and monitor overall business health effortlessly
- **Finance & Accounting Leads** — audit sales records and manage provider payments via simple commands
- **Operations Managers** — check real-time inventory and manage product catalogs on the fly
- **Sales Teams** — research client history and create new contact records without leaving the chat


## Available Tools
- **list_invoices**: Supports date filtering.

List sales invoices
- **get_invoice_details**: Get invoice metadata
- **create_invoice**: Add a new sales invoice
- **list_contacts**: List client/provider profiles
- **get_contact_details**: Get contact metadata
- **create_contact**: Add a new contact
- **list_inventory_items**: Check stock levels
- **get_item_details**: Get product metadata
- **list_payments**: List business payments
- **list_estimates**: List business estimates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Alegra** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 invoices generated in Alegra."

**🤖 AI Agent:**
> I've retrieved the latest 5 invoices. They include sales to 'Client A', 'Global Tech', and 3 others, totaling $2,500. Would you like to see the payment status for any of them?

---

**👤 You:**
> "Show me the current stock for 'Office Chair v2'."

**🤖 AI Agent:**
> I've checked the inventory. You currently have 45 units of 'Office Chair v2' in stock. The unit price is $85.00. Would you like to see the inventory adjustments history for this item?

---

**👤 You:**
> "List all contacts of type 'provider'."

**🤖 AI Agent:**
> I've retrieved your providers. You have 12 registered providers, including 'Wholesale Logistics' and 'Office Supplies Co'. Would you like the contact details for any of them?


## ❓ FAQ

**Q: How do I find my Alegra API Token?**
Log in to Alegra, navigate to **Settings** > **API**, and copy your token. You will need this along with your login email for Basic Authentication.

**Q: Can I filter contacts by type?**
Yes! Use the `list_contacts` tool and specify the `type` parameter as either 'client' or 'provider' to filter your list.

**Q: Does this support checking stock levels?**
Yes, the `list_inventory_items` tool provides real-time stock quantities for all your products and services managed in Alegra.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alegra](https://vinkius.com/mcp/alegra)
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
3. Set Type to "SSE", enter `alegra` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Alegra** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "alegra": {
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
