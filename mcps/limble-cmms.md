# Limble CMMS MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/limble-cmms)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/limble-cmms-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/limble-cmms-mcp)
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


## Available Tools
- **get_asset_details**: Get details for a specific asset
- **list_labor_entries**: List labor logs for tasks
- **list_asset_part_relations**: List parts linked to assets
- **list_assets**: List maintenance assets
- **list_locations**: List facility locations
- **list_parts**: List inventory parts
- **list_tasks**: List work orders and PMs
- **list_vendors**: List maintenance vendors
- **update_asset_field**: g. runtime hours, temperature) for an asset.

Update a custom field for an asset


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


## Installation & Usage

To install and use the **Limble CMMS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/limble-cmms](https://vinkius.com/mcp/limble-cmms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
