# UKG Pro Workforce Management MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ukg-pro-workforce-management)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ukg-pro-workforce-management-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ukg-pro-workforce-management-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage schedules, timesheets, accruals, and time-off requests via UKG Pro WFM.

## Description
The UKG Pro Workforce Management (WFM) MCP Server provides AI agents with direct access to UKG Dimensions/WFM APIs, allowing them to retrieve employee schedules, managing time-off, querying timesheets, and fetching accrual balances across the workforce.


## Available Tools
- **accruals**: List accrual balances (e.g. sick leave, PTO)
- **schedules**: List schedules for employees
- **timeoff**: List time off requests for employees
- **timesheets**: List timesheets for employees


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UKG Pro Workforce Management** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get John Doe's work schedule for this week."

**🤖 AI Agent:**
> John Doe is scheduled for 40 hours this week: Monday-Friday from 9 AM to 5 PM EST.

---

**👤 You:**
> "Check the available PTO (Paid Time Off) balance for employee ID 9921."

**🤖 AI Agent:**
> Querying UKG Dimensions accrual metrics ('get_accruals')...
Employee ID 9921 currently has exactly 112 hours (14 days) of accrued PTO available.

---

**👤 You:**
> "List any missing timesheet punches for our front-line staff today."

**🤖 AI Agent:**
> Executing `check_time_punches`...
Detected 2 exceptions for front-line associates today:
1. Alex M. missed clock out at 4:00 PM
2. David K. missed clock in for the 1:00 PM shift


## Installation & Usage

To install and use the **UKG Pro Workforce Management** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ukg-pro-workforce-management](https://vinkius.com/mcp/ukg-pro-workforce-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
