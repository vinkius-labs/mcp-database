# Katana MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/katana)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Automate manufacturing ERP workflows, sales orders, and inventory via Katana Cloud Manufacturing.

## Description
Connect your **Katana Cloud Manufacturing** account to any AI agent to streamline your production and shop floor operations. This MCP server enables your agent to interact with products, materials, and complex manufacturing workflows directly from natural language interfaces.

### What you can do

- **Production Visibility** — List and inspect manufacturing orders (MOs) and production tasks
- **Order Management** — List, retrieve, and create sales orders (SOs) and purchase orders (POs)
- **Inventory Control** — Get real-time stock levels for products and material variants to prevent stockouts
- **Catalog Exploration** — Query your full product and material database, including metadata and internal IDs
- **Supply Chain Management** — Access lists of suppliers and customers to maintain clear partner visibility

### How it works

1. Subscribe to this server
2. Enter your Katana API Key
3. Start managing your manufacturing business from Claude, Cursor, or any MCP client

### Who is this for?

- **Production Managers** — Monitor live manufacturing orders and task progress without opening the Katana dashboard
- **Inventory Specialists** — Quickly check availability of specific material variants during planning
- **Sales Teams** — Retrieve order statuses and customer details instantly during client calls


## Available Tools
- **create_sales_order**: Requires a customer ID.

Create a new sales order
- **list_customers**: List all customers
- **get_sales_order**: Get details for a specific sales order
- **list_inventory**: List overall inventory status
- **get_inventory_by_variant**: Get inventory levels for a specific variant
- **list_manufacturing_orders**: List all manufacturing orders
- **list_materials**: List all materials in Katana
- **list_products**: List all products in Katana
- **list_purchase_orders**: List all purchase orders
- **list_sales_orders**: List all sales orders
- **list_suppliers**: List all suppliers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Katana** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all active sales orders in Katana."

**🤖 AI Agent:**
> I've retrieved your sales orders. You have 15 active orders, including SO-101 for 'Acme Corp' and SO-102 for 'Tech Solutions'.

---

**👤 You:**
> "Check the inventory level for variant ID 'VAR_987'."

**🤖 AI Agent:**
> For variant 'VAR_987', there are currently 45 units in stock, with 10 units committed to existing sales orders.

---

**👤 You:**
> "List all my manufacturing orders."

**🤖 AI Agent:**
> I've fetched 8 manufacturing orders. Current jobs include production of 'Wooden Table' and 'Office Chair'.


## ❓ FAQ

**Q: Can I check the inventory of a specific material variant?**
Yes, use the `get_inventory_by_variant` tool with the unique variant ID to see current stock levels and availability in real-time.

**Q: Is it possible to list all current manufacturing orders?**
Absolutely. The `list_manufacturing_orders` tool retrieves a list of all production jobs, helping you track shop floor activities.

**Q: Can I see my customer list via the agent?**
Yes, the `list_customers` tool provides access to your customer database, making it easy to reference customer IDs for new sales orders.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/katana](https://vinkius.com/mcp/katana)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Katana** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `katana` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Katana** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "katana": {
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
