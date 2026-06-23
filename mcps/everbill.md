# everbill MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/everbill)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Invoice clients, track expenses, and manage your freelance finances with clean accounting tools that save tax season headaches.

## Description
Connect your **everbill** account to any AI agent and take full control of your business administration and invoicing workflows through natural conversation.

### What you can do

- **Invoicing Orchestration** — Create and manage professional invoices programmatically, including detailed line items and customer association
- **Customer CRM** — Manage your complete directory of clients and retrieve detailed profiles and history directly through your agent
- **Inventory Intelligence** — Monitor real-time stock levels and retrieve granular product metadata to maintain high-fidelity oversight of your assets
- **Document Navigation** — Access the complete history of your business documents and retrieve detailed invoice information for audit or support
- **Administrative Visibility** — Monitor your business health by listing customers and products programmatically using natural language commands

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your everbill settings (Settings > API / Interface)
3. Start managing your business accounting from Claude, Cursor, or any MCP client

No more manual deal logging or digging through fragmented tables. Your AI acts as your dedicated business and accounting coordinator.

### Who is this for?

- **Small Business Owners** — instantly check inventory levels and create quick invoices using natural language queries
- **Accountants & Admins** — monitor customer statuses and retrieve financial records without leaving your workspace
- **Operations Leads** — manage product catalogs and coordinate customer data through simple AI commands


## Available Tools (7)
- **create_customer**: Create a new customer
- **create_invoice**: Create a new invoice
- **get_customer**: Get customer details
- **get_invoice**: Get invoice details
- **list_customers**: List all customers in everbill
- **list_invoices**: List all invoices
- **list_products**: List products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **everbill** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my customers in everbill."

**🤖 AI Agent:**
> I've retrieved your customer directory. You have 15 registered clients. Notable accounts include 'Acme Corp' (ID: 101) and 'John Doe' (ID: 102). Which one would you like to view the history for?

---

**👤 You:**
> "Check the stock levels for all products."

**🤖 AI Agent:**
> Scanning inventory... I've found 25 items in your catalog. Highlights: 'Wireless Mouse' (50 units), 'Mechanical Keyboard' (12 units), and 'USB-C Cable' (150 units). Would you like to see a list of low-stock items?

---

**👤 You:**
> "Get details for invoice ID '12345'."

**🤖 AI Agent:**
> Fetching invoice 12345... This document is for 'Acme Corp' totaling €450.00. It includes 2 items and is currently marked as 'Open'. Shall I download the PDF link for you?


## ❓ FAQ

**Q: How do I find my everbill API Key?**
In your everbill account, go to **Settings (Einstellungen)** > **API / Interface (Schnittstelle)** and generate your unique key.

**Q: Can I check specific product stock levels?**
Yes! The `list_products` tool retrieves your complete inventory directory, including current stock counts and technical metadata.

**Q: How do I create a new invoice via AI?**
Use the `create_invoice` tool by providing the `customer_id` and a JSON array of items (product IDs and quantities).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/everbill](https://vinkius.com/mcp/everbill)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **everbill** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `everbill` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **everbill** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "everbill": {
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
