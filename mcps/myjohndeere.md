# MyJohnDeere MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/myjohndeere)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/myjohndeere-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/myjohndeere-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Manage agricultural operations via MyJohnDeere — list organizations, equipment assets, fields, and machine telematics directly from any AI agent.

## Description
Connect your **MyJohnDeere** account to any AI agent to monitor and manage your precision agriculture data through natural conversation.

### What you can do

- **Organization Management** — List all organizations, including farms and dealerships, associated with your account.
- **Asset Tracking** — Fetch detailed lists of physical machinery and equipment assets for any specific organization.
- **Field & Land Analysis** — Retrieve field lists and precise spatial boundaries to understand your land layout.
- **Telematics & Sensor Data** — Access real-time machine measurements and sensor data for specific equipment.
- **Data File Access** — List and manage data files associated with your agricultural operations for deeper analysis.

### How it works

1. Subscribe to this server
2. Enter your MyJohnDeere Access Token
3. Start querying your fleet and field data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Farm Managers** — quickly check equipment locations and field statuses without navigating complex dashboards.
- **Agronomists** — retrieve field boundaries and operational files directly into your analysis workflow.
- **Fleet Operators** — monitor machine measurements and telematics to ensure optimal equipment performance.


## Available Tools
- **list_fields**: List fields for an organization
- **list_machine_measurements**: List measurements for a specific machine
- **list_organizations**: g., farms, dealerships) available to the authenticated user.

List MyJohnDeere organizations
- **list_assets**: List assets (equipment) for an organization
- **list_boundaries**: List boundaries for a specific field
- **list_files**: List files (data) for an organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MyJohnDeere** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my MyJohnDeere organizations."

**🤖 AI Agent:**
> I've found 2 organizations associated with your account: 'Green Valley Farm' (ID: 12345) and 'Central Plains Ops' (ID: 67890). Which one would you like to explore?

---

**👤 You:**
> "Show me the equipment assets for organization 12345."

**🤖 AI Agent:**
> Retrieving assets for Green Valley Farm... I found 3 active machines: a 8R 370 Tractor (ID: T100), a S780 Combine (ID: C200), and a R4038 Sprayer (ID: S300).

---

**👤 You:**
> "Get the latest telematics measurements for machine T100 in org 12345."

**🤖 AI Agent:**
> Fetching telematics for Tractor T100... Current fuel level is 65%, engine load is at 42%, and the GPS location is confirmed at the North Field boundary.


## Installation & Usage

To install and use the **MyJohnDeere** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/myjohndeere](https://vinkius.com/mcp/myjohndeere)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
