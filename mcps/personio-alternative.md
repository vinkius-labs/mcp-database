# Personio MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/personio-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/personio-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/personio-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Automate HR operations via Personio — manage employee records, track attendance, handle absences, and streamline recruiting directly from any AI agent.

## Description
Connect your **Personio** HR platform to any AI agent to streamline your people operations and recruitment workflows through natural conversation.

### What you can do

- **Employee Management** — List, create, and update employee records (v1) or persons (v2) with full support for custom attributes.
- **Attendance & Absences** — Log daily working hours, manage attendance records, and track employee absences efficiently.
- **Recruiting Pipeline** — Access job listings, manage candidates, and track applications to accelerate your hiring process.
- **Custom Reporting** — Fetch data from your custom Personio reports directly into your AI workspace for instant analysis.
- **Webhooks** — Monitor and manage HR event triggers to keep your external systems in sync.

### How it works

1. Subscribe to this server
2. Enter your Personio Client ID and Client Secret (and optionally your Recruiting Token)
3. Start managing your HR tasks from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Managers** — quickly retrieve employee data, check attendance logs, and generate report summaries without manual exports.
- **Recruiters** — list open jobs and candidates to stay on top of the hiring pipeline directly from the chat.
- **Team Leads** — verify team attendance and absence statuses to plan sprints and resources effectively.


## Available Tools
- **create_absence**: Create an absence record
- **create_application**: Post a new recruiting application (v1)
- **create_attendance**: Periods cannot span across two days.

Create an attendance record
- **create_employee**: Create a new employee
- **create_person**: Create a new person (v2 API)
- **create_webhook**: Create a new webhook (v2)
- **delete_absence**: Delete an absence record
- **delete_attendance**: Delete an attendance record
- **delete_webhook**: Delete a webhook (v2)
- **get_custom_report_columns**: Get columns for a custom report
- **get_custom_report_data**: Archived reports require manual refresh in UI.

Get data for a custom report
- **list_absences**: List employee absences
- **list_applications**: List recruiting applications (v2 Beta)
- **list_attendances**: List employee attendances
- **list_candidates**: List recruiting candidates (v2 Beta)
- **list_custom_attributes**: List custom attributes for employees
- **list_custom_reports**: List custom reports
- **list_employees**: Note: Specific attributes must be whitelisted in the Personio Wizard.

List company employees
- **list_jobs**: List recruiting jobs (v2 Beta)
- **list_persons**: List persons (v2 API)
- **list_webhooks**: List configured webhooks (v2)
- **update_attendance**: Update an attendance record
- **update_employee**: Update an existing employee
- **update_person**: Update an existing person (v2 API)
- **update_webhook**: Update an existing webhook (v2)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Personio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active employees in the Engineering department."

**🤖 AI Agent:**
> I've retrieved the employee list. There are 12 active employees in Engineering, including Sarah Chen (Lead Developer) and Marco Rossi (DevOps). Would you like to see their contact details?

---

**👤 You:**
> "Create an attendance record for employee ID 456 for today from 09:00 to 18:00."

**🤖 AI Agent:**
> Attendance record created successfully for employee 456 on 2023-10-27 (09:00 - 18:00).

---

**👤 You:**
> "Show me the data from my custom report 'Monthly Payroll Export'."

**🤖 AI Agent:**
> Fetching report data... I've loaded the 'Monthly Payroll Export'. It contains 50 rows of data across columns like 'Base Salary', 'Bonus', and 'Department'. Should I summarize the totals for you?


## Installation & Usage

To install and use the **Personio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/personio-alternative](https://vinkius.com/mcp/personio-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
