# MaintainX MCP Server

Manage work orders, assets, and facility locations via the MaintainX REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/maintainx)

## Overview
**Category:** operations-management
**Tools Count:** 8

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


## Installation & Usage

To install and use the **MaintainX** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/maintainx](https://vinkius.com/mcp/maintainx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
