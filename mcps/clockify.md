# Clockify MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clockify)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clockify-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clockify-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage time tracking and projects via Clockify — track entries, monitor projects, and audit team hours directly from any AI agent.

## Description
Connect your **Clockify** account to any AI agent and take full control of your time tracking and project management through natural conversation. Streamline how you monitor work hours and team productivity natively.

### What you can do

- **Workspace Oversight** — List and retrieve details for all workspaces you have access to natively
- **Project Intelligence** — Access and monitor all projects and clients configured in your account flawlessly
- **Time Tracking** — List and retrieve details for all time entries for any user in your team securely
- **Timer Management** — Start and stop timers directly from your chat interface to ensure accurate logging flawlessly
- **Team Logistics** — List all users and team members within a workspace to understand allocation securely
- **Productivity Auditing** — Retrieve detailed time entry metadata including descriptions and project associations flawlessly

### How it works

1. Subscribe to this server
2. Enter your Clockify API Key (found in Settings > My Profile)
3. Start managing your time tracking from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — monitor team hours and project progress using natural language
- **Freelancers** — quickly log time and verify billable hours without opening the dashboard
- **Operations Teams** — quickly look up project assignments and user rosters straight from their chat interface
- **HR Teams** — verify timesheet completeness and team member status


## Available Tools
- **add_new_time_entry**: Add a new time entry to a workspace
- **get_my_clockify_profile**: Retrieve information about the authenticated user
- **list_workspace_clients**: List all clients configured in a workspace
- **list_workspace_projects**: List all projects within a specific workspace
- **list_user_time_entries**: List time entries for a specific user in a workspace
- **list_workspace_users**: List all users within a specific workspace
- **list_clockify_workspaces**: List all workspaces the user has access to
- **stop_current_timer**: Stop the currently running timer for a specific user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clockify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Clockify workspaces."

**🤖 AI Agent:**
> Retrieving your Clockify workspaces... I found 2: 'Engineering Team' (ID: 1234) and 'Marketing Ops' (ID: 5678). Which one would you like to see projects for?

---

**👤 You:**
> "Show me the last 5 time entries for user 'John Doe'."

**🤖 AI Agent:**
> Checking time entries for John Doe... I found 5 items: 'Bug fixing' (2.0 hrs), 'API Integration' (4.5 hrs), 'Team Sync' (1.0 hr), and 2 others. All were logged against the 'Vinkius Cloud' project.

---

**👤 You:**
> "Stop my running timer in the 'Engineering' workspace."

**🤖 AI Agent:**
> Stopping your timer... The active timer for 'API Research' has been successfully stopped. It was logged for 1 hour and 15 minutes.


## Installation & Usage

To install and use the **Clockify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clockify](https://vinkius.com/mcp/clockify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
