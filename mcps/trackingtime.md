# TrackingTime MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/trackingtime)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track how your team spends time across projects and clients with timesheets, reports, and budgeting tools that keep work profitable.

## Description
Connect your **TrackingTime** account to any AI agent and simplify how you manage your productivity, project tasks, and billable hours through natural conversation.

### What you can do

- **Live Tracking** — Start and stop timers for specific tasks instantly via AI commands to track your real-time activity.
- **Task Management** — Create, list, and update tasks, and organize them into specific projects for better workflow.
- **Time Logging** — Retrieve detailed logs of your time entries for any date range and manually add missing blocks of time.
- **Project & Client Oversight** — List all projects and customers to manage your business directory and assignments.
- **Team Coordination** — Query workspace users to understand team structure and member availability.
- **Account Visibility** — Fetch your user profile and verify account configurations directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your TrackingTime Email and Password
3. Start managing your time and productivity from Claude, Cursor, or any MCP client

### Who is this for?

- **Freelancers & Consultants** — quickly start timers and log billable hours via simple AI commands.
- **Project Managers** — monitor task progress and project logs across the team directly from the workspace.
- **Productivity Junkies** — keep an organized record of daily activities and time spent on specific projects via the AI assistant.


## Available Tools
- **add_time_entry**: Manual time entry
- **create_project**: Add new project
- **create_task**: Add new task
- **get_user_profile**: Get current user
- **list_customers**: List project clients
- **list_time_entries**: Get time logs
- **list_projects**: List your projects
- **list_tasks**: List your tasks
- **list_workspace_users**: List team members
- **start_timer**: Start tracking time
- **stop_timer**: Stop tracking time
- **update_task**: Modify task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TrackingTime** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Start my timer for the 'Design Review' task."

**🤖 AI Agent:**
> Timer started! I've initiated the tracking for 'Design Review' (ID: task_10293). I'll keep the clock running until you tell me to stop.

---

**👤 You:**
> "Show me all active tasks in the 'Marketing' project."

**🤖 AI Agent:**
> I've retrieved the tasks. There are 4 active items in 'Marketing': 'Social Media Posts', 'Email Campaign Setup', 'Blog Draft v1', and 'SEO Audit'. Which one would you like to start a timer for?

---

**👤 You:**
> "What are my time logs for today?"

**🤖 AI Agent:**
> Checking today's entries... You've tracked a total of 5.5 hours today: 2h on 'Backend API', 1.5h on 'Team Sync', and 2h on 'Documentation'. Great progress!


## ❓ FAQ

**Q: Can I start a timer for a specific task using the AI?**
Yes! Use the `start_timer` tool and provide the Task ID. Your agent will instantly begin tracking time for that specific activity in your workspace.

**Q: How do I see my time logs for the last 7 days?**
Run the `list_time_entries` query. Provide the `fromDate` and `toDate` in YYYY-MM-DD format to retrieve the full history of tracked blocks for that period.

**Q: Is it possible to add a time entry manually via AI?**
Absolutely. Use the `add_time_entry` action. Provide the start time, end time, and the associated Task ID to register a completed block of time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/trackingtime](https://vinkius.com/mcp/trackingtime)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TrackingTime** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `trackingtime` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TrackingTime** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "trackingtime": {
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
