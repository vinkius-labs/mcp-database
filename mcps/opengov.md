# OpenGov MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opengov)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/opengov-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/opengov-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Access OpenGov data directly—list reports, query financial funds, and manage users or departments through your AI agent.

## Description
Connect your **OpenGov** account to any AI agent to streamline public sector data management and financial reporting through natural conversation.

### What you can do

- **Reporting & Data** — List available reports, fetch detailed data rows (JSON/CSV), and inspect metadata schemas for precise analysis
- **User Management** — List, create, and update user profiles, roles, and statuses directly from your agent
- **Organizational Structure** — Manage departments and financial funds to track budgetary allocations and institutional hierarchy
- **Resource Inspection** — Fetch specific details for users or funds using unique identifiers

### How it works

1. Subscribe to this server
2. Enter your OpenGov API Key
3. Start querying public sector data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Public Officials** — instantly retrieve budget reports and fund statuses without manual portal navigation
- **Data Analysts** — fetch report schemas and data rows directly into your analysis environment
- **IT Administrators** — manage platform users and departmental structures via simple commands


## Available Tools
- **create_department**: Create a new OpenGov department
- **create_user**: Create a new OpenGov user
- **get_fund**: Get details for a specific OpenGov fund
- **get_report_data**: Get data rows for a specific report
- **get_report_metadata**: Get metadata and schema for a specific report
- **get_user**: Get details for a specific OpenGov user
- **list_departments**: List OpenGov departments
- **list_funds**: List OpenGov funds
- **list_reports**: List available OpenGov reports
- **list_users**: List OpenGov users
- **update_user**: Update an existing OpenGov user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenGov** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all the reports I have access to in OpenGov."

**🤖 AI Agent:**
> I've retrieved the list of reports. You have access to 'Annual Budget 2024', 'Departmental Expenses', and 'Grant Tracking'. Which one would you like to explore?

---

**👤 You:**
> "Get the data for report ID 'rep-123' in CSV format."

**🤖 AI Agent:**
> Fetching data for report 'rep-123' in CSV format... I've processed the rows. Would you like me to summarize the financial highlights or provide the raw output?

---

**👤 You:**
> "Create a new user with email 'admin@city.gov' as an Admin."

**🤖 AI Agent:**
> I've created the user 'admin@city.gov' with the Admin role. They should now appear in your user list and have access to the platform.


## Installation & Usage

To install and use the **OpenGov** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opengov](https://vinkius.com/mcp/opengov)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
