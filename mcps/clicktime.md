# ClickTime MCP Server

Manage time tracking and resource planning via ClickTime — track entries, monitor projects, and audit client hours directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/clicktime)

## Overview
**Category:** productivity
**Tools Count:** 8

## Description
Connect your **ClickTime** account to any AI agent and take full control of your time tracking and resource management through natural conversation. Streamline how you monitor billable hours and project progress natively.

### What you can do

- **Time Oversight** — List and retrieve details for all time entries including hours and descriptions natively
- **Project Intelligence** — Access and monitor all projects and clients configured in your account flawlessly
- **Resource Management** — List all users and people in the company to understand team allocation securely
- **Task Logistics** — Access work types and tasks available for time tracking to ensure accurate data entry flawlessly
- **Reporting Deep-Dives** — Retrieve high-volume time reports and daily completeness summaries flawlessly
- **User Visibility** — Access your own profile and API authentication details directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your ClickTime API Token (obtainable via the /Me endpoint with your credentials)
3. Start managing your time tracking from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — monitor project hours and billable time using natural language
- **Accountants** — audit time entry completeness and user rosters without opening the dashboard
- **Operations Teams** — quickly look up client IDs and task types straight from their chat interface
- **Individual Contributors** — verify their own time entries and profile information


## Available Tools
- **get_my_clicktime_profile**: Retrieve information about the currently authenticated user
- **get_high_volume_time_report**: Retrieve a high-volume report of time entries (up to 2500 records)
- **list_clicktime_clients**: List all clients configured in ClickTime
- **list_clicktime_jobs**: List all jobs (active and inactive) in the system
- **list_clicktime_projects**: List all projects configured in ClickTime
- **list_clicktime_tasks**: List all tasks (work types) available for time tracking
- **list_time_entries**: List time tracking entries
- **list_clicktime_users**: List all people and users in the company


## Installation & Usage

To install and use the **ClickTime** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clicktime](https://vinkius.com/mcp/clicktime)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
