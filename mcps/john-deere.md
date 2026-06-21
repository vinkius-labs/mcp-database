# John Deere MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/john-deere)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/john-deere-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/john-deere-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Monitor farm operations via John Deere APIs — track machines, map fields, review planting and harvest data from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **John Deere** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all machines in my main farm and their current locations."

**🤖 AI Agent:**
> Your farm 'Sunrise Acres' (org: 384721) has 6 machines:
1. John Deere 8R 410 (SN: 1RW8410RJPD002871) — 2,340 hrs — GPS: 41.284° N, 96.012° W (Field: North Quarter)
2. S790 Combine (SN: 1H0S790SJN0770123) — 890 hrs — Parked at equipment barn
3. R4045 Sprayer (SN: 1N04045XLMD210456) — 1,120 hrs — GPS: 41.291° N, 96.008° W (Field: East 160)
Showing 3 of 6. Want me to check active alerts for any of these?

---

**👤 You:**
> "What was the corn yield on the North Quarter field this season?"

**🤖 AI Agent:**
> Harvest operation for North Quarter (Field ID: F-4821):
• Crop: Corn (Zea mays)
• Harvest date: October 12, 2025
• Yield: 218 bu/acre (area: 156.3 acres)
• Total harvest: 34,073 bushels
• Moisture: 15.2%
• Operator: Mike Johnson
This is 8% above your 5-year average of 202 bu/acre for this field. Want me to compare with your other corn fields?

---

**👤 You:**
> "Are there any active alerts on my fleet?"

**🤖 AI Agent:**
> 3 active alerts found:
1. ⚠️ HIGH — 8R 410 Tractor: Engine oil pressure low (triggered 2h ago). Recommend stopping for inspection.
2. 🔔 MEDIUM — R4045 Sprayer: Nozzle calibration overdue (last calibrated 45 days ago)
3. ℹ️ LOW — S790 Combine: Scheduled maintenance at 900 engine hours (currently at 890 hrs)
The tractor alert is urgent. Should I pull the full machine details?


## Installation & Usage

To install and use the **John Deere** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/john-deere](https://vinkius.com/mcp/john-deere)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
