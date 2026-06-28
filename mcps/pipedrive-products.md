# Pipedrive Products MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pipedrive-products)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your product catalog and attach products to deals in Pipedrive.

## Description
Connect **Pipedrive CRM** to any AI agent — manage your entire sales pipeline without switching tabs.

### What you can do
- **Deals** — Search, create, and update deals with pipeline tracking
- **Contacts** — Find and create persons with email, phone, and organization
- **Organizations** — Search companies linked to deals and contacts
- **Activities** — Create calls, meetings, tasks, and emails
- **Notes** — Attach notes to deals, persons, or organizations
- **Pipelines** — View all pipeline stages and deal flow

### Who is this for?
- **Sales Reps** — Manage your pipeline without leaving your AI assistant
- **SDRs** — Quickly create leads, contacts, and activities
- **Sales Managers** — Pipeline overview and deal insights through conversation
- **RevOps** — Full CRM visibility and reporting


## Available Tools (7)
- **pd_create_product**: Name is required. Code serves as the internal SKU/reference. Unit defines how the product is measured (piece, hour, kg, etc.). Tax is the default tax percentage. Products in the catalog can be attached to deals using pd_add_product_to_deal.

Create a new product in the Pipedrive catalog with name, code (SKU), unit type, and tax rate
- **pd_list_products**: Returns product name, unit price, code (SKU), unit type, and whether it is active. Use for product catalog browsing, inventory auditing, or when the user wants to see all available products.

List all products in the Pipedrive product catalog with names, prices, codes, and unit information
- **pd_add_product_to_deal**: Requires the deal ID, product ID (use pd_search_products or pd_list_products to find), unit price, and quantity. The line-item total is calculated automatically. Use when the user wants to add a product to a deal, build a quote, or track what is being sold.

Attach a product from the catalog to a deal with a specific quantity and unit price for line-item tracking
- **pd_search_products**: Returns product name, unit price, product code (SKU), unit type, and tax percentage. Use when the user wants to find a product, check pricing, or needs a product ID before attaching it to a deal.

Search Pipedrive products by name to find items in the product catalog with prices, codes, and unit types
- **pd_deal_products**: Returns product name, quantity, item price, discount percentage, and total value per line. Use when the user asks "what products are on this deal?", needs to check line-item pricing, or wants to review the deal composition before closing.

Get all products attached to a specific deal with quantities, prices, and line-item totals
- **pd_get_product**: Returns full product data including name, prices per currency, code, unit, tax, and custom fields. Use after searching to drill into a specific product for complete details.

Get complete details of a specific Pipedrive product by ID including all pricing, tax, and custom fields
- **pd_update_product**: Only specified fields change. Use when the user wants to rename a product, update its SKU code, or change pricing information.

Update an existing Pipedrive product — change name, code, pricing, or other catalog properties


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pipedrive Products** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for deals with Acme Corp"

**🤖 AI Agent:**
> 📊 **Deals with Acme Corp**
| Title | Value | Stage | Pipeline |
|---|---|---|---|
| Acme Enterprise License | $45,000 | Proposal Made | Sales Pipeline |
| Acme Support Plan | $12,000 | Won | Renewals |

---

**👤 You:**
> "Create a call activity for tomorrow at 2pm"

**🤖 AI Agent:**
> ✅ **Activity Created!**
- Type: Call
- Subject: Follow-up call
- Due: Tomorrow at 2:00 PM
- Status: Pending

---

**👤 You:**
> "Show me the pipeline stages"

**🤖 AI Agent:**
> 📦 **Sales Pipeline**
1. Lead In
2. Contact Made
3. Prospect Qualified
4. Proposal Made
5. Negotiations Started
6. Won ✅
7. Lost ❌


## ❓ FAQ

**Q: What Pipedrive data can I access?**
Deals, Persons, Organizations, Activities, Notes, and Pipelines. All data respects your Pipedrive permissions.

**Q: Can I create and update records?**
Yes! Create and update deals, contacts, activities, and notes — all through natural conversation.

**Q: How does authentication work?**
Uses your personal Pipedrive API token. Find it in Settings > Personal preferences > API. No OAuth flow needed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pipedrive-products](https://vinkius.com/mcp/pipedrive-products)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pipedrive Products** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pipedrive-products` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pipedrive Products** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pipedrive-products": {
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
