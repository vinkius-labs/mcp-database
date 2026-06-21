# Todoist MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/todoist)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage tasks, organize projects, and streamline your personal or team workflows natively with your AI agent.

## Description
Connect your **Todoist** account to any AI agent and bring your daily productivity directly into your chat. View your active tasks, manage projects, and quickly add new items to your workflow entirely through conversational commands without ever needing to open the app.

### What you can do

- **Project Management** — List all your active project folders, retrieve their specific IDs, and view sections within specific projects
- **Task Execution** — View your complete list of pending tasks and mark them as completed instantly
- **Create Tasks** — Add new items to a specific project or your inbox naturally in plain conversation
- **Organization** — Look up available labels/tags to categorize your work
- **Collaboration** — Read through existing comments to catch up on discussion history for any particular task

### How it works

1. Subscribe to this server
2. Navigate to your Todoist integrations page and generate your personal API Token
3. Plug the token into your setup and start executing task-management queries naturally

### Who is this for?

- **Productivity Enthusiasts** — Log and review pending actions directly from their command center
- **Project Managers** — Keep track of tasks and labels actively across different contexts without switching contexts
- **Software Developers** — Check off coding chores or track individual project issues directly from their connected IDEs


## Available Tools (7)
- **complete_task**: Marks a task as completed
- **create_task**: Provide content and an optional project ID.

Creates a new task in Todoist
- **list_comments**: Lists all comments for a specific task
- **list_labels**: Lists all user-defined labels
- **list_projects**: Lists all active projects in Todoist
- **list_sections**: Lists all sections within a specific project
- **list_tasks**: Can filter by project_id.

Lists active tasks, optionally filtered by project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Todoist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check all my active tasks and projects."

**🤖 AI Agent:**
> I've retrieved 3 projects (Personal, Work, Grocery). Under your Inbox, you have 1 active task:
- Task: 'Summarize weekly sync', ID: 81229

---

**👤 You:**
> "Complete the task with ID 81229."

**🤖 AI Agent:**
> I have successfully marked the task 81229 as completed in your Todoist workspace.


## ❓ FAQ

**Q: Where do I get my Todoist API Token?**
You can locate your personal API Token securely via the web application by clicking your profile avatar, going to **Settings**, and selecting the **Integrations** tab. Your token will be visible at the bottom or in a dedicated Developer section. Alternatively, navigate directly to `https://todoist.com/prefs/integrations`.

**Q: Can the agent delete projects or workspaces?**
No. The integration exclusively lists resources (projects, items, labels) and supports only basic item modifications: creating tasks and marking tasks as completed. Destructive actions on structural settings are not supported.

**Q: Can the agent organize my tasks using sub-projects or sections?**
Yes. The Todoist integration allows the agent to retrieve project IDs and navigate into their specific sections. When creating a new task, you can explicitly ask the agent to place it within a specific section to keep your work neatly organized.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/todoist](https://vinkius.com/mcp/todoist)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `todoist` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Todoist** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "todoist": {
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
