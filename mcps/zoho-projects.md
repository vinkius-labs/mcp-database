# Zoho Projects MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-projects)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage projects, tasks, and milestones via the Zoho Projects V3 API.

## Description
Connect your **Zoho Projects** account to any AI agent to streamline your project management and team collaboration. This MCP server enables your agent to interact with portals, projects, and tasks directly through natural language interfaces using the latest V3 API.

### What you can do

- **Project Oversight** — List all projects within your portals and retrieve detailed configurations and metadata
- **Task Management** — List, retrieve, create, and update tasks across your projects with support for partial updates
- **Milestone Tracking** — Monitor project milestones and their associated target dates to stay on schedule
- **Team Visibility** — List all users and participants registered for a specific project to manage responsibilities
- **Organization Control** — List task lists and portals to maintain a clear picture of your entire project management hierarchy

### How it works

1. Subscribe to this server
2. Enter your Zoho Client ID, Client Secret, and Data Center Domain
3. Start managing your projects from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — Quickly update task statuses and monitor project health via natural language commands
- **Team Leads** — Move tasks through the pipeline and assign responsibilities without opening the dashboard
- **Developers** — Integrate project management data and task automation into your daily development workflow


## Available Tools
- **create_project**: Requires a portal ID and a project name.

Create a new project in a portal
- **create_task**: Requires portal ID, project ID, and task name.

Create a new task in a project
- **list_milestones**: List all milestones in a project
- **list_portals**: Use this to identify the portal ID for subsequent project and task calls.

List all Zoho Projects portals
- **list_projects**: List all projects in a portal
- **list_task_lists**: List all task lists in a project
- **list_tasks**: List all tasks in a project
- **update_task**: Update an existing task
- **list_project_users**: List all users associated with a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho Projects** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all portals in my Zoho Projects account."

**🤖 AI Agent:**
> I've retrieved your portals. You have 2 portals: 'Main Business Portal' (ID: 123456) and 'Client Collaborations' (ID: 789012). Which one would you like to access?

---

**👤 You:**
> "Show me the tasks for project ID '987654' in portal '123456'."

**🤖 AI Agent:**
> I found 10 tasks for project 987654. Notable ones include 'Design Final Approval', 'Frontend Implementation', and 'API Integration'. Would you like more details on any of them?

---

**👤 You:**
> "Update task ID '101' in project '987654' to 'Completed' status."

**🤖 AI Agent:**
> Successfully updated task 101. Its status has been set to 'Completed' in your Zoho project.


## ❓ FAQ

**Q: How do I find my Portal ID?**
Use the `list_portals` tool to retrieve all portals you have access to along with their unique IDs.

**Q: Which Data Center domains are supported?**
You can use any Zoho Data Center domain such as `zoho.com` (US), `zoho.eu` (Europe), `zoho.in` (India), `zoho.com.au` (Australia), or `zoho.jp` (Japan).

**Q: Can I update a task name without sending all other fields?**
Yes, the `update_task` tool uses the V3 PATCH method, allowing you to perform partial updates by only providing the fields you want to change.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-projects](https://vinkius.com/mcp/zoho-projects)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zoho Projects** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zoho-projects` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zoho Projects** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zoho-projects": {
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
