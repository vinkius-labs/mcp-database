# John Deere MCP Server

Monitor farm operations via John Deere APIs — track machines, map fields, review planting and harvest data from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/john-deere)

## Overview
**Category:** iot-hardware
**Tools Count:** 7

## Description
Connect your **John Deere** Operations Center to any AI agent and manage fleet, field, and agronomic data through natural conversation instead of switching between dashboards.

### What you can do

- **Organizations & Farms** — List all farms, cooperatives, and organizations you manage with their full profiles
- **Fleet Management** — View every tractor, combine, and sprayer with serial numbers, engine hours, and make/model details
- **Real-Time GPS** — Get live machine positions and telemetry data to know exactly where your equipment is operating
- **Field Mapping** — List all agricultural fields with boundaries, acreage, and current crop assignments
- **Operation History** — Review planting, spraying, harvesting, and tillage records with product rates, yields, and operators
- **Alerts & Clients** — Monitor machine alerts by severity and manage grower and landowner relationships

### How it works

1. Subscribe to this server
2. Enter your John Deere App ID, App Secret, and OAuth Access Token from developer.deere.com
3. Start managing your farm operations from Claude, Cursor, or any MCP-compatible client

John Deere is the world's leading manufacturer of agricultural machinery and precision farming technology, trusted by millions of farmers.

### Who is this for?

- **Farm Managers** — check machine locations and field operation status without opening the Operations Center app
- **Agronomists** — pull planting and yield data for specific fields to build season analysis reports instantly
- **Fleet Coordinators** — monitor alerts across the entire fleet and identify machines needing maintenance


## Available Tools
- **list_organizations**: Each org has machines, fields, and clients.

List farms and organizations
- **list_machines**: List fleet machines
- **get_machine_locations**: Get machine GPS locations
- **list_fields**: List fields/plots
- **get_field_operations**: Includes date, product, rate, yield, and operator.

Get field operations
- **list_alerts**: Includes alert type, severity, timestamp, and affected machine.

List machine alerts
- **list_clients**: List farm clients


## Installation & Usage

To install and use the **John Deere** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/john-deere](https://vinkius.com/mcp/john-deere)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
