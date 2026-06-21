# BugHerd MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bugherd)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage visual feedback and bug reports via BugHerd — track projects, tasks, and users directly from any AI agent.

## Description
Connect your **BugHerd** account to any AI agent and orchestrate your visual feedback, website bug tracking, and QA workflows through natural conversation.

### What you can do

- **Project Oversight** — List all your active projects and retrieve detailed metadata, including development URLs.
- **Task & Bug Management** — List all tasks in a project, retrieve detailed descriptions, and update statuses or priorities.
- **Feedback Processing** — Access the dedicated feedback queue to triage new reports from your clients or team.
- **User Coordination** — Access your directory of organization users and manage their involvement in projects.
- **Task Creation** — Create new tasks or feedback reports directly from your workspace with descriptions and priority levels.
- **Organizational Insights** — Retrieve core organization information and settings straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your BugHerd API Key
3. Start managing your visual feedback from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web Developers & QA** — quickly check task statuses or retrieve feedback details without manual portal logins.
- **Project Managers** — triage new bugs and update priorities straight from their workflow tools.
- **Designers** — monitor visual feedback and client requests using natural language.


## Available Tools
- **create_project**: Create a new BugHerd project
- **create_task**: Create a new task or feedback in a project
- **get_organization_info**: Retrieve core organization settings
- **get_project**: Get details of a specific project
- **get_task**: Get details of a specific task
- **list_feedback**: List tasks specifically in the Feedback queue
- **list_projects**: List all BugHerd projects
- **list_tasks**: List all tasks in a project
- **list_users**: List all users in the organization
- **update_task**: Update an existing task status or details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BugHerd** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active projects in BugHerd."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active projects: 'Vinkius Redesign' (ID: proj_1), 'Client Portal' (ID: proj_2), and 'Marketing Blog' (ID: proj_3).

---

**👤 You:**
> "Show the new feedback for the 'Vinkius Redesign' project."

**🤖 AI Agent:**
> Retrieving feedback... There are 5 items in the queue, including 'Header alignment issue on mobile' and 'Button color doesn't match spec'. Which one would you like to address?

---

**👤 You:**
> "Update task task_123 in project proj_456 to status 'Doing'."

**🤖 AI Agent:**
> Task task_123 has been successfully updated to 'Doing' in the 'Vinkius Redesign' project.


## ❓ FAQ

**Q: Can I update the status of a bug using the agent?**
Yes! Use the `update_task` tool with the Project ID and Task ID. You can change the `status` (e.g., 'To Do', 'Doing', 'Done') or `priority` directly from your workspace.

**Q: How do I see the feedback queue for a specific project?**
Simply ask the agent to `list_feedback` and provide the Project ID. It will retrieve all the tasks currently in the Feedback column, allowing you to triage them using natural language.

**Q: Does the integration allow creating a new project?**
Yes. Use the `create_project` action and provide the project name and optionally a development URL. The project will be created in your BugHerd organization instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bugherd](https://vinkius.com/mcp/bugherd)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BugHerd** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bugherd` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BugHerd** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bugherd": {
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
