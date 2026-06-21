# Cedar AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cedar-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Process insurance documents with AI that extracts claims data, validates coverage, and accelerates underwriting decisions.

## Description
Connect your **Cedar AI** railway management account to any AI agent and simplify how you coordinate rail operations, track car movements, and manage logistics documentation through natural conversation.

### What you can do

- **Inventory Management** — List all railcars currently in your facility and retrieve detailed metadata and status for individual units.
- **Car Movement Tracking** — Record placements (setouts) and removals (pickups) of railcars at specific locations or tracks.
- **Logistics Documentation** — List and query waybills to understand shipping instructions, routes, and commodity data.
- **Work Order Control** — Manage the lifecycle of movement instructions by listing and updating work orders and associated tasks.
- **Consist Coordination** — Record train arrivals and departures to keep your inventory and operations synchronized.
- **Status Maintenance** — Update railcar tags and conditions (e.g., Bad Order, Empty/Loaded) directly via AI commands.

### How it works

1. Subscribe to this server
2. Enter your Cedar AI API Key (found in your developer settings)
3. Start managing your railway ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **Railroad Operators & Terminal Managers** — quickly check yard inventory and record car movements via simple AI queries.
- **Logistics Coordinators** — monitor waybills and manage work orders across different tracks directly from the workspace.
- **Fleet Managers** — track railcar statuses and conditions to optimize equipment availability via the AI assistant.


## Available Tools
- **arrive_train**: Record train arrival
- **depart_train**: Record train departure
- **get_railcar_details**: Get details for a specific railcar
- **get_waybill_details**: Get details for a specific waybill
- **get_work_order_details**: Get details for a specific work order
- **list_inventory**: List railcars currently in inventory
- **list_waybills**: List waybills
- **list_work_orders**: List work orders
- **pickup_cars**: Record removal of cars
- **setout_cars**: Record placement of cars
- **update_railcar_status**: g., Bad Order, Clean, Loaded/Empty).

Update status of a railcar
- **update_work_order**: Update a work order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cedar AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all railcars currently in the main yard inventory."

**🤖 AI Agent:**
> I've retrieved the railcar inventory. You have 15 cars in the main yard including: TBOX 12345 (Loaded), BNSF 98765 (Empty), and GATX 5521 (Bad Order). Would you like detailed metadata for any of them?

---

**👤 You:**
> "Record a setout of cars 'TBOX 101, TBOX 102' at 'Customer Track 4'."

**🤖 AI Agent:**
> Placement recorded! I've logged the setout for railcars TBOX 101 and TBOX 102 at Customer Track 4. The inventory status has been updated successfully in Cedar AI.

---

**👤 You:**
> "Show me the details for waybill 'WB-88231'."

**🤖 AI Agent:**
> Fetching waybill details... WB-88231 is an active shipment for 'Lumber' from Portland to Houston via CONSIST-102. It contains 3 flatcars. Would you like to see the movement history?


## ❓ FAQ

**Q: Can I record a railcar movement via AI?**
Yes! Use the `setout_cars` tool to record placement or `pickup_cars` for removal. Provide the location name and a list of railcar IDs to log the movement instantly.

**Q: How do I see the latest waybills for my shipments?**
Run the `list_waybills` query. The agent will retrieve a history of active and completed shipping instructions, including route details and commodity info.

**Q: Is it possible to check the status of a specific work order via AI?**
Absolutely. Use the `get_work_order_details` tool with the Work Order ID to retrieve the current status, assigned tasks, and completion progress.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cedar-ai](https://vinkius.com/mcp/cedar-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cedar AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cedar-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cedar AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cedar-ai": {
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
