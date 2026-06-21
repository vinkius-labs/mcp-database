# 7shifts MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/7shifts-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/7shifts-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/7shifts-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Schedule restaurant staff, manage shifts, track labor costs, and coordinate your team with intelligent workforce planning.

## Description
Connect your **7shifts** restaurant management account to any AI agent and simplify how you coordinate your workforce, manage shift assignments, and track labor costs through natural conversation.

### What you can do
- **Employee Management** — List all staff members, create new employee profiles, and retrieve detailed metadata for individual users.
- **Shift Coordination** — Create, list, and monitor work assignments across different locations and departments.
- **Schedule Oversight** — List all work weeks (schedules) to understand your staffing coverage and planning.
- **Labor Tracking** — List actual time punches to monitor clock-in/out times and verify labor compliance.
- **Organization Control** — Query business locations, employee roles, and departments to manage your restaurant's structure.
- **Operational Visibility** — Check account status and monitor configured webhooks for real-time schedule events.

### How it works
1. Subscribe to this server
2. Enter your 7shifts Company GUID and Token (found in your developer settings)
3. Start managing your restaurant team from Claude, Cursor, or any MCP client

### Who is it for?
- **Restaurant Managers** — quickly retrieve staff lists and verify shift coverage via simple AI commands.
- **Operations Teams** — create new work assignments and monitor time clock entries directly from the workspace.
- **Business Owners** — get instant bird's-eye views of active shifts and team structure via the AI assistant.


## Available Tools
- **create_employee**: Create a new employee
- **create_shift**: Create a new shift
- **get_account_info**: Get my profile
- **get_employee**: Get employee details
- **list_departments**: List departments
- **list_employees**: List all employees
- **list_locations**: List business locations
- **list_roles**: List employee roles
- **list_schedules**: List all schedules
- **list_shifts**: List all shifts
- **list_time_punches**: List time clock entries
- **list_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **7shifts** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all employees in my 7shifts account."

**🤖 AI Agent:**
> I've retrieved your employee list. You have 15 active staff members including 'Alex Rivera', 'Sarah Chen', and 'Mike Ross'. Which one would you like to see the shifts for?

---

**👤 You:**
> "Show me the shifts for 'Alex Rivera' (ID: user_10293)."

**🤖 AI Agent:**
> I've fetched the shifts for Alex. He has 3 assignments this week: Tuesday (10:00 - 18:00), Thursday (12:00 - 20:00), and Saturday (08:00 - 16:00). All are scheduled at the 'Downtown' location.

---

**👤 You:**
> "Create a new shift at location 'loc_8823' for tomorrow from 09:00 to 17:00."

**🤖 AI Agent:**
> Success! A new work assignment has been created for tomorrow (09:00 - 17:00) at the Downtown unit. It is currently unassigned. Would you like me to assign an employee to it?


## Installation & Usage

To install and use the **7shifts** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/7shifts-alternative](https://vinkius.com/mcp/7shifts-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
