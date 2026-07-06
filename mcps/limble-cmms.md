# Limble CMMS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/limble-cmms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Keep your equipment running with preventive maintenance scheduling, work order management, and asset tracking for facility teams.

## Description
Connect your **Limble CMMS** account to any AI agent and manage maintenance operations through natural conversation.

### What you can do

- **Work Orders** — Create, update, and track work orders with priority and status
- **Asset Management** — Browse assets, inspect maintenance history, and track uptime
- **Preventive Maintenance** — Monitor PM schedules and upcoming tasks
- **Parts Inventory** — Track spare parts stock levels and reorder points
- **Maintenance Reports** — Access downtime, MTTR, and reliability metrics

### How it works

1. Subscribe to this server
2. Enter your Limble Client ID and Client Secret
3. Start managing maintenance from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Maintenance Teams** — manage work orders and preventive schedules
- **Facility Managers** — track asset health and downtime
- **Operations** — monitor parts inventory and maintenance costs


## Available Tools (9)
- **list_locations**: List facility locations
- **list_parts**: List inventory parts
- **list_tasks**: List work orders and PMs
- **list_vendors**: List maintenance vendors
- **update_asset_field**: g. runtime hours, temperature) for an asset.

Update a custom field for an asset
- **get_asset_details**: Get details for a specific asset
- **list_labor_entries**: List labor logs for tasks
- **list_asset_part_relations**: List parts linked to assets
- **list_assets**: List maintenance assets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Limble CMMS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show open work orders and overdue preventive maintenance."

**🤖 AI Agent:**
> Open work orders: 14. Critical: 2 (⚠️ 'HVAC Unit 3 — compressor failure', 'Conveyor Belt B — alignment'). High: 4. Normal: 8. Overdue PMs: 3. 'Generator monthly check' (5 days late). 'Fire alarm quarterly test' (2 days). 'Elevator inspection' (1 day). PM compliance: 91%.

---

**👤 You:**
> "Show asset health for HVAC systems and parts inventory."

**🤖 AI Agent:**
> HVAC assets: 6. Healthy: 4 (✅). At risk: 1 (⚠️ Unit 3, 3 WOs this month). Down: 1 (❌ Unit 5, compressor failure). MTTR avg: 4.2 hours. Uptime: 94%. Parts inventory: Compressor filters (8 in stock, reorder at 5). Belts (3, ⚠️ at reorder point). Refrigerant (12 cans). Bearings (6).

---

**👤 You:**
> "Create a work order for Conveyor Belt B and show maintenance costs this quarter."

**🤖 AI Agent:**
> Work order created! 'Conveyor Belt B — Alignment & Tension Adjustment'. Priority: High. Assigned: Mike Torres. ETA: 2 hours. Parts: 1 belt ($45), alignment tools (in stock). Q2 costs: $18,400 total. Labor: $12,200 (66%). Parts: $4,800 (26%). External: $1,400 (8%). vs Q1: +5% ($17,500). Top cost asset: HVAC Unit 3 ($3,200).


## ❓ FAQ

**Q: Can I create and track work orders?**
Yes. Create work orders with priority, assign technicians, and track status through completion. Access full maintenance history per asset.

**Q: Does Limble CMMS use Basic Auth?**
Yes. Limble uses **HTTP Basic Auth** with Client ID and Client Secret against `api.limblecmms.com/v2`.

**Q: Can I monitor preventive maintenance schedules?**
Yes. Track PM schedules with due dates, recurrence patterns, and compliance rates. Monitor overdue and upcoming PMs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/limble-cmms](https://vinkius.com/mcp/limble-cmms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Limble CMMS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `limble-cmms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Limble CMMS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "limble-cmms": {
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
