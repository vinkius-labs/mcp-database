# MaintainX MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/maintainx)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [operations-management](../categories/operations-management.md)

Manage work orders, assets, and facility locations via the MaintainX REST API.

## Description
Connect your **MaintainX** workspace to any AI agent to automate your maintenance operations and asset management. This MCP server enables your agent to list work orders, retrieve detailed asset metadata, update task statuses, and monitor facility locations directly from natural language interfaces.

### What you can do

- **Work Order Oversight** — List all maintenance tasks and retrieve detailed statuses, priorities, and descriptions
- **Asset Management** — Monitor equipment and machinery health by retrieving complete metadata and associated work orders
- **Status Automation** — Update the progress of tasks (e.g., to 'Done' or 'In Progress') programmatically from your conversation
- **Facility Tracking** — List and inspect physical sites and areas where your assets and team members reside
- **User Coordination** — List team members and manage assignees for specific maintenance tasks effortlessly

### How it works

1. Subscribe to this server
2. Enter your MaintainX API Key (Bearer Token)
3. Start managing your operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Maintenance Managers** — Monitor operational performance and update task statuses via simple natural language commands
- **Facility Coordinators** — Quickly audit asset locations and team assignments without opening the portal
- **Operations Developers** — Integrate maintenance data and task automation directly into your custom internal tools


## Available Tools
- **list_maintenance_assets**: List all physical assets and equipment
- **create_new_work_order**: Requires title.

Create a new maintenance work order
- **get_asset_details**: Get metadata for a specific asset
- **get_work_order_details**: Get details for a specific work order
- **list_facility_locations**: List facility locations
- **update_work_order_status**: g., "DONE", "IN_PROGRESS").

Change the status of a work order
- **list_team_members**: List all users in the MaintainX account
- **list_maintenance_orders**: Use optional params for filtering.

List all work orders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MaintainX** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all open work orders in MaintainX."

**🤖 AI Agent:**
> I've retrieved your open work orders. You have 5 tasks pending, including 'HVAC Repair (ID: 123)', 'Monthly Safety Check', and 'Generator Maintenance'.

---

**👤 You:**
> "Update the status of work order ID '123' to 'DONE'."

**🤖 AI Agent:**
> Successfully updated work order 123. The status has been set to 'DONE' in your MaintainX workspace.

---

**👤 You:**
> "Show details for the asset with ID 'asset-abc'."

**🤖 AI Agent:**
> I've fetched the details for asset-abc. It is a 'Main Boiler' located in 'Section A'. Current status is 'Active' and it has 2 associated open work orders.


## ❓ FAQ

**Q: How do I find my MaintainX API Key?**
Log in to your MaintainX account as an admin, navigate to Settings > Integrations, and click 'New Key' to generate your token. Your token is encrypted at rest and injected securely at runtime.

**Q: What status codes should I use for work orders?**
Common status codes include 'OPEN', 'IN_PROGRESS', 'DONE', and 'ON_HOLD'. Use the `update_work_order_status` tool with these values.

**Q: Can I see which asset is linked to a work order?**
Yes, when using `list_maintenance_orders`, you can provide `params` with `include=assets` to see linked equipment names in the results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/maintainx](https://vinkius.com/mcp/maintainx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MaintainX** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `maintainx` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MaintainX** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "maintainx": {
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
