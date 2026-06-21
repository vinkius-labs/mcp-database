# KeepTruckin MCP Server

Manage your fleet and assets via KeepTruckin — track locations, monitor reefer sensors, and analyze vehicle utilization directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/keeptruckin)

## Overview
**Category:** shipping-logistics
**Tools Count:** 10

## Description
Connect your **KeepTruckin** (Motive) account to any AI agent to streamline fleet operations and asset tracking through natural language conversation.

### What you can do

- **Asset Management** — List all company assets, lookup specific units by external IDs, and create or update asset records in your inventory.
- **Real-time Tracking** — Trigger immediate location updates for specific assets to know exactly where your equipment is at any moment.
- **Cold Chain Monitoring** — Access detailed reefer activity reports and sensor samples, including temperature and humidity metrics, to ensure cargo safety.
- **Fleet Safety** — Monitor camera connection events to keep track of hardware status, associated drivers, and vehicle safety connectivity.
- **Operational Analytics** — Retrieve comprehensive vehicle utilization data, including driving time, idle time, fuel usage, and distance traveled.
- **Dispatching** — Create team dispatches to assign multiple authorized drivers to a single trip efficiently.

### How it works

1. Subscribe to this server
2. Enter your KeepTruckin API Key
3. Start managing your fleet operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fleet Managers** — monitor asset locations and vehicle health without toggling between multiple dashboards
- **Logistics Coordinators** — verify reefer temperatures and manage team dispatches through simple queries
- **Safety Officers** — check camera connectivity and driver associations to maintain compliance standards


## Available Tools
- **list_assets**: List all company assets
- **list_camera_connections**: List Camera Connection Events
- **create_asset**: Create a new asset
- **create_team_dispatch**: Create Team Dispatches (V1, V2, V3)
- **locate_asset**: Locate an asset
- **lookup_asset_by_external_id**: Lookup asset by External ID
- **list_reefer_activity_reports**: Reefer Activity Report
- **list_reefer_sensor_samples**: List Sensor Samples for Reefers
- **update_asset**: Update an existing asset
- **get_vehicle_utilization**: Fetch Vehicle Utilization (V2)


## Installation & Usage

To install and use the **KeepTruckin** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/keeptruckin](https://vinkius.com/mcp/keeptruckin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
