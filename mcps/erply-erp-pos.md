# Erply ERP & POS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/erply-erp-pos)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to manage retail products, track sales invoices, and monitor inventory via the Erply API.

## Description
Integrate **Erply**, the powerful enterprise resource planning (ERP) and point-of-sale (POS) platform, directly into your AI workflow. Manage your retail product catalog and pricing, track sales documents and invoices, monitor real-time inventory levels across locations, and oversee your customer database using natural language.

### What you can do

- **Product Oversight** — List and retrieve detailed information, SKUs, and pricing for all your retail products.
- **Sales Intelligence** — Monitor sales documents and invoices, resolving document numbers, total amounts, and payment statuses.
- **Inventory Management** — Access and monitor real-time stock levels, tracking available quantities and reserved counts across your ERP.
- **Retail Auditing** — Retrieve high-level summaries of product volume, sales performance, and organizational inventory health instantly.

### How it works

1. Connect the Erply integration to your AI assistant.
2. Authorize using your Erply Client Code and Session Token (generated via API or dashboard).
3. Orchestrate your retail operations and inventory management through intuitive conversation.

### Who is this for?

- **Retail Managers** — Quickly check stock levels and sales performance on the go.
- **Inventory Specialists** — Research product details and stock availability via chat.
- **Operations Teams** — Monitor invoice statuses and organizational ERP metadata instantly.


## Available Tools
- **get_erply_user_metadata**: Retrieve metadata and settings for the current Erply user
- **list_inventory_stock_levels**: List real-time inventory levels across all products
- **get_product_detailed_data**: Get detailed settings and information for a specific product
- **quick_retail_performance_audit**: Retrieve a high-level summary of products, sales, and stock
- **list_crm_customers**: List all customers registered in your ERP
- **list_sales_documents**: List all sales invoices and documents
- **list_retail_price_lists**: List all active price lists and promotion schemes
- **list_retail_products**: List all products in your Erply retail account
- **list_latest_sales_transactions**: Identify the most recently recorded sales documents
- **search_products_by_name**: Search for products using a name keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Erply ERP & POS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products with zero stock."

**🤖 AI Agent:**
> I've identified several products with zero stock, including 'Vintage Denim Jacket' and 'Leather Belt (Black)'. Would you like to see the last supplier order for these items?

---

**👤 You:**
> "Show me the last 5 sales invoices."

**🤖 AI Agent:**
> I've retrieved the 5 most recent sales invoices, including '#INV-9988' ($150, Paid) and '#INV-9977' ($240, Pending). Should I pull the line items for the most recent invoice?

---

**👤 You:**
> "Search for product 'Wireless Mouse'."

**🤖 AI Agent:**
> I've found 3 products matching 'Wireless Mouse': 'Basic Wireless Mouse' ($25), 'Pro Gaming Mouse' ($85), and 'Ergo Mouse' ($45). All are currently in stock. Would you like the detailed data for the Pro Gaming Mouse?


## ❓ FAQ

**Q: How do I get Erply API credentials?**
You need your **Client Code** (found in your Erply account URL) and a **Session Token**. You can generate a Session Token by making a login request to the Erply API using your credentials. Please refer to the Erply API documentation for details on generating long-lived tokens.

**Q: Is the inventory data real-time?**
Yes, you can use the list_inventory_stock_levels tool to retrieve current available and reserved counts directly from the Erply database.

**Q: Can the agent process new sales in the POS?**
This integration currently focuses on listing and auditing products, sales documents, and inventory. Processing live transactions should be performed via the Erply POS interface or dedicated hardware.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/erply-erp-pos](https://vinkius.com/mcp/erply-erp-pos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Erply ERP & POS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `erply-erp-pos` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Erply ERP & POS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "erply-erp-pos": {
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
