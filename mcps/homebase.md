# Homebase MCP Server

Automate employee scheduling and time tracking via Homebase — manage shifts, locations, and timecards directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/homebase)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **Homebase** (joinhomebase.com) account to any AI agent and take full control of your employee scheduling, time tracking, and team management through natural conversation.

### What you can do

- **Location Oversight** — List all business locations and retrieve unique identifiers for multi-site management.
- **Employee Management** — Access lists of employees for specific locations and retrieve detailed profile information.
- **Schedule Monitoring** — List scheduled shifts and retrieve upcoming agendas to ensure adequate coverage.
- **Time Tracking** — Monitor actual hours worked by retrieving timecard entries, including clock-in/out times.
- **Real-time Presence** — Instantly check which employees are currently clocked in at a specific location.
- **Role & Department Tracking** — List defined roles and departments to understand your team structure.
- **Operational Efficiency** — Retrieve labor budget configurations to stay aligned with your operational costs.

### How it works

1. Subscribe to this server
2. Enter your Homebase API Key (from Settings > API Access)
3. Start managing your team from Claude, Cursor, or any MCP-compatible client

No more manual exporting of timesheets for simple availability checks. Your AI assistant acts as a dedicated Schedule Coordinator or Operations Manager.

### Who is this for?

- **Store Managers** — instantly check team presence and upcoming shifts without leaving the floor.
- **Operations Leaders** — monitor labor costs and timecard compliance across multiple locations.
- **HR Specialists** — automate the process of retrieving employee profiles and role assignments.


## Available Tools
- **get_active_clock_ins**: List all employees currently clocked in at a specific location
- **get_employee_profile**: Get detailed information for a specific employee
- **get_api_profile**: Retrieve information about the authenticated user and plan status
- **list_departments**: List all departments configured for a location
- **list_employees**: List all employees for a specific location
- **list_labor_budgets**: Retrieve labor budget configurations for a location
- **list_locations**: Use this to find the "location_uuid" required for all other tools.

List all business locations associated with the Homebase account
- **list_defined_roles**: List all roles (e.g., Manager, Server) defined for a location
- **list_scheduled_shifts**: List scheduled shifts for employees at a specific location
- **list_timecards**: Useful for monitoring actual hours worked.

List timecard entries (timesheets) for a specific location


## Installation & Usage

To install and use the **Homebase** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/homebase](https://vinkius.com/mcp/homebase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
