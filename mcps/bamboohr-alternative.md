# BambooHR MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bamboohr-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bamboohr-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bamboohr-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Human Resources management platform — organize employee data, track time off, and audit HR workflows via AI.

## Description
Empower your AI agent to orchestrate your entire HR ecosystem with **BambooHR**, the leading platform for small and medium businesses. By connecting BambooHR to your agent, you transform complex employee management into a natural conversation. Your agent can instantly list the company directory, audit employee profiles, and retrieve detailed data tables like compensation history without you ever touching a dashboard. Whether you are managing a growing startup or an established enterprise, your agent acts as a real-time HR operations manager, ensuring your people data is always structured and accessible.

### What you can do

- **Employee Directory** — List all active employees in your organization and access their basic contact and role information.
- **Deep Profile Inspection** — Fetch complete metadata, job titles, departments, and specific field details for any individual employee.
- **Time Off Tracking** — Monitor and analyze time off requests, including status filtering (pending, approved) and date ranges.
- **Data Table Auditing** — Access structured historical data such as job history, compensation, and other internal tables.
- **Custom Reporting** — Generate targeted reports on the fly by specifying exactly which employee fields you need to analyze.

### How it works

1. Subscribe to this server
2. Enter your BambooHR Subdomain and API Key
3. Start managing your HR data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Managers** — instantly retrieve employee statuses, audit time off balances, and inspect organizational charts without manual dashboard navigation.
- **Operations Leads** — perform rapid health checks on department staffing and compensation structures directly from chat.
- **IT & Security Teams** — verify employee roles and metadata for access control audits and organizational planning.
- **Team Leaders** — stay updated on their team's availability and profile details through simple natural language queries.


## Available Tools
- **get_custom_report**: Requires a JSON list of fields.

Generate a custom report
- **get_employee**: You can specify fields to retrieve.

Get details for a specific employee
- **get_employee_table**: g., compensation history).

Get data from an employee table
- **list_employees**: List all employees in the company directory
- **list_employee_files**: List files for an employee
- **list_meta_fields**: List available employee fields
- **list_meta_tables**: g., Job Info, Compensation) in BambooHR.

List available data tables
- **list_time_off_requests**: List time off requests
- **update_employee**: Note: BambooHR uses POST for updates.

Update employee data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BambooHR** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all employees in the organization directory."

**🤖 AI Agent:**
> I've retrieved your employee directory. You currently have 45 active employees, including 'John Doe' (Engineering) and 'Jane Smith' (Marketing). Would you like to inspect a specific profile?

---

**👤 You:**
> "Show the job history for employee ID 123."

**🤖 AI Agent:**
> Fetching job history for employee 123... They started as 'Junior Developer' in 2021 and were promoted to 'Senior Developer' in 2023. I have the full list of department changes as well.

---

**👤 You:**
> "Find all pending time off requests from last month."

**🤖 AI Agent:**
> I've scanned the requests from last month. There are 4 pending requests that need review, including a 3-day personal leave from 'Alice Johnson'. Shall I list the dates for you?


## Installation & Usage

To install and use the **BambooHR** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bamboohr-alternative](https://vinkius.com/mcp/bamboohr-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
