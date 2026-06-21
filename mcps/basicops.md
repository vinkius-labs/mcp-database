# BasicOps MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/basicops)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Centralize team communication with task management, document sharing, and project tracking designed for small business clarity.

## Description
Connect your **BasicOps** account to any AI agent and take full control of your project management and team collaboration workflows through natural conversation.

### What you can do

- **Project & Section Orchestration** — List and manage your entire project hierarchy programmatically, including creating new project sections (phases) in real-time
- **Task Lifecycle Management** — Programmatically create and update tasks, monitoring status transitions, due dates, and high-fidelity descriptions directly through your agent
- **Team Coordination Intelligence** — Access complete directories of team members and retrieve communication history within tasks to maintain perfectly coordinated context
- **Workflow Automation** — Programmatically manage project sections to organize your team's workflow into high-fidelity sprints or operational phases
- **Workspace Visibility** — Access high-fidelity metadata for your workspace and monitor active webhooks directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Personal Access Token** from your BasicOps settings (Settings > API)
3. Start managing your team's productivity from Claude, Cursor, or any MCP client

No more manual toggling between project tabs or missing task deadlines. Your AI acts as your dedicated project coordinator and task architect.

### Who is this for?

- **Project Managers** — instantly retrieve project summaries and update task statuses using natural language commands
- **Team Leads** — monitor team bandwidth and manage project sections without leaving your creative workspace
- **Operations Leads** — automate the oversight of workspace metadata and task distribution through simple AI queries


## Available Tools (12)
- **create_project**: Create a new project
- **create_task**: Create a new task
- **get_account_info**: Get my profile
- **get_project**: Get project details
- **get_task**: Get task details
- **list_task_messages**: List task messages
- **list_projects**: List all BasicOps projects
- **list_project_sections**: List project sections
- **list_project_tasks**: List tasks in project
- **list_team_users**: List team members
- **list_webhooks**: List active webhooks
- **update_task**: Update a task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BasicOps** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in my BasicOps workspace."

**🤖 AI Agent:**
> I've retrieved your projects. You currently have 3 active projects, including 'Marketing Launch' (ID: 123) and 'App Development'. Which one should we check for tasks?

---

**👤 You:**
> "Create a new high-priority task 'Fix Login Bug' in project '123'."

**🤖 AI Agent:**
> Task created! I've successfully registered 'Fix Login Bug' in project 123. It's now visible to your team with high priority. Need help assigning a specific member?

---

**👤 You:**
> "Show the communication history for task ID '456'."

**🤖 AI Agent:**
> Accessing task intelligence... I've retrieved 5 recent updates for task 456, including a technical note from @user1 and a status confirmation. Would you like the high-fidelity metadata for these messages?


## ❓ FAQ

**Q: How do I find my BasicOps Personal Access Token?**
Log in to your account, navigate to **Settings** > **API**, and generate a new Personal Access Token for your integration.

**Q: What is a Project Section via AI?**
Sections allow your agent to group related tasks into specific phases, sprints, or categories within a larger project programmatically.

**Q: How do I list team members programmatically?**
Use the `list_users` tool to retrieve your complete organizational directory including high-fidelity names and email addresses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/basicops](https://vinkius.com/mcp/basicops)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BasicOps** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `basicops` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BasicOps** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "basicops": {
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
