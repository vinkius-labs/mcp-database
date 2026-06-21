# KeepTruckin MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/keeptruckin)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/keeptruckin-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/keeptruckin-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [shipping-logistics](../categories/shipping-logistics.md)

Manage your fleet and assets via KeepTruckin — track locations, monitor reefer sensors, and analyze vehicle utilization directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **KeepTruckin** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active assets in our fleet."

**🤖 AI Agent:**
> I've retrieved the list of active assets. You have 12 assets currently active, including 'Truck-01' (ID: 55021) and 'Trailer-A' (ID: 55022). Would you like to locate one of them?

---

**👤 You:**
> "Show me the utilization for vehicle ID 55021 from yesterday."

**🤖 AI Agent:**
> Fetching utilization data for vehicle 55021... For yesterday, the vehicle had 6.5 hours of driving time, 42 minutes of idle time, and consumed 38.2 gallons of fuel over 310 miles.

---

**👤 You:**
> "Locate asset ID 55022 and check its reefer status."

**🤖 AI Agent:**
> Asset 55022 is currently located at 34.0522° N, 118.2437° W (Los Angeles, CA). The reefer activity report shows a set point of 34°F with an ambient temperature of 72°F. Fuel level is at 85%.


## Installation & Usage

To install and use the **KeepTruckin** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/keeptruckin](https://vinkius.com/mcp/keeptruckin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
