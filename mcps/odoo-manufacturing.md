# Odoo Manufacturing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/odoo-manufacturing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Create manufacturing orders, manage BOMs, work orders, and work centers — Odoo MRP through natural conversation.

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


## Available Tools (7)
- **odoo_create_manufacturing_order**: production record in "draft" state. Requires a product.product ID and desired quantity. Odoo will auto-select the default BOM if bomId is not specified. Once confirmed, the system will check component availability and create work orders if the BOM has routing operations. Use when the user wants to schedule new production, replenish stock via manufacturing, or create a custom production run.

Create a new manufacturing order to produce a specific product quantity, optionally with a specific Bill of Materials
- **odoo_get_bom_components**: bom.line records for the given BOM ID, showing each raw material/component needed, its required quantity, and unit of measure. Use when the user needs to know what materials are needed to manufacture a product, wants to verify component quantities, or is planning material procurement.

Get the component list (raw materials and quantities) of a specific Bill of Materials
- **odoo_get_manufacturing_order**: production record with all key fields for drill-down analysis. Use after listing MOs to inspect a specific production order — e.g., to check how much has been produced vs planned, which BOM is being used, or the planned start date.

Get the complete details of a specific manufacturing order including product, BOM, quantities, and progress
- **odoo_list_boms**: bom records — the recipes/formulas that define how products are manufactured. Returns BOM name, finished product, quantity produced per BOM, BOM type (normal manufacturing vs kit), and reference code. Use when the user asks about product recipes, manufacturing formulas, component lists, or needs to find a BOM ID for creating manufacturing orders.

List all Bills of Materials (BOMs) in Odoo showing the finished product, quantity, type, and reference code
- **odoo_list_manufacturing_orders**: production records showing all manufacturing orders across the shop floor. Returns MO reference number, product being manufactured, planned quantity, quantity already produced, production state (draft/confirmed/progress/done/cancel), linked Bill of Materials, and planned start date. Filter by state to focus on orders in progress, waiting for materials, or completed. Use when the user asks about production activity, shop floor status, manufacturing backlog, or wants to check which products are being produced.

List manufacturing orders (production orders) in Odoo with product, planned quantity, BOM, and production status
- **odoo_list_work_centers**: workcenter records — the physical or logical production resources where operations are performed. Returns work center name, code, capacity, time efficiency percentage, and active status. Use when the user asks about available production resources, machine capacity, or needs work center codes for planning.

List all work centers (machines, stations, production lines) configured in Odoo Manufacturing
- **odoo_list_work_orders**: workorder records — the individual operations within manufacturing orders. Each work order represents a step in the production routing (e.g., cutting, assembly, painting). Returns work order name, product, assigned work center, state (pending/ready/progress/done), expected duration, and linked production order. Use when the user asks about shop floor activity, operator assignments, or production bottlenecks.

List active work orders on the shop floor showing product, assigned work center, state, and estimated duration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Odoo Manufacturing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

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

1. View installation instructions and explore the server: [https://vinkius.com/mcp/odoo-manufacturing](https://vinkius.com/mcp/odoo-manufacturing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Odoo Manufacturing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `odoo-manufacturing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Odoo Manufacturing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "odoo-manufacturing": {
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
