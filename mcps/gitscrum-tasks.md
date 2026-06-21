# GitScrum Tasks MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gitscrum-tasks)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Master task execution via GitScrum — create, filter, assign, and track tasks with subtasks, checklists, and comments directly from any AI agent.

## Description
### What you can do

- **Full task lifecycle** — create, update, delete, and toggle completion on tasks with rich metadata including types, effort levels, and dates
- **Advanced filtering** — query tasks by status, sprint, user story, assignee, label, type, effort, workflow column, blocker flag, and date ranges
- **Subtask management** — list, link, unlink subtasks and discover related tasks across your project
- **Checklists** — add checklist items with sub-items and toggle completion for granular progress tracking
- **Team coordination** — assign and unassign members, duplicate tasks, move between projects, and set story points
- **Comments** — list, create, update, and delete task comments for rich collaboration context

### How it works

1. Subscribe to the GitScrum Tasks integration from the marketplace
2. Enter your GitScrum API token and company slug
3. Start managing tasks conversationally — ask your agent to create tasks, assign team members, or review today's workload in Claude, Cursor, or any MCP client

Your agent handles the complete task lifecycle so you never need to context-switch to the GitScrum UI.

### Who is this for?

- **Developers** — create and check off tasks without leaving the IDE
- **Scrum masters** — assign tasks, set estimates, and manage sprint backlogs via natural language
- **Product managers** — filter and review task progress across multiple dimensions instantly


## Available Tools
- **assign_member**: Assign a user to a task
- **create_checklist_item**: Use parent_id to create sub-items.

Add a checklist item to a task
- **list_checklists**: List checklists on a task
- **toggle_checklist_item**: Toggle a checklist item done/undone
- **create_comment**: Supports rich text content.

Add a comment to a task
- **delete_comment**: Delete a comment
- **list_comments**: Comments support rich text.

List comments on a task
- **update_comment**: Edit an existing comment
- **duplicate_task**: Duplicate a task
- **list_effort_levels**: List effort/priority levels
- **set_task_estimate**: Set story points / estimate for a task
- **move_task_to_project**: Move a task to a different project
- **my_tasks**: Get all tasks assigned to me
- **related_tasks**: Get tasks related to a task
- **link_subtask**: Link an existing task as a subtask
- **list_subtasks**: List subtasks of a task
- **unlink_subtask**: Unlink a subtask
- **get_task_by_code**: g., WEB-42) instead of UUID.

Get task by human-readable code
- **create_task**: Create a new task
- **delete_task**: This action cannot be undone.

Delete a task permanently
- **toggle_task_done**: Toggle task completion status
- **get_task**: Get task details by UUID
- **list_tasks**: Filter by status (todo, in-progress, done), sprint, user_story, users, labels, type, effort, workflow, is_blocker, is_archived, unassigned, created_at (YYYY-MM-DD=YYYY-MM-DD), closed_at, per_page.

List tasks with advanced filters
- **update_task**: Update an existing task
- **my_today_tasks**: Get tasks due today
- **create_task_type**: g., Chore, Tech Debt) with a hex color code.

Create a new task type
- **list_task_types**: ) with their colors.

List task types in a project
- **unassign_member**: Remove a user from a task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GitScrum Tasks** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all in-progress tasks in the web-app project."

**🤖 AI Agent:**
> Found 8 tasks in progress in web-app: 1) 'WEB-42: Implement auth flow' assigned to johndoe (Feature, High effort), 2) 'WEB-38: API rate limiting' assigned to janedoe (Improvement), 3) 'WEB-45: Dashboard redesign' unassigned... Would you like to assign the unassigned task or check subtasks for any of these?

---

**👤 You:**
> "Create a bug task 'Login timeout on slow connections' in web-app and assign it to janedoe."

**🤖 AI Agent:**
> Created task 'WEB-51: Login timeout on slow connections' as a Bug type in the web-app project, assigned to janedoe, placed in the 'To Do' column. The task code is WEB-51. Shall I add a checklist for the investigation steps or set a due date?

---

**👤 You:**
> "Add a checklist to task WEB-42 with items for 'Write unit tests', 'Update docs', and 'Deploy to staging'."

**🤖 AI Agent:**
> Done! Added 3 checklist items to WEB-42: ☐ Write unit tests, ☐ Update docs, ☐ Deploy to staging. All start as unchecked. Shall I mark any as complete or add sub-items under any of them?


## ❓ FAQ

**Q: Can my AI agent find a specific task by its human-readable code like WEB-42?**
Yes! Use the `get_task_by_code` tool with the task code (e.g., WEB-42). Your agent will return the full task details including description, assignees, workflow status, labels, sprint association, time estimates, and checklist progress — in seconds.

**Q: I want to quickly see what I need to work on today. Can the agent help?**
Absolutely. Use `my_today_tasks` to see everything due today, or `my_tasks` for your full assignment list across all workspaces. The agent returns task titles, project context, due dates, and current workflow status — your daily standup briefing in one command.

**Q: Can the agent manage task assignments and checklists too?**
Yes. Use `assign_member` and `unassign_member` to manage task assignments by username. For checklists, use `create_checklist_item` to add items (including nested sub-items via parent_id), and `toggle_checklist_item` to mark them done. The complete task lifecycle is covered — from creation to completion.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gitscrum-tasks](https://vinkius.com/mcp/gitscrum-tasks)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GitScrum Tasks** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gitscrum-tasks` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GitScrum Tasks** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gitscrum-tasks": {
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
