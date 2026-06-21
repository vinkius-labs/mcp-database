# Homebase MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/homebase)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/homebase-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/homebase-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate employee scheduling and time tracking via Homebase — manage shifts, locations, and timecards directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Homebase** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all business locations and find the UUID for 'Downtown Cafe'."

**🤖 AI Agent:**
> I've retrieved your locations. You have 3 sites: 'Downtown Cafe' (UUID: hbc_102), 'Airport Kiosk' (UUID: hbc_105), and 'Main Warehouse'. Which location's schedule would you like to check?

---

**👤 You:**
> "Who is currently clocked in at the Downtown Cafe?"

**🤖 AI Agent:**
> Checking active clock-ins for Downtown Cafe (hbc_102)... Currently, 4 employees are on-site: 'Alice Smith' (Barista), 'John Doe' (Manager), 'Michael Brown', and 'Elena Rossi'. Would you like to see their scheduled shift end times?

---

**👤 You:**
> "Show the scheduled shifts for next Wednesday."

**🤖 AI Agent:**
> Retrieving schedules... For next Wednesday (April 14th) at your primary location, 6 shifts are scheduled, starting with 'Morning Prep' at 06:00 AM and ending with 'Closing Duty' at 10:00 PM. Should I list the assigned employees for each shift?


## Installation & Usage

To install and use the **Homebase** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/homebase](https://vinkius.com/mcp/homebase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
