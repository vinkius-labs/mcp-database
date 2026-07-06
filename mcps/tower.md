# Tower MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tower)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Lightweight project management and team collaboration platform — manage tasks, projects, and discussions via AI.

## Description
Empower your AI agent to orchestrate your team's productivity with **Tower**, the lightweight and intuitive collaboration platform. By connecting Tower to your agent, you transform complex project tracking and task assignment into a natural conversation. Your agent can instantly list your projects, create new tasks, update statuses, and even browse project discussions without you ever needing to navigate the web interface. Whether you are managing a small creative project or a large-scale operation, your agent acts as a real-time team assistant, keeping your workspace organized and your team aligned.

### What you can do

- **Project Management** — List all accessible projects and retrieve detailed information about your collaboration workspace.
- **Task Operations** — Create, update, and track tasks with full support for descriptions, assignees, and completion status.
- **Team Coordination** — List teams and members to manage assignments and collaboration effectively.
- **Discussion Monitoring** — Browse project discussions and topics to stay informed about team updates.
- **Resource Organization** — List document folders within projects to access shared resources instantly.

### How it works

1. Subscribe to this server
2. Enter your Tower Access Token
3. Start managing your projects through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — track development progress, audit task statuses, and align team members through natural language.
- **Creative Teams** — manage assignments and monitor project discussions directly from your AI-powered workspace.
- **Operations Leads** — oversee multiple project workflows and team structures through a unified AI interface.
- **Knowledge Workers** — manage your personal tasks and team collaborations directly from your AI-powered assistant.


## Available Tools (10)
- **create_task**: Create a new Tower task
- **get_project**: Get project details
- **get_task_details**: Get task details
- **list_discussions**: List project discussions
- **list_tasks**: List tasks in a project
- **list_doc_folders**: List document folders
- **list_members**: List team members
- **list_projects**: List all Tower projects
- **list_teams**: List available teams
- **update_task**: Update an existing Tower task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tower** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active projects on Tower."

**🤖 AI Agent:**
> I've retrieved your Tower projects. You have 3 active projects: 'Design Refresh', 'API Integration', and 'Content Calendar'. Which one would you like to explore?

---

**👤 You:**
> "Create a task in project 'Design Refresh' titled 'Select primary color palette'."

**🤖 AI Agent:**
> Done! I've created the task 'Select primary color palette' in the 'Design Refresh' project. Would you like to assign it to someone?

---

**👤 You:**
> "Show me recent discussions in the 'API Integration' project."

**🤖 AI Agent:**
> I've found 4 recent discussions in 'API Integration', including 'Authentication Flow' and 'Endpoint Mapping'. Would you like to see the details of any of these topics?


## ❓ FAQ

**Q: How do I obtain a Tower Access Token?**
Log in to your Tower account, go to the [App Center](https://tower.im/oauth/tokens), and generate a new Personal Access Token. Make sure to copy it immediately.

**Q: Can I see team discussions through this server?**
Yes. Use the `list_discussions` tool with a project ID to retrieve the list of recent topics and discussions shared within that project.

**Q: Is it possible to manage multiple teams?**
Yes. You can use `list_teams` to see all teams you are a part of and then use the team IDs to list members or access specific projects associated with those teams.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tower](https://vinkius.com/mcp/tower)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tower** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tower` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tower** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tower": {
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
