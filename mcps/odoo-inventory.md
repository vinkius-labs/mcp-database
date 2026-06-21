# Odoo Inventory MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/odoo-inventory)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Track stock levels, manage warehouses and transfers, search lot numbers — complete Odoo Inventory control through natural conversation.

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


## Available Tools (9)
- **odoo_product_stock**: quant records for the given product ID, showing quantity and reserved quantity at each internal location. Use when the user needs to know WHERE stock is located, not just the total — e.g., "how much of Product X is in Warehouse A vs Warehouse B?"

Get detailed stock levels for a specific product broken down by warehouse location
- **odoo_get_transfer**: picking record with all fields including move line IDs. Use after listing transfers to drill into a specific receipt, delivery, or internal transfer for full details.

Get complete details of a specific stock transfer including its individual stock move lines
- **odoo_list_adjustments**: quant records where inventory_quantity_set is true — these are quants with a proposed adjustment that has not yet been applied. Use when the user asks about pending stock corrections, cycle count discrepancies, or inventory adjustments awaiting approval.

List pending inventory adjustments that need to be validated or reviewed by a warehouse manager
- **odoo_list_locations**: location records with usage="internal" — the physical locations where stock is stored. Returns location name, full hierarchical path (e.g., WH/Stock/Zone A), and parent warehouse. Use when the user needs to find specific storage locations, plan inventory placement, or understand the warehouse structure.

List internal stock locations (bins, zones, shelves) within Odoo warehouses
- **odoo_list_stock_moves**: move records ordered by date descending. Each move represents a single product movement from one location to another. Returns product name, quantity, state, origin/destination locations, and source document. Use when the user needs a granular audit trail of what moved where and when.

List recent individual stock movements showing product, quantity, source, destination, and processing state
- **odoo_list_transfers**: picking records — each represents a batch of stock moves like incoming shipments, outgoing deliveries, or internal transfers. Returns transfer reference, partner, operation type, state (draft/waiting/confirmed/assigned/done), source document (e.g., SO or PO number), scheduled date, and source/destination locations. Filter by state to see only pending, ready, or completed transfers.

List stock transfers (receipts, deliveries, internal moves) in Odoo with their current processing status
- **odoo_list_warehouses**: warehouse records. Each warehouse has a name, short code (e.g., WH, WH2), and linked partner/address. Warehouses are the top-level organizational unit in Odoo Inventory. Use when the user asks about warehouse locations, needs warehouse codes for transfers, or wants an overview of the logistics network.

List all configured warehouses in Odoo with their short codes and addresses
- **odoo_search_lots**: lot records by name/number. Returns lot name, associated product, and total quantity in that lot. Use for traceability — when the user needs to find which products belong to a specific batch, or trace a serial number back to its origin.

Search for lot numbers or serial numbers in Odoo to trace product batches
- **odoo_search_inventory_products**: product records (variants) by name. Returns product name, internal reference (SKU), quantity on hand (qty_available), forecasted quantity (virtual_available), incoming qty, outgoing qty, category, and product type. Use when the user wants to check stock levels, find products with low inventory, or verify availability before fulfillment.

Search products in Odoo Inventory with real-time stock quantities, including available, incoming, and outgoing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Odoo Inventory** MCP server using an AI Agent (Claude, ChatGPT, etc.).

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

1. View installation instructions and explore the server: [https://vinkius.com/mcp/odoo-inventory](https://vinkius.com/mcp/odoo-inventory)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Odoo Inventory** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `odoo-inventory` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Odoo Inventory** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "odoo-inventory": {
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
