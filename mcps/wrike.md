# Wrike MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wrike)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage tasks, projects, and folders on Wrike — the most versatile work management platform for teams.

## Description
Connect your **Wrike** account to any AI agent and manage your enterprise workflows through natural conversation.

### What you can do

- **Task Monitoring** — List and browse tasks across your entire account or filter by specific folder/project IDs
- **Deep Task Analysis** — Retrieve comprehensive metadata for specific tasks, including descriptions, assignees, and custom fields
- **Project Navigation** — Browse top-level project containers and monitor their current status and organization
- **Folder Hierarchy** — Explore your organizational structure to understand how tasks are grouped and categorized
- **Team Discovery** — List all users and contacts within your Wrike workspace to find IDs for task assignment
- **Space Access** — List all available work areas (spaces) to navigate your team's different departments or functions
- **Workflow Automation** — Quickly find unique task and folder IDs required for building automated project management flows

### How it works

1. Subscribe to this server
2. Enter your Wrike Access Token
3. Start managing your tasks and projects through Claude, Cursor, or any MCP-compatible client

No more manual digging through complex project folders to find an update. Your AI agent becomes your project operations assistant.

### Who is this for?

- **Project Managers** — monitor task progress and audit project health through simple chat commands
- **Team Leads** — lookup team member IDs and browse departmental spaces without manual navigation
- **Operations Managers** — audit folder structures and verify task assignments across the workspace
- **Executive Assistants** — quickly surface task details and project statuses for reporting and coordination


## Available Tools
- **get_task_details**: Retrieves comprehensive details for a specific Wrike task
- **list_wrike_contacts**: Lists all users and contacts within the Wrike workspace
- **list_wrike_folders**: Lists all folders and projects in the Wrike account
- **list_wrike_projects**: Lists all active projects in the account
- **list_wrike_spaces**: Lists all Wrike spaces available to the authenticated user
- **list_wrike_tasks**: You can optionally provide a folder_id to scope the results.

Lists tasks in the Wrike account, optionally filtered by folder


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wrike** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Wrike projects."

**🤖 AI Agent:**
> I found 5 active projects in your account: 1. 'Product Launch 2026' (ID: IE...), 2. 'Q1 Marketing Campaign' (ID: IE...), 3. 'Internal Website Redesign' (ID: IE...), and 2 others. Which one would you like to explore?

---

**👤 You:**
> "Show me tasks in the 'Product Launch 2026' folder."

**🤖 AI Agent:**
> Searching folder 'Product Launch 2026' (ID: IE...)... I found 8 tasks. The most recent are: 1. 'Finalize Design Specs' (Status: Active), 2. 'Coordinate with Vendors' (Status: Active), and 3. 'Budget Approval' (Status: Completed). Would you like the details for any of these?

---

**👤 You:**
> "Get full details for task ID 'IEA...'."

**🤖 AI Agent:**
> Task 'Finalize Design Specs' (ID: IEA...): Description: 'Complete the UI/UX documentation for the mobile dashboard'. Status: Active, Priority: High, Assigned to: John Doe. Would you like me to check for any custom field values?


## ❓ FAQ

**Q: Can I check the details of a specific task through the agent?**
Yes. The `get_task_details` tool allows your AI agent to retrieve full metadata for any specific task ID, including its description, current status, assignees, and any custom fields you have configured.

**Q: How do I find tasks belonging to a specific folder or project?**
You can use the `list_wrike_tasks` tool and provide the unique `folder_id`. Your agent will return all tasks contained within that specific organizational unit, helping you stay focused on a specific project.

**Q: Is it possible to see all my team members' contact IDs via chat?**
Absolutely. The `list_wrike_contacts` tool retrieves all users and contacts in your Wrike workspace, providing their names and unique contact IDs required for task assignment or mentions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wrike](https://vinkius.com/mcp/wrike)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wrike** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `wrike` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wrike** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wrike": {
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
