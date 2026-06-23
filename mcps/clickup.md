# ClickUp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clickup)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage tasks and projects via ClickUp — track work, monitor spaces, and manage team productivity directly from any AI agent.

## Description
Connect your **ClickUp** account to any AI agent and take full control of your project management and productivity through natural conversation. Streamline how you manage tasks, subtasks, and complex workflows natively.

### What you can do

- **Workspace Oversight** — List and retrieve details for all workspaces (teams) you belong to natively
- **Hierarchy Intelligence** — Access and monitor spaces, folders, and lists to understand project structures flawlessly
- **Task Management** — List and retrieve detailed information for tasks, including statuses and priorities, securely
- **Workflow Logistics** — Create new tasks and manage subtasks to keep your team organized flawlessly
- **Productivity Tracking** — Access your own user profile and team member information securely
- **Integrated Visibility** — Retrieve detailed task metadata including descriptions and due dates directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your ClickUp Personal API Token (obtained from Settings > Apps)
3. Start managing your projects from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — monitor task progress and team capacity using natural language
- **Team Leads** — audit project hierarchies and task statuses without opening the complex dashboard
- **Developers** — quickly look up task details and create new to-dos straight from their chat interface
- **Ops Teams** — verify workspace configurations and monitor organizational productivity


## Available Tools (8)
- **create_new_task**: Create a new task in a specific list
- **get_my_clickup_profile**: Retrieve information about the authenticated user
- **get_task_details**: Get detailed information for a specific task
- **list_space_folders**: List all folders within a space
- **list_space_lists**: List all lists within a space
- **list_workspace_spaces**: List all spaces within a workspace
- **list_list_tasks**: List all tasks in a specific list
- **list_clickup_workspaces**: List all workspaces (teams) the user belongs to


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClickUp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my ClickUp workspaces."

**🤖 AI Agent:**
> Retrieving your ClickUp workspaces... I found 2: 'Product Team' (ID: 1234) and 'Marketing Dept' (ID: 5678). Which one would you like to see the spaces for?

---

**👤 You:**
> "Show me the tasks in the 'Q2 Launch' list."

**🤖 AI Agent:**
> Checking tasks in Q2 Launch... I found 5 items: 'Update Landing Page' (To Do), 'Finalize Copy' (In Progress), 'Security Audit' (Closed), and 2 others. Should I include subtasks?

---

**👤 You:**
> "Create a new task called 'Prepare presentation' in list 'wf_123'."

**🤖 AI Agent:**
> Creating task 'Prepare presentation'... The task has been successfully created in ClickUp. You can find it under the ID 'task_abc123'. Would you like to add a description or a due date?


## ❓ FAQ

**Q: Can I see the subtasks for a specific task?**
Yes! Use the `get_task_details` tool with the task ID. The agent will fetch the full task record, which includes all subtasks nested within it.

**Q: How do I find all the tasks in a specific list?**
Use the `list_list_tasks` tool. Provide the list ID, and your agent will return all tasks in that list, including their current statuses and priorities.

**Q: Where do I find my ClickUp API Token?**
Log in to ClickUp, go to your **Personal Settings**, select **Apps**, and generate a **Personal API Token** under the API section.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clickup](https://vinkius.com/mcp/clickup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ClickUp** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clickup` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ClickUp** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clickup": {
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
