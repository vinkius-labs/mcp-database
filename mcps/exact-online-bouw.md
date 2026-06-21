# Exact Online Bouw MCP Server

Manage Dutch construction accounting with project budgets, cost tracking, and financial reporting built for the building industry.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/exact-online-bouw)

## Overview
**Category:** erp-operations
**Tools Count:** 12

## Description
Connect your **Exact Online Bouw** account to any AI agent and take full control of your construction projects and time tracking workflows through natural conversation.

### What you can do

- **Project Orchestration** — List and manage construction projects programmatically, including creating new entries with account and date metadata
- **Time Tracking Automation** — Register and monitor employee hours for specific projects to maintain a high-fidelity record of labor costs
- **Financial Intelligence** — Programmatically track project costs and expenses to monitor budget utilization and financial health in real-time
- **Structure Visualization** — Access and retrieve Work Breakdown Structures (WBS) to understand project deliverables and activities structured hierarchically
- **Account & Employee Visibility** — Retrieve complete directories of accounts and employees to ensure precise data association for all project entries

### How it works

1. Subscribe to this server
2. Retrieve your **Access Token**, **Division ID**, and **Region** from the Exact Online App Center
3. Start managing your construction projects and hours from Claude, Cursor, or any MCP client

No more manual logging of site hours or complex navigation through ERP tables. Your AI acts as your dedicated construction project and cost coordinator.

### Who is this for?

- **Project Managers** — instantly check project progress and register site hours using natural language commands
- **Finance Teams** — monitor project-specific costs and budget status without leaving your workspace
- **Site Supervisors** — quickly verify employee assignments and project structures through simple AI queries


## Available Tools
- **create_cost_transaction**: Requires project ID, item, date, and amount.

Register a cost or expense for a project
- **create_project**: You can also associate it with an account.

Create a new project in Exact Online
- **create_time_transaction**: Requires project ID, employee ID, item/activity, date, and number of hours.

Register hours (time entry) for a project
- **get_me**: Get current authenticated user and division information
- **get_project**: Get detailed information about a specific project
- **list_accounts**: List accounts (CRM) from Exact Online
- **list_cost_transactions**: List cost transactions registered in Exact Online
- **list_employees**: List employees from Exact Online
- **list_project_hour_budgets**: List hour budgets for projects
- **list_project_wbs**: List the Work Breakdown Structure (WBS) for projects
- **list_projects**: List all projects in Exact Online
- **list_time_transactions**: List time transactions (hours) registered in Exact Online


## Installation & Usage

To install and use the **Exact Online Bouw** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/exact-online-bouw](https://vinkius.com/mcp/exact-online-bouw)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
