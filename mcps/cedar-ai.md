# Cedar AI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cedar-ai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cedar-ai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cedar-ai-mcp)
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


## Installation & Usage

To install and use the **Cedar AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cedar-ai](https://vinkius.com/mcp/cedar-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
