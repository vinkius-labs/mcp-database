# Lucca (HR & Finance Suite) MCP Server

Manage your HRIS via Lucca — track employee data, leave requests (Timmi), and expense reports (Cleemy).

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/lucca-hr-finance-suite)

## Overview
**Category:** human-resources
**Tools Count:** 8

## Description
Connect your **Lucca** instance to any AI agent and take full control of your HR and administrative management through natural conversation.

### What you can do

- **Employee Orchestration** — List all employees in your HR directory and retrieve detailed profiles including job titles, managers, and hire dates directly from your agent
- **Leave & Absence (Timmi)** — Monitor active leave requests and retrieve precise vacation balances for specific users to manage team availability effectively
- **Expense Management (Cleemy)** — Audit company expense reports and list individual claims to monitor spending, status, and currency distributions securely
- **Timesheet Monitoring** — Extract detailed timesheet chunks within specific date boundaries to understand team work allocations and project logs
- **Organizational Audit** — Enumerate hierarchical company departments and sub-units to map your organization's structural boundaries natively
- **Diagnostic Investigation** — Deep-dive into specific employee UUIDs to retrieve exact metadata mappings required for rapid HR audits and reporting

### How it works

1. Subscribe to this server
2. Enter your Lucca Subdomain and API Key
3. Start managing your HRIS from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Managers** — audit employee directories and monitor leave requests through natural conversation without manually navigating the HRIS
- **Finance Teams** — track expense reports and individual claims from Cleemy to ensure financial policy compliance across the organization
- **Team Leads** — monitor team availability and timesheet logs to optimize project planning and workload distribution efficiently


## Available Tools
- **list_users**: List all employees in the Lucca HR directory
- **get_user**: Get detailed data mapping a target explicit employee UUID
- **list_departments**: List all departments inside the enterprise company
- **list_leaves**: List explicitly requested leaves mapping the Timmi Absences application limits
- **list_expense_reports**: List explicit company expense reports extracting Cleemy mapped targets
- **list_expense_claims**: List absolute bounded individual expense claims across a specific mapped report
- **list_timesheets**: List explicit matching timesheet chunks mapped in Timmi arrays limits
- **get_leave_balances**: Pull active strictly bound leave balances representing vacation arrays globally


## Installation & Usage

To install and use the **Lucca (HR & Finance Suite)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lucca-hr-finance-suite](https://vinkius.com/mcp/lucca-hr-finance-suite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
