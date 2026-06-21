# Deputy MCP Server

Equip your AI agent to manage employee rosters, track timesheets, and monitor leave requests via the Deputy API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/deputy)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Integrate **Deputy**, the ultimate workforce management solution, directly into your AI workflow. Manage your employee directory, monitor real-time shift rosters, track submitted timesheets, and handle leave requests using natural language.

### What you can do

- **Workforce Visibility** — List and retrieve detailed profiles for all employees in your Deputy organization.
- **Roster Monitoring** — Track current and upcoming shift rosters to ensure proper coverage across locations.
- **Timesheet Tracking** — Review submitted timesheets, including actual start and end times and approval statuses.
- **Leave Management** — List and monitor employee leave and time-off requests pending approval.

### How it works

1. Connect the Deputy integration to your AI assistant.
2. Authorize using your Deputy API Token and account Subdomain.
3. Optimize your team operations and scheduling through intuitive conversation.

### Who is this for?

- **Operations Managers** — Quickly check who is currently clocked in and shift coverage on the go.
- **HR & Payroll Teams** — Audit timesheets and monitor leave balances via chat.
- **Team Leads** — Review rosters and manage employee profiles during scheduling meetings.


## Available Tools
- **get_employee_profile**: Get detailed information for a specific employee
- **get_authenticated_user**: Retrieve metadata for the current authenticated API user
- **list_currently_active_shifts**: Identify employees who are currently clocked in (mock logic)
- **list_workforce_employees**: List all employees in your Deputy organization
- **list_leave_requests**: List all employee leave and time-off requests
- **list_business_locations**: List all physical business locations (companies) configured in Deputy
- **list_pending_leave_approvals**: List only the leave requests that are awaiting manager approval
- **list_active_rosters**: List all current and upcoming shift rosters
- **list_completed_timesheets**: List timesheets submitted by employees
- **search_employees_by_name**: Search for an employee by their display name


## Installation & Usage

To install and use the **Deputy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deputy](https://vinkius.com/mcp/deputy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
