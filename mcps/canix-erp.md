# Canix ERP MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/canix-erp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage your cannabis operations via Canix — track inventory, plants, and sales orders directly from any AI agent.

## Description
Connect your **Canix** account to any AI agent and orchestrate your cannabis cultivation, inventory management, and sales workflows through natural conversation.

### What you can do

- **Inventory Oversight** — List and retrieve detailed metadata for all cannabis packages and individual inventory items.
- **Cultivation Tracking** — Monitor individual plants and immature plant batches across your facilities.
- **Sales Coordination** — Access and monitor sales orders, including contents and payment history directly from your workspace.
- **Non-Cannabis Management** — Track non-cannabis inventory like packaging, nutrients, and supplies.
- **Operational Reporting** — Retrieve core account and facility information straight from your workspace.
- **Data Deep Dives** — Get detailed data for specific package, plant, or order IDs using natural language.

### How it works

1. Subscribe to this server
2. Enter your Canix API Key
3. Start managing your cannabis ERP from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Cultivation Managers** — quickly check plant statuses or batch details without manual dashboard monitoring.
- **Inventory Leads** — verify package tags and weights straight from their workflow tools.
- **Sales Teams** — monitor order progress and inventory availability using natural language.


## Available Tools
- **get_account_info**: Retrieve core account information
- **get_non_cannabis_product**: Get details of a specific non-cannabis product
- **get_package_details**: Get details of a specific cannabis package
- **get_plant_details**: Get details of a specific plant
- **get_sales_order**: Get details of a specific sales order
- **list_plant_batches**: List immature plant batches
- **list_non_cannabis_inventory**: List non-cannabis inventory like packaging or nutrients
- **list_inventory_packages**: List all cannabis packages (inventory) in Canix
- **list_plants**: List individual plants in the cultivation phase
- **list_sales_orders**: List all sales orders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Canix ERP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active inventory packages in Canix."

**🤖 AI Agent:**
> I've retrieved your packages. You have several active items, including 'Blue Dream Flower' (ID: pkg_1, 5lb) and 'OG Kush Pre-rolls' (ID: pkg_2).

---

**👤 You:**
> "Show the details for sales order with ID 99283."

**🤖 AI Agent:**
> Sales order 99283 is for 'Green Relief' dispensary. It contains 10 units of 'Indica Cartridges' and is currently in 'Shipped' status.

---

**👤 You:**
> "How many plants are currently in the Flowering phase?"

**🤖 AI Agent:**
> Retrieving cultivation data... You currently have 150 plants in the 'Flowering' phase across 3 facilities.


## ❓ FAQ

**Q: Can I check the weight of a specific package using the agent?**
Yes! Use the `get_package_details` tool with the Package ID. Your agent will fetch the detailed metadata, which includes the weight and unit of measure directly from Canix.

**Q: How do I list all the plants in a specific growth phase?**
Simply ask the agent to `list_plants`. You can then filter the results by growth phase or status metadata using the agent's natural language capabilities.

**Q: Does the integration allow creating a new sales order?**
The current toolset is focused on querying and monitoring (Read-Only) for operational oversight. Creating or updating sales orders should be managed through the Canix web interface or dedicated sales terminal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/canix-erp](https://vinkius.com/mcp/canix-erp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Canix ERP** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `canix-erp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Canix ERP** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "canix-erp": {
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
