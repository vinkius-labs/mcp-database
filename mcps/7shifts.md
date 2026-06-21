# 7shifts MCP Server

Restaurant workforce management — manage employee schedules, time-off, and staff profiles via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/7shifts)

## Overview
**Category:** productivity
**Tools Count:** 6

## Description
Connect your **7shifts** account to your AI agent to streamline restaurant workforce management. From creating weekly schedules to auditing employee time-off requests, your agent handles staffing operations through natural conversation.

### What you can do

- **Employee Management** — List all staff members, create new profiles, and manage employee technical details
- **Scheduling & Shifts** — Create, view, and update work shifts for your entire team across different locations
- **Time-Off Requests** — Audit pending or approved time-off and submit new requests on behalf of employees
- **Labor Tracking** — Access time punch data and monitor clock-in/out patterns for payroll accuracy
- **Location Organization** — Manage multiple restaurant locations, departments, and roles seamlessly

### How it works

1. Subscribe to this server
2. Enter your 7shifts API Key
3. Start managing your restaurant's schedule and staff through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Restaurant Managers** — build weekly schedules and handle staff changes without manual spreadsheet work
- **Business Owners** — monitor labor costs and employee attendance across multiple locations
- **HR Coordinators** — manage employee records and time-off requests efficiently
- **Operations Leads** — automate staffing reports and schedule notifications


## Available Tools
- **list_employees**: Retrieve all employees registered in the 7shifts company account
- **create_employee**: Requires name and email.

Create a new staff profile inside 7shifts with basic contact information
- **list_shifts**: Retrieve scheduled work shifts from 7shifts, filterable by date or location
- **create_shift**: Requires user_id, location_id, and ISO 8601 start/end times.

Assign a new work shift to a 7shifts employee for a specific date and time
- **list_time_off**: Retrieve pending or approved employee time-off requests from 7shifts
- **list_locations**: Retrieve all locations, departments, and roles configured in the 7shifts account


## Installation & Usage

To install and use the **7shifts** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/7shifts](https://vinkius.com/mcp/7shifts)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
