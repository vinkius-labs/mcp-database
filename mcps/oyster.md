# Oyster MCP Server

Manage global HR, payroll, and compliance via Oyster — list engagements, track expenses, and manage time-off requests directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/oyster)

## Overview
**Category:** human-resources
**Tools Count:** 15

## Description
Connect your **Oyster** account to any AI agent to streamline your global team management and HR operations through natural conversation.

### What you can do

- **Engagement Management** — List all active engagements and fetch detailed metadata for specific team members globally.
- **Expense Tracking** — Query existing expenses, filter by review states, and create new expense requests with receipt metadata.
- **Time Off Requests** — Monitor, retrieve, and create time-off requests (vacation, sick leave) for your entire distributed workforce.
- **Financial Insights** — Access and filter company invoices by payroll periods, statuses, or specific engagement IDs.
- **Global Expansion** — Retrieve lists of supported hiring countries and subdivisions to plan your next global hire.
- **Operation Monitoring** — Track the status of asynchronous operations and manage webhooks for real-time updates.

### How it works

1. Subscribe to this server
2. Enter your Oyster Personal Access Token
3. Start managing your global workforce from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Managers** — quickly check time-off balances and engagement details without navigating the Oyster dashboard.
- **Finance Teams** — audit expenses and invoices directly through conversational queries.
- **Operations Leads** — streamline the hiring process by checking country availability and creating draft employments.


## Available Tools
- **create_draft_employment**: This is an async operation.

Create a draft employment (Beta, Async)
- **create_expense**: This is an async operation, returns an operationKey.

Create a new expense (Async)
- **create_time_off_request**: Create a new time off request
- **create_webhook**: Create a new webhook endpoint
- **get_company**: Get company details
- **get_engagement**: Get details for a specific engagement
- **get_expense**: Get details for a specific expense
- **get_operation_status**: Get async operation status
- **get_time_off_request**: Get details for a specific time off request
- **list_engagements**: List Oyster engagements
- **list_expenses**: List expenses
- **list_hiring_countries**: List hiring countries (Beta)
- **list_invoices**: List invoices
- **list_subdivisions**: List subdivisions for a country (Beta)
- **list_time_off_requests**: List time off requests


## Installation & Usage

To install and use the **Oyster** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oyster](https://vinkius.com/mcp/oyster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
