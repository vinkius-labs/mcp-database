# Height (Project Management) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/height-project-management)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage projects and tasks via Height — track activities, list tasks, and manage workspace lists.

## Description
Connect your **Height** workspace to any AI agent and take full control of your project management workflow through natural conversation.

### What you can do

- **Task Management** — List, retrieve, and inspect tasks with their full metadata and structural details directly from your agent
- **Lists & Grouping** — Discover and manage high-level grouping constructs and lists to organize your workspace effectively
- **Workspace Audit** — Extract explicit workspace domains and user credentials linked to your account for quick audits
- **Activity Tracking** — Access full audit trails and activity logs for any task to monitor its history and state mutations
- **Team Collaboration** — Fetch and map registered teammates and user identities across the organization securely

### How it works

1. Subscribe to this server
2. Enter your Height API Key
3. Start managing your tasks and projects from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — audit task history and generate rapid status reports through natural conversation
- **Developers** — list and retrieve task details without leaving your IDE or switching context to the web UI
- **Operations Teams** — track workspace activities and monitor team member assignments and roles


## Available Tools (6)
- **list_users**: List users
- **list_activities**: List activities
- **workspace**: Get workspace
- **list_tasks**: List tasks
- **get_task**: Get task
- **list_lists**: List lists


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Height (Project Management)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all tasks in my 'Product Roadmap' list"

**🤖 AI Agent:**
> I've found 8 tasks in the 'Product Roadmap' list. Highlights include 'API V2 Release' (T-102), 'User Onboarding Flow' (T-105), and 'Security Audit' (T-108). Would you like the details for any of these?

---

**👤 You:**
> "Show me the recent activity for task T-102"

**🤖 AI Agent:**
> Recent activity for T-102 ('API V2 Release'): Status changed from 'In Progress' to 'Review' by Alex. Sarah added a comment: 'Endpoint documentation is complete'. Would you like to see earlier history?

---

**👤 You:**
> "What are the details for task T-108?"

**🤖 AI Agent:**
> Task T-108 ('Security Audit'): Assigned to Mark, Priority: High, Due Date: Next Friday. Description: 'Complete the quarterly security audit for the core infrastructure'. Current status: 'Blocked'.


## ❓ FAQ

**Q: Can I see the full history of a task through my agent?**
Yes. Use the `list_activities` tool with a specific Task ID to retrieve the full audit trail, including state changes and comments, ensuring you never miss the context of a task's evolution.

**Q: How do I find a specific task ID?**
You can use `list_tasks` to browse tasks within a workspace or list. Your agent will display the Task IDs along with their names, making it easy to identify the exact task you need to inspect.

**Q: Can I list all members of my workspace?**
Absolutely. The `list_users` tool allows you to fetch all registered teammates in your Height workspace, helping you map assignments and identify collaborators in your projects.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/height-project-management](https://vinkius.com/mcp/height-project-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Height (Project Management)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `height-project-management` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Height (Project Management)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "height-project-management": {
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
