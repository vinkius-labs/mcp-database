# AssessTEAM MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/assessteam)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/assessteam-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/assessteam-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Evaluate employee performance, run 360-degree reviews, and track team goals with streamlined assessment workflows.

## Description
Connect your **AssessTEAM** account to any AI agent and simplify how you manage employee evaluations, project timesheets, and organizational profitability through natural conversation.

### What you can do

- **Performance Management** — List and query employee evaluations and KPI assessments to track workforce development.
- **Timesheet Control** — Create and list time logs for project tracking to ensure accurate labor reporting.
- **Project Profitability** — Retrieve detailed financial reports and margin analysis for your active projects.
- **Team Directory** — List employees, teams, and organizational structures to manage your workforce hierarchy.
- **Project Oversight** — Monitor all current projects and their associated profitability metrics in real-time.
- **Compliance & Reporting** — Fetch history of recorded time logs and evaluations directly via AI commands.

### How it works

1. Subscribe to this server
2. Enter your AssessTEAM API Key (found in your account settings)
3. Start managing your human capital from Claude, Cursor, or any MCP client

### Who is this for?

- **HR Managers** — quickly retrieve performance reviews and monitor team evaluations via simple AI queries.
- **Operations Leads** — track project hours and verify labor costs directly from the workspace.
- **Business Owners** — get instant bird's-eye views of project profitability and employee productivity via the AI assistant.


## Available Tools
- **create_timesheet_entry**: Create a new timesheet entry
- **list_employees**: List team employees
- **list_performance_evaluations**: List performance evaluations
- **get_profitability_report**: Get project profitability report
- **list_projects**: List AssessTEAM projects
- **list_organizational_teams**: List organizational teams
- **list_timesheets**: List timesheet entries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AssessTEAM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects and their status."

**🤖 AI Agent:**
> I've retrieved your projects. You have 4 active initiatives including 'Website Redesign' (On track), 'Mobile App v2', and 'Client Audit'. Which one would you like profitability metrics for?

---

**👤 You:**
> "Log 8 hours for employee 'emp_1029' on project 'proj_8823' for today."

**🤖 AI Agent:**
> Time log created! I've added 8 hours to employee emp_1029's timesheet for project proj_8823 today. The entry has been recorded successfully in AssessTEAM.

---

**👤 You:**
> "Show me the latest performance evaluations."

**🤖 AI Agent:**
> I've fetched the evaluations. Over the last quarter, 15 reviews were completed. Average KPI score is 4.2/5.0. Shall I retrieve the detailed feedback for the 'Engineering' team?


## Installation & Usage

To install and use the **AssessTEAM** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/assessteam](https://vinkius.com/mcp/assessteam)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
