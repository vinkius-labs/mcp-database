# OptimoRoute MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/optimoroute-1)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/optimoroute-1-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/optimoroute-1-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics-supply-chain](../categories/logistics-supply-chain.md)

Optimize delivery routes via OptimoRoute — create orders, track driver locations, and manage route planning directly from any AI agent.

## Description
Connect your **OptimoRoute** account to any AI agent and take full control of your logistics and delivery operations through natural conversation.

### What you can do

- **Order Management** — Create, retrieve, and delete delivery orders with precise location metadata.
- **Route Oversight** — List planned routes for any specific date to maintain visibility over your daily operations.
- **Real-time Tracking** — Get live driver locations and stop sequences to provide accurate updates to customers.
- **Optimization Planning** — Start and monitor route optimization tasks to ensure maximum efficiency.
- **Performance Analytics** — Extract delivery analytics to audit your logistics performance over time.

### How it works

1. Subscribe to this server
2. Enter your OptimoRoute API Key
3. Start optimizing your deliveries from Claude, Cursor, or any MCP client

### Who is this for?

- **Logistics Managers** — quickly check the status of a daily route or verify a driver's location without touching the dashboard.
- **Dispatchers** — create new orders and initiate planning tasks directly through the agent.
- **Operations Teams** — audit delivery performance and stop sequences during the work day.


## Available Tools
- **create_order**: Create a new delivery order
- **delete_order**: Delete a delivery order
- **get_analytics**: Get delivery performance analytics
- **get_driver_locations**: Get real-time driver locations
- **get_order**: Get details for a specific order
- **get_planning_status**: Check status of an optimization task
- **list_routes**: List routes for a specific date
- **get_stop_sequence**: Get stop sequence for a driver
- **list_drivers**: List all drivers
- **start_planning**: Start route optimization for a date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OptimoRoute** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new delivery order #ABC-123 for 123 Main St for tomorrow."

**🤖 AI Agent:**
> Order #ABC-123 has been successfully created for the location '123 Main St' scheduled for 2026-10-25.

---

**👤 You:**
> "Show me the real-time locations of all my drivers."

**🤖 AI Agent:**
> I've retrieved the fleet status. Driver John is at (40.7128, -74.0060), Driver Sarah is at (34.0522, -118.2437), and 3 others are currently on their routes.

---

**👤 You:**
> "Start route optimization for today's pending orders."

**🤖 AI Agent:**
> Route optimization has been started for 2026-10-24. Planning ID: 98765. You can check the status using the `get_planning_status` tool.


## Installation & Usage

To install and use the **OptimoRoute** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/optimoroute-1](https://vinkius.com/mcp/optimoroute-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
