# Onfleet MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/onfleet)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/onfleet-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/onfleet-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage last-mile deliveries via Onfleet — create tasks, track drivers, check ETAs, and complete orders directly from any AI agent.

## Description
Connect your **Onfleet** delivery operations to any AI agent and run your fleet from a single conversation.

### What you can do

- **Delivery Tasks** — Create, update, delete, and force-complete delivery tasks with full address and recipient details
- **Fleet Tracking** — List all active drivers, check who's online, and view their assigned capacities in real time
- **Driver Schedules** — Pull exact shift times and availability windows for any worker in your fleet
- **Teams & Hubs** — Browse your team structure and dispatch hubs with geographic coordinates and zone coverage
- **Task History** — Query tasks by date range to audit completed, failed, or pending deliveries across your operation

### How it works

1. Subscribe to this server
2. Enter your Onfleet API Key
3. Start dispatching and tracking deliveries from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics managers** — monitor fleet performance and driver availability without switching between dashboards
- **Ops teams** — create and update delivery tasks on the fly, resolve exceptions, and force-complete stuck orders
- **Customer support** — look up any delivery by ID to get real-time ETA and driver location for customer inquiries


## Available Tools
- **complete_task_override**: Force-complete a delivery task
- **create_delivery_task**: Create a new delivery task in Onfleet
- **delete_delivery_task**: Delete/Archive a delivery task
- **list_dispatch_hubs**: List all dispatch hubs
- **get_task_details**: Get details for a specific delivery task
- **list_tasks_by_date**: List delivery tasks within a date range
- **list_fleet_teams**: List all delivery teams
- **get_worker_schedule**: Get a driver's work schedule
- **list_fleet_workers**: List all fleet drivers/workers
- **update_delivery_task**: Update an existing delivery task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Onfleet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a delivery task to 123 Main St, San Francisco for John Doe with phone 415-555-0100."

**🤖 AI Agent:**
> Task created successfully. Tracking ID: 8f3a...b2c1. Destination: 123 Main St, San Francisco, CA. Recipient: John Doe (415-555-0100). Status: unassigned. The task is ready to be auto-assigned to the nearest available driver. Want me to check which drivers are currently online?

---

**👤 You:**
> "Show me all deliveries from yesterday with their status."

**🤖 AI Agent:**
> Found 47 tasks from yesterday. 41 completed successfully (87.2%), 3 failed (wrong address), 2 cancelled by customer, and 1 still pending. The failed deliveries are task IDs a4f2..., b3e1..., and c7d8.... Want me to pull the details on the failed ones?

---

**👤 You:**
> "Which drivers are online right now and how many active tasks does each have?"

**🤖 AI Agent:**
> 5 drivers currently online. Maria Chen — 3 active tasks, last seen at Market St. Alex Rivera — 6 active tasks (at capacity). Tom Wilson — 1 active task, available for more. Sarah Kim — 4 active tasks. Jake Patel — 0 active tasks, standing by at Hub North. Want me to pull Tom's schedule to confirm his shift end time?


## Installation & Usage

To install and use the **Onfleet** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/onfleet](https://vinkius.com/mcp/onfleet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
