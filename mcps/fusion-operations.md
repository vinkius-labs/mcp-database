# Fusion Operations MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fusion-operations)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Optimize factory floor operations with real-time production tracking, worker scheduling, and quality control automation.

## Description
Connect your **Autodesk Fusion Operations** (formerly Prodsmart) account to any AI agent and take full control of your manufacturing execution and shop floor workflows through natural conversation.

### What you can do

- **Production Orchestration** — List and manage all manufacturing orders and retrieve detailed status and technical metadata programmatically
- **Shop Floor Visibility** — Monitor workers, production records, and machine operations in real-time to maintain a high-fidelity oversight of your factory
- **Inventory & Logistics** — Oversight stock levels across different storage locations and warehouses to ensure precise material management
- **Product Catalog** — Access complete metadata and technical details for all items in your manufacturing database directly through your agent
- **Operational Monitoring** — Check site/company information and retrieve historical production logs for instant reporting and process analysis

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** and **Secret** from Fusion Operations (Profile > Request an API key)
3. Start managing your factory operations from Claude, Cursor, or any MCP client

No more manual status checking or digging through manufacturing tables. Your AI acts as your dedicated production and operations coordinator.

### Who is this for?

- **Production Managers** — instantly retrieve order statuses and monitor site-wide output using natural language commands
- **Operations Leads** — track real-time inventory levels and machine performance without leaving your workspace
- **Manufacturing Engineers** — automate the extraction of production records and technical specifications for analysis


## Available Tools (12)
- **get_manufacturing_site_info**: Get current site/company details
- **list_inventory_stocks**: List current inventory levels
- **list_floor_machines**: List production machines
- **list_manufacturing_operations**: List manufacturing operations
- **list_production_orders**: List all production orders
- **list_manufacturing_products**: List all products/items
- **list_production_records**: List history of production records
- **list_storage_locations**: List storage locations
- **list_floor_workers**: List shop floor workers
- **create_production_order**: Requires product and quantity.

Create a new production order
- **get_product_details**: Get details for a specific product
- **get_production_order_details**: Get details for a specific production order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fusion Operations** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active production orders in Fusion Operations."

**🤖 AI Agent:**
> I've retrieved your active production orders. You have 3 jobs in progress, including 'PO-1001' (Gear Shafts) and 'PO-1002' (Pump Units). Which one would you like to check for completion status?

---

**👤 You:**
> "What is the current stock level for 'Gasket Kit'?"

**🤖 AI Agent:**
> Checking inventory... For 'Gasket Kit' (ID: prod_789), you currently have 150 units in the 'Main Warehouse' and 50 units in the 'Assembly Area'. Total availability is 200 units.

---

**👤 You:**
> "Show me the production records from today."

**🤖 AI Agent:**
> Scanning production logs... Today, 5 records have been completed so far. Total output includes 500 Gear Shafts and 25 Pump Units. All operations are running within the scheduled timeframe.


## ❓ FAQ

**Q: How do I find my API Key and Secret?**
Log in to Fusion Operations as an Admin, click on your profile name, and select **Request an API key**. You will receive your credentials via email.

**Q: Can I check stock levels in a specific warehouse?**
Yes! Use the `list_inventory_stocks` tool. You can also use `list_storage_locations` first to identify the correct warehouse ID.

**Q: Does the integration support tracking individual floor workers?**
The `list_floor_workers` tool allows you to retrieve a directory of all registered personnel and their current status in the system.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fusion-operations](https://vinkius.com/mcp/fusion-operations)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fusion Operations** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fusion-operations` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fusion Operations** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fusion-operations": {
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
