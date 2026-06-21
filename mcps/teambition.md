# Teambition MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/teambition)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Collaborative project management platform by Alibaba — manage tasks, projects, and team workflows via AI.

## Description
Empower your AI agent to orchestrate your team's productivity with **Teambition**, the leading collaboration platform under Alibaba Group. By connecting Teambition to your agent, you transform complex project tracking and task assignment into a natural conversation. Your agent can instantly list your projects, create new tasks, update statuses, and even browse organization members without you ever touching the web interface. Whether you are managing a software development sprint or a marketing campaign, your agent acts as a real-time project assistant, keeping your workspace organized and your team aligned.

### What you can do

- **Project Management** — List all accessible projects, get detailed info, and monitor overall progress.
- **Task Operations** — Create, update, and track tasks with full support for descriptions, assignees, and due dates.
- **Workflow Visualization** — Browse task groups and stages to understand your Kanban or list-based workflows.
- **Team Coordination** — List project members and organization users to manage assignments effectively.
- **Organization Insights** — Retrieve high-level information about your Teambition organization structure.

### How it works

1. Subscribe to this server
2. Enter your Teambition App ID and App Secret
3. Start managing your projects through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — track development progress, audit task statuses, and align team members through natural language.
- **Software Developers** — manage your assigned tasks and update project progress directly from your AI-powered workspace.
- **Operations Teams** — oversee multiple project workflows and organizational structures through a unified AI interface.
- **Enterprise Leaders** — get real-time insights into organization-wide project activity and team member coordination.


## Available Tools (10)
- **create_task**: Create a new Teambition task
- **get_org_info**: Get organization details
- **get_project**: Get Teambition project details
- **list_members**: List project members
- **list_projects**: List all Teambition projects
- **list_stages**: List stages in a task group
- **list_task_groups**: List task groups in a project
- **list_tasks**: List tasks in a project
- **list_users**: List organization users
- **update_task**: Update an existing Teambition task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Teambition** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active projects on Teambition."

**🤖 AI Agent:**
> I've retrieved your Teambition projects. You have 4 active projects, including 'Website Redesign' and 'Q2 Marketing Plan'. Which one would you like to explore?

---

**👤 You:**
> "Create a task in project 'Product Launch' titled 'Review landing page copy'."

**🤖 AI Agent:**
> Done! I've created the task 'Review landing page copy' in the 'Product Launch' project. Would you like to assign it to someone or set a due date?

---

**👤 You:**
> "Show me the tasks for project 'Internal Audit'."

**🤖 AI Agent:**
> I've listed the tasks for 'Internal Audit'. There are 8 pending tasks, including 'Inventory check' and 'Compliance review'. Should I filter them by status or assignee?


## ❓ FAQ

**Q: How do I find my Teambition App ID and Secret?**
Log in to the [Teambition Open Platform](https://open.teambition.com/), navigate to the 'Developer Center', and create a new application. Your App ID and App Secret will be generated there.

**Q: Can I assign tasks to specific team members?**
Yes. When using `create_task` or `update_task`, you can provide an `executorId` to assign the task to a specific user. You can find user IDs using the `list_members` or `list_users` tools.

**Q: Does this server support Kanban stages?**
Yes. You can use `list_task_groups` to see your project's lists and `list_stages` to see the specific columns (stages) within those groups, allowing you to track exactly where a task is in the workflow.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/teambition](https://vinkius.com/mcp/teambition)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Teambition** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `teambition` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Teambition** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "teambition": {
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
