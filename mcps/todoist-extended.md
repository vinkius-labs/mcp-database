# Todoist MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/todoist-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Organize your personal and team tasks with the productivity app that millions trust to stay on top of everything that matters.

## Description
Connect your **Todoist** account to any AI agent and simplify how you organize your life and work through natural conversation.

### What you can do

- **Task Control** — Create, update, and complete tasks with full support for due dates, priorities, and descriptions.
- **Project Oversight** — List all your projects and manage sections to keep your workflows structured.
- **Smart Filtering** — Query your tasks using Todoist's powerful filter syntax (e.g., 'today', 'p1') via AI.
- **Categorization** — List and manage labels to tag your tasks across different projects.
- **Collaboration** — List comments on tasks and projects to track discussions and notes.
- **Workspace Maintenance** — Reopen completed tasks or fetch detailed metadata for specific to-do items.

### How it works

1. Subscribe to this server
2. Enter your Todoist API Personal Access Token (found in your developer settings)
3. Start managing your to-do list from Claude, Cursor, or any MCP client

### Who is this for?

- **Busy Professionals** — quickly add tasks and check your daily schedule via simple AI commands.
- **Project Managers** — monitor project progress and verify task statuses across different boards directly from the workspace.
- **Organized Individuals** — keep your life in sync by letting your AI assistant help you prioritize what truly matters.


## Available Tools (12)
- **complete_task**: Mark a task as finished
- **create_project**: Create a new project
- **create_task**: Add a new to-do item
- **get_project_details**: Get metadata for a project
- **get_task_details**: Get details for a specific task
- **list_comments**: List comments for a task or project
- **list_all_labels**: List your personal labels
- **list_projects**: List your Todoist projects
- **list_project_sections**: List sections within a project
- **list_active_tasks**: Can filter by project, label, or filter.

List active tasks
- **reopen_task**: Mark a closed task as active
- **update_task_details**: Modify an existing task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Todoist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are my high priority tasks for today?"

**🤖 AI Agent:**
> I've checked your active tasks. You have 2 high priority items (P1) for today: 'Finalize presentation' and 'Call client about API update'. Would you like to mark either as complete?

---

**👤 You:**
> "Create a task in the 'Work' project: 'Submit expense report' due Friday at 5pm."

**🤖 AI Agent:**
> Success! The task 'Submit expense report' has been added to your 'Work' project (ID: 10293) and is scheduled for this Friday at 5:00 PM.

---

**👤 You:**
> "Show me all active tasks with the label '@errand'."

**🤖 AI Agent:**
> I've fetched the tasks. You have 3 active items with the '@errand' label: 'Buy groceries', 'Post office', and 'Pick up dry cleaning'. Shall I retrieve the details for the post office task?


## ❓ FAQ

**Q: Can I filter tasks for today using the AI?**
Yes! Use the `list_active_tasks` tool and provide the `filter` parameter set to 'today'. Your agent will retrieve all tasks scheduled for the current date.

**Q: How do I add a new task to a specific project?**
Use the `create_task` tool. Provide the content and the unique Project ID. You can also include a `due_string` like 'tomorrow at 10am' to set a deadline.

**Q: Is it possible to list all my labels via AI?**
Absolutely. Run the `list_all_labels` query. The agent will retrieve the complete directory of labels you use to categorize tasks in your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/todoist-extended](https://vinkius.com/mcp/todoist-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Todoist** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `todoist-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Todoist** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "todoist-extended": {
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
