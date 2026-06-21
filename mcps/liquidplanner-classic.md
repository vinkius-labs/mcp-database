# LiquidPlanner Classic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/liquidplanner-classic)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Plan projects with intelligent scheduling that automatically adjusts timelines based on team capacity and task dependencies.

## Description
Connect your **LiquidPlanner Classic** workspace to any AI agent and manage project planning through natural conversation.

### What you can do

- **Task Management** — Create, update, and assign tasks with priority and estimates
- **Project Tracking** — Browse projects, milestones, and deliverables
- **Timeline Monitoring** — Track predictive schedules and deadline forecasts
- **Workspace Browsing** — Navigate workspace structure and team members
- **Time Tracking** — Access logged time and effort data

### How it works

1. Subscribe to this server
2. Enter your LiquidPlanner email, password, and Workspace ID
3. Start managing projects from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **PMs** — manage predictive project schedules
- **Teams** — track tasks and time entries
- **Executives** — monitor deadline forecasts and resource allocation


## Available Tools (10)
- **create_project**: Create a new project in the default workspace
- **create_task**: Requires parent_id if it should be nested under a project or folder.

Create a new task in the default workspace
- **get_project**: Get details of a specific project
- **get_task**: Get details of a specific task
- **get_workspace**: Uses the default configured workspace if no ID is provided.

Get details of a specific workspace or the default workspace
- **list_members**: List members in the default workspace
- **list_projects**: List projects in the default workspace
- **list_tasks**: List tasks in the default workspace
- **list_workspaces**: List workspaces from LiquidPlanner Classic
- **update_task**: Update an existing task in the default workspace


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LiquidPlanner Classic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all projects and the predicted schedule for the Platform v2 project."

**🤖 AI Agent:**
> Projects: 5. 'Platform v2' (78 tasks), 'Mobile App' (34), 'API Redesign' (22), 'Infrastructure' (15), 'Marketing Site' (12). Platform v2 schedule: Best case: Jun 12. Most likely: Jun 28. Worst case: Jul 15. Progress: 45%. On-time probability: 72%. Critical path: 'Auth Module' → 'API Gateway' → 'Load Testing'. ⚠️ 3 tasks at risk.

---

**👤 You:**
> "Create a task and show time tracking for the team this week."

**🤖 AI Agent:**
> Task created! 'Implement caching layer' — Best: 8h, Worst: 16h. Assigned: Sarah. Project: API Redesign. Predicted completion: May 2. Time tracking (this week): Team total: 142h. Sarah: 38h (95%), Mike: 35h (88%), Lisa: 32h (80%), James: 22h (55%), Others: 15h. Most time: 'Auth Module' (28h).

---

**👤 You:**
> "Show workspace members and resource allocation."

**🤖 AI Agent:**
> Workspace members: 8. Resource allocation: Sarah (95% ⚠️ overloaded, 3 projects). Mike (88%, 2 projects). Lisa (80%, 2 projects). James (55%, 1 project). Ana (70%, 2 projects). 3 others at 40-60%. Availability next week: James (40% free), Ana (30%), others fully allocated.


## ❓ FAQ

**Q: Can I manage tasks with predictive scheduling?**
Yes. Create tasks with best/worst case estimates. LiquidPlanner calculates predictive schedules and deadline probabilities automatically.

**Q: Does LiquidPlanner Classic require three credentials?**
Yes. Requires **Email**, **Password**, and **Workspace ID**. Uses **HTTP Basic Auth** (email:password) against `app.liquidplanner.com/api/workspaces/{id}`.

**Q: Can I track time entries?**
Yes. Access logged time entries per task and team member with effort hours and date ranges.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/liquidplanner-classic](https://vinkius.com/mcp/liquidplanner-classic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LiquidPlanner Classic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `liquidplanner-classic` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LiquidPlanner Classic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "liquidplanner-classic": {
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
