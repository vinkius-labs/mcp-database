# HiBob MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hibob)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hibob-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hibob-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate HR workflows via HiBob — manage employees, time off, and tasks directly from any AI agent.

## Description
Connect your **HiBob** HR platform to any AI agent and take full control of your people management and organizational data through natural conversation.

### What you can do

- **Employee Search** — Perform advanced searches for employees, retrieve full profiles, and access custom fields.
- **Time Off Oversight** — Monitor who is out of the office, check leave balances, and submit new time off requests.
- **Task Management** — List all open HR tasks and mark them as completed directly from the chat interface.
- **Payroll & Compensation** — Access historical payroll data and retrieve detailed compensation packages for employees.
- **Operational Efficiency** — Send welcome invitations to new hires and monitor organizational lists and configurations.
- **Public Profiles** — Quickly retrieve basic contact information for any active member of your organization.

### How it works

1. Subscribe to this server
2. Enter your HiBob Service User API Token
3. Start managing your HR operations from Claude, Cursor, or any MCP-compatible client

No more manual exporting of employee spreadsheets. Your AI assistant acts as a dedicated HR Coordinator or People Ops Specialist.

### Who is this for?

- **HR Managers** — instantly retrieve employee data and check leave compliance during planning.
- **Team Leads** — monitor who is out from your team and manage pending approval tasks.
- **Operations Leaders** — automate the oversight of payroll history and employee onboarding steps.


## Available Tools
- **complete_task**: Mark a specific task as completed
- **get_leave_balance**: Get the leave balance for a specific employee
- **get_employee_compensation**: Get detailed salary and benefit information for an employee
- **get_payroll_history**: Retrieve platform payroll history
- **list_public_profiles**: List basic contact information for all active employees
- **get_whos_out**: List employees on leave for a specific date range
- **invite_employee**: Send a welcome invitation to a new employee
- **list_company_settings_lists**: List custom dropdown and configuration lists used in the platform
- **list_open_tasks**: List all pending tasks across the company
- **search_employees**: Pass search criteria as a JSON string in "search_json". Returns active employees by default.

Search for employees using filters and retrieve profiles
- **request_time_off**: Pass the payload as a JSON string in "request_json" (requires policyType, startDate, endDate).

Submit a new time off request for an employee


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HiBob** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for employees in the 'Engineering' department."

**🤖 AI Agent:**
> I've searched your team. I found 12 employees in the Engineering department, including 'Mark Thompson' (Lead Engineer), 'Sarah Chen', and 'David Miller'. Would you like to see the contact details for any of them?

---

**👤 You:**
> "Check who is out of the office this week."

**🤖 AI Agent:**
> Retrieving leave data... There are 3 employees out this week: 'Maria Garcia' (Vacation until Friday), 'John Doe' (Sick leave), and 'Elena Rossi'. Should I check the pending approval tasks for their replacements?

---

**👤 You:**
> "Show my open HR tasks and complete ID 'task_992'."

**🤖 AI Agent:**
> Task list retrieved! You had 5 open items. I have successfully marked 'task_992' (Onboarding Check) as completed. You now have 4 tasks remaining. Would you like me to list them?


## Installation & Usage

To install and use the **HiBob** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hibob](https://vinkius.com/mcp/hibob)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
