# ClickUp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clickup-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Bring tasks, docs, goals, and team communication together in one workspace that replaces scattered project management tools.

## Description
Connect your **ClickUp** account to any AI agent and take full control of your project hierarchy and task management workflows through natural conversation.

### What you can do

- **Hierarchy Orchestration** — Navigate through your entire ClickUp structure, from Workspaces and Spaces to Folders and Lists programmatically
- **Task Lifecycle Management** — Create, update, and manage tasks in real-time, including monitoring status, priority, and detailed metadata directly through your agent
- **Deep Task Intelligence** — Retrieve complete task details, including descriptions, assigned users, and custom fields to maintain high-fidelity project records
- **Workflow Automation** — Programmatically list tasks within specific lists or filter folderless lists to understand your team's progress and individual workloads
- **Administrative Oversight** — List all accessible workspaces and team members to ensure perfectly coordinated collaboration and permission management

### How it works

1. Subscribe to this server
2. Retrieve your **Personal API Token** from the ClickUp dashboard (Settings > Apps)
3. Start managing your productivity pipeline from Claude, Cursor, or any MCP client

No more manual toggling between lists or digging through complex status folders. Your AI acts as your dedicated project coordinator and task architect.

### Who is this for?

- **Project Managers** — instantly retrieve task lists and update project statuses using natural language commands
- **Software Teams** — manage complex sprints and automate task assignment without leaving your creative workspace
- **Operations Leads** — monitor team capacity and orchestrate folder structures through simple AI queries


## Available Tools (10)
- **create_task**: Requires a task name. Optional status and description can be provided.

Create a new task in a List
- **delete_task**: Delete a specific task
- **get_task_details**: Note: Do not include the # prefix.

Get details for a specific task
- **list_folderless_lists**: List Lists not contained in a Folder
- **list_folders**: Folders help organize multiple lists.

List all Folders in a Space
- **list_lists**: Lists contain the actual tasks.

List all Lists in a Folder
- **list_spaces**: Spaces are large groupings of folders and lists.

List all Spaces in a Workspace
- **list_tasks**: Supports pagination to handle large numbers of tasks.

List tasks within a List
- **list_workspaces**: Workspaces are the top-level unit in ClickUp.

List all ClickUp Workspaces
- **update_task**: Can update the name, description, or status.

Update an existing task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClickUp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all ClickUp Workspaces I have access to."

**🤖 AI Agent:**
> I've retrieved your accessible workspaces. You currently belong to: 'Vinkius Global' (ID: 123) and 'Personal Tasks' (ID: 456). Which one should we explore for project spaces?

---

**👤 You:**
> "Show the tasks in list ID '789' and their current statuses."

**🤖 AI Agent:**
> Scanning list 789... I found 5 active tasks, including 'Redesign UI' (In Progress) and 'API Documentation' (To Do). Would you like the detailed metadata for the 'In Progress' task?

---

**👤 You:**
> "Create a high-priority task 'Fix Login Bug' in list '789'."

**🤖 AI Agent:**
> Action complete! I've created the high-priority task 'Fix Login Bug' in specified list (ID: 789). It's now visible on your dashboard for your team to address. Need help assigning a crew member?


## ❓ FAQ

**Q: How do I find my ClickUp Personal API Token?**
Log in to ClickUp, navigate to **Settings** > **Apps**, and click **Generate** under the Personal API Token section.

**Q: What is the difference between a Space and a List?**
A Space is a top-level grouping for high-level organization, while a List contains the actual individual tasks you want to track.

**Q: Can I filter for archived tasks?**
The current toolset is optimized for active project management and typically retrieves non-archived tasks to maintain workflow focus.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clickup-alternative](https://vinkius.com/mcp/clickup-alternative)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `clickup-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ClickUp** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clickup-alternative": {
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
