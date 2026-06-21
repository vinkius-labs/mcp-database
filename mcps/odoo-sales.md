# Odoo Sales MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/odoo-sales)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Create quotations, confirm sales orders, manage products and pricelists — Odoo Sales pipeline through natural conversation.

## Description
Connect **Odoo ERP** to any AI agent — manage your entire business without switching tabs.

### What you can do
- **CRM** — Search and create leads, track opportunities through your pipeline
- **Contacts** — Find individual contacts and companies, create new partners
- **Sales** — List and manage sales orders with full order details
- **Notes** — Add comments and notes to any record in your Odoo instance

### Who is this for?
- **Sales Teams** — CRM pipeline at your fingertips through AI
- **Account Managers** — Quick access to contact and company information
- **Operations** — Monitor sales orders without switching screens
- **Odoo Administrators** — Query any module through natural conversation


## Available Tools
- **odoo_confirm_order**: order, transitioning it from "draft"/"sent" to "sale" state. This triggers downstream operations like delivery order creation and inventory reservation. Use when the user says a quote is approved or wants to confirm an order.

Confirm a draft quotation, converting it into an active sales order ready for fulfillment
- **odoo_create_quotation**: order in "draft" state with the specified customer and order lines. The partnerId must be an existing res.partner ID. Lines must be a JSON array where each element has product_id (existing product.template ID), product_uom_qty (quantity), and price_unit (unit price). Example lines: [{"product_id": 5, "product_uom_qty": 2, "price_unit": 100.00}]

Create a new quotation for a customer with product lines, quantities, and unit prices
- **odoo_get_order_lines**: order.line records for the given order. Returns each line with product name, quantity, unit price, and subtotal. Use when the user wants to see what products are in an order, verify quantities, or check line-level pricing.

Get the individual line items (products, quantities, prices) of a specific sales order
- **odoo_get_sales_order**: order record with all key fields: customer, status, amounts, salesperson, dates. Use after finding an order via list/search to drill down into its details. The ID is the numeric Odoo database ID (not the order number like S00042).

Get the complete details of a specific sales order or quotation by its numeric ID
- **odoo_list_pricelists**: pricelist records. Pricelists define pricing rules for different customer segments, currencies, or regions. Returns pricelist name, currency, and whether it is active. Use when the user asks about available pricing tiers or currency-specific pricing.

List all configured pricelists in Odoo with their currencies and active status
- **odoo_list_quotations**: order records in "draft" or "sent" state — these are quotations pending customer acceptance. Returns quotation number, customer name, total amount, salesperson, currency, and creation date. Use when the user asks about pending quotes, proposals awaiting approval, or the current quotation pipeline.

List all draft and sent quotations in Odoo that have not yet been confirmed as sales orders
- **odoo_list_sales_orders**: order records in "sale" or "done" state — these are confirmed orders being fulfilled or already completed. Returns order number, customer, total/untaxed amounts, salesperson, currency, and order date. Use when the user asks about active orders, confirmed sales, or order fulfillment status.

List confirmed and completed sales orders in Odoo with customer, amounts, and fulfillment status
- **odoo_search_products**: template records by name. Returns product name, sale price (list_price), cost price (standard_price), product type (consu/service/product), category, available stock quantity, and internal reference (SKU/code). Use when the user needs to find a product, check prices, or verify stock before creating a quotation.

Search the Odoo product catalog by name, returning prices, cost, category, stock, and SKU


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Odoo Sales** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for leads from the website"

**🤖 AI Agent:**
> 👥 **CRM Leads — Website**
| Name | Email | Stage | Revenue |
|---|---|---|---|
| Acme Corp | info@acme.com | Qualification | $15,000 |
| Beta Inc | hello@beta.io | Proposition | $8,500 |

---

**👤 You:**
> "Show recent sales orders"

**🤖 AI Agent:**
> 📋 **Sales Orders**
| SO# | Customer | Amount | Status |
|---|---|---|---|
| S00042 | Acme Corp | $12,500 | Confirmed |
| S00041 | Beta Inc | $3,200 | Draft |


## ❓ FAQ

**Q: Which Odoo versions are supported?**
This server uses the JSON-RPC protocol, which is compatible with Odoo 14, 15, 16, 17, and 18. Both Odoo Community and Enterprise editions are supported.

**Q: Does it work with Odoo.com (SaaS)?**
Yes! Works with both Odoo.com hosted instances and self-hosted Odoo servers. Just provide your instance URL and API key.

**Q: How do I generate an API Key?**
Go to Settings → Users → select your user → API Keys tab → New API Key. Give it a descriptive name and copy the generated key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/odoo-sales](https://vinkius.com/mcp/odoo-sales)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Odoo Sales** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `odoo-sales` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Odoo Sales** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "odoo-sales": {
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
