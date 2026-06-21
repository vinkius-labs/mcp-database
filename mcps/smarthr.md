# SmartHR MCP Server

Empower your AI to manage employee records, organizational structures, and payrolls directly from your SmartHR workspace.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/smarthr)

## Overview
**Category:** human-resources
**Tools Count:** 8

## Description
Connect your **SmartHR** directory to any AI agent and empower your team to query employee data, organizational hierarchies, and payroll records securely. Interact with your organization's human capital database through natural language without ever switching tabs.

### What you can do

- **Employee Tracking** — Call the `list_crews` tool to retrieve the roster of all employees and cross-reference demographic metadata
- **Department Hierarchies** — Ask your AI to `list_departments` or check `list_positions` to understand the internal structure
- **Deep Employee Profiles** — Perform targeted queries using `get_crew_details` or `list_crew_dependents` to fetch highly sensitive contract details
- **Payroll Overviews** — Securely query active or historical payroll ledgers to audit compensation scaling

### How it works

1. Subscribe to this server
2. Enter your SmartHR Access Token and Subdomain
3. Start using Claude, Cursor, or any MCP-compatible client to query your employee database

Stop clicking through countless profiles on the SmartHR platform just to find out someone's department or employment type. Your AI agent can read your internal database directly.

### Who is this for?

- **HR Managers & Admins** — easily audit payroll accounts or check an employee's listed dependents internally via chat
- **Department Leads** — request the agent to fetch a list of active job positions and associated team members
- **Security Teams** — check office locations and active employee sublists via the physical `list_establishments` tools


## Available Tools
- **list_crews**: Lists all employees (crews) in SmartHR
- **get_crew_details**: Retrieves details for a specific employee
- **list_departments**: Lists all organizational departments
- **list_positions**: Lists all job positions or roles
- **list_employment_types**: Lists all employment types
- **list_payrolls**: Lists employee payroll records
- **list_establishments**: Lists business establishments or office locations
- **list_crew_dependents**: Lists dependents for a specific employee


## Installation & Usage

To install and use the **SmartHR** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smarthr](https://vinkius.com/mcp/smarthr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
