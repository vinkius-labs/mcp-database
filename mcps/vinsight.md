# Vinsight MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vinsight)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage wine, beer, and spirits production — inventory, sales orders, batches, vessels, and lab results for your Vinsight operation through natural conversation.

## Description
Connect your **Vinsight** operation to any AI agent and manage your entire beverage production business through natural conversation.

### What you can do

- **Stock Items** — Search your product catalog: wines, beers, spirits, and raw materials with pricing and compliance codes
- **Sales Orders** — Track orders: customer, items, totals, status, and shipping across all channels
- **Production Orders** — Monitor production runs: input materials, output products, vessel assignments
- **Batches** — Track individual lots through the production lifecycle with batch codes and vintage
- **Vessels** — Monitor tanks, fermenters, barrels, and bright tanks with capacity and fill levels
- **Lab Results** — View QC analyses: pH, TA, alcohol, SO₂, dissolved oxygen, and residual sugar
- **Inventory** — Real-time stock levels across all warehouses: available, committed, and on-order
- **Contacts** — Manage customers, suppliers, and distributors
- **Purchase Orders** — Track incoming materials: grapes, bottles, corks, chemicals

### Who is this for?

- **Winemakers & Brewmasters** — Production tracking, batch management, and quality control
- **Operations Managers** — Inventory visibility, warehouse management, and supply chain tracking
- **Sales Teams** — Order status, customer insights, and available stock queries
- **Finance** — Revenue tracking, purchase costs, and margin analysis


## Available Tools
- **search_stock_items**: Returns product details including SKU, description, unit of measure, price, tax code, and current stock level. Works for wine, beer, spirits, and raw materials.

Search wine/beer/spirit products
- **list_stock_levels**: Critical for fulfillment and reorder decisions.

List current inventory
- **list_lab_results**: Sorted by date. For quality control and compliance monitoring.

List lab analysis results
- **list_warehouses**: For multi-site inventory management.

List warehouses
- **get_stock_item**: The definitive product record.

Get product details
- **list_sales_orders**: Core revenue tracking for wineries and breweries.

List sales orders
- **get_sales_order**: Get order details
- **search_contacts**: Returns contact profile, type, addresses, payment terms, and order history.

Search contacts
- **list_purchase_orders**: Supply chain tracking for production inputs.

List purchase orders
- **list_production_orders**: Tracks the winemaking or brewing process.

List production orders
- **list_batches**: Track individual lots through the production lifecycle.

List production batches
- **list_vessels**: With capacity, current contents, fill level, and location. For cellar space planning.

List tanks and barrels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vinsight** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's our current Chardonnay 2024 inventory?"

**🤖 AI Agent:**
> 🏭 **Chardonnay 2024 — Inventory Report**

📦 **Stock levels**:
- Available: **4,200 bottles** (350 cases)
- Committed (orders): 1,800 bottles
- On-hand total: 6,000 bottles

🛢️ **Bulk stock**: 2,400L in Tank S-12
📍 **Warehouse**: Main Cellar (bonded)

📊 **Sales velocity**: ~600 bottles/month
⏰ **Stock duration**: ~7 months at current rate

💡 Consider scheduling next bottling run in Q1 2026.

---

**👤 You:**
> "Create a new production order to blend 500L of 'Batch 44' into Tank 12."

**🤖 AI Agent:**
> Executing `create_production_order`...
Production Order #PO-9912 successfully registered.
Action: Transfer & Blend
Source: Batch 44 (500L)
Destination: Tank 12
Status: Pending execution by Cellar Team.

---

**👤 You:**
> "Check the latest lab results for the Pinot Noir fermentations in Tank B."

**🤖 AI Agent:**
> Fetching QC analysis ('get_lab_results')...
Tank B (Pinot Noir 2025 - Fermentation):
- pH: 3.45
- TA: 6.2 g/L
- Temp: 24°C
- Brix: 4.5° (Dropping steadily)
- Residual Sugar: Not tested yet.


## ❓ FAQ

**Q: Does Vinsight work for breweries too?**
Yes! Vinsight manages wine, beer, and spirits production. The same API covers all beverage types — wineries, breweries, and distilleries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vinsight](https://vinkius.com/mcp/vinsight)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vinsight** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `vinsight` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vinsight** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vinsight": {
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
