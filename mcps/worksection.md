# Worksection MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/worksection)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Collaborative project management to manage tasks, projects, and timers with AI using Admin API v2.

## Description
Connect your **Worksection** account to any AI agent to automate your project management and team productivity workflows. Worksection provides a comprehensive set of tools for managing tasks, tracking time, and monitoring real-time project activities through natural conversation.

### What you can do

- **Project Lifecycle Management** — List all projects, create new ones, and manage tasks across your entire organization programmatically.
- **Time Tracking & Timers** — Monitor active timers for team members and stop time trackers directly from the AI interface.
- **Activity Monitoring** — Retrieve a detailed event log of recent account activities to stay updated on project changes and completions.
- **Stakeholder Collaboration** — Access task comments, project members, and attached files to maintain a clear overview of team collaboration.
- **Hierarchical Oversight** — Navigate project folders and task sub-trees using simple natural language commands.

### How it works

1. Subscribe to this server
2. Enter your Worksection Account Name (subdomain) and Administrative API Key
3. Start managing your projects from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — automate task status reports and monitor team timers without manual oversight.
- **Operations Leads** — track real-time activity across multiple projects and folders via natural conversation.
- **Distributed Teams** — streamline task coordination and ensure all project stakeholders are aligned programmatically.


## Available Tools (12)
- **complete_task**: Finish a task
- **create_task**: Add new task
- **get_project_details**: Get project info
- **get_task_details**: Get full task info
- **list_work_history**: Get event log
- **list_project_members**: List team on project
- **list_projects**: List workspace projects
- **list_project_tasks**: List tasks in project
- **list_active_timers**: Check running timers
- **list_all_users**: List company users
- **reopen_task**: Restore a task
- **stop_timer**: Finish time tracking


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Worksection** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active project folders in Worksection."

**🤖 AI Agent:**
> I've retrieved your projects. You have several active folders including 'Main Projects', 'Internal Tasks', and 'Client Work'. Which one would you like to explore?

---

**👤 You:**
> "Show me the last 10 events from my account activity log."

**🤖 AI Agent:**
> Fetching activity... Recent events include 'Task #123 completed by John', 'New comment on project Alpha', and 'Timer started by Sarah'.


## ❓ FAQ

**Q: How do I find my Worksection Administrative API Key?**
Log in to Worksection, navigate to **Account Settings** > **API**, and you will find your Administrative API Key listed there along with your account subdomain.

**Q: Can the AI stop active timers for team members?**
Yes! Use the `stop_timer` tool and provide the task identifier (page) to stop any active time tracking for that specific task in your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/worksection](https://vinkius.com/mcp/worksection)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Worksection** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `worksection` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Worksection** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "worksection": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
