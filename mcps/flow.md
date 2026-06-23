# Flow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage projects, tasks, and team collaboration via AI agents with Flow (getflow.com).

## Description
Connect your **Flow** account to any AI agent and automate your project management and team collaboration through the Model Context Protocol (MCP). Flow (getflow.com) provides a clean and powerful platform for organizing work, tracking task progress, and facilitating team discussions. Now, you can manage your workspaces, projects, and individual tasks directly through natural conversation.

### What you can do

- **Project Coordination** — List all projects within your workspaces and retrieve detailed metadata, including ownership and due dates.
- **Task Management** — Create, update, and list tasks across workspaces, projects, or specific task lists. Change statuses (incomplete/completed) instantly.
- **Organized Lists** — Access and list task groups (Lists) within projects to maintain a clear hierarchy of work.
- **Team Interaction** — List all workspace members and teams, and participate in task discussions by reading or adding comments.
- **Workspace Oversight** — Get a high-level view of all the top-level workspaces you belong to.
- **Real-time Updates** — Fetch specific task details or metadata to keep your team informed and your projects on track.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Flow Personal Access Token (found in Account Settings > Apps & Developers)
3. Start managing your projects and tasks from Claude, Cursor, or any MCP client

### Who is this for?

- **Project Managers** — quickly check task statuses or update project timelines while coordinating with team leads.
- **Software Teams** — automate the retrieval of task comments and metadata directly from your development environment.
- **Marketing Agencies** — manage client projects and task lists through simple AI commands to stay organized and productive.


## Available Tools (12)
- **add_task_comment**: Post a comment
- **create_task**: Create a new task
- **get_project**: Get project details
- **get_task**: Get task details
- **list_task_lists**: List lists in project
- **list_workspace_members**: List team members
- **list_projects**: List projects in workspace
- **list_task_comments**: List task discussions
- **list_tasks**: List tasks
- **list_workspace_teams**: List workspace teams
- **list_workspaces**: List top-level workspaces
- **update_task**: ).

Update an existing task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Flow projects in the 'Marketing' workspace."

**🤖 AI Agent:**
> Fetching projects... I found 4 projects in your 'Marketing' workspace, including 'Q4 Campaign' and 'Brand Guidelines'. Would you like to see the task lists for any of these?

---

**👤 You:**
> "Create a new task: 'Review final design mockup' in the 'Design' list."

**🤖 AI Agent:**
> Task created! I've added 'Review final design mockup' to your 'Design' task list. The task ID is 'task_123'. Would you like to assign it to someone or set a due date?

---

**👤 You:**
> "Add a comment to task 'task_123': 'Design looks great, proceed to coding'."

**🤖 AI Agent:**
> Comment added! Your feedback has been successfully posted to task 'task_123'. The team will see your update in the task discussion timeline.


## ❓ FAQ

**Q: How do I find the Workspace ID for my Flow account?**
You can use the 'list_workspaces' tool. The agent will retrieve all workspaces you have access to and return their names and unique IDs, which you can then use for other operations.

**Q: Can I mark a task as completed using the agent?**
Yes! Use the 'update_task' tool, provide the Task ID, and set the 'status' parameter to 'completed'. The task will be immediately updated in Flow.

**Q: How do I see the discussion history for a task?**
Use the 'list_task_comments' tool and provide the Task ID. The agent will retrieve all messages and replies associated with that task, allowing you to catch up on the discussion.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flow](https://vinkius.com/mcp/flow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flow": {
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
