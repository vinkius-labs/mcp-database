# VivifyScrum MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vivifyscrum)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage agile projects with Scrum and Kanban boards, sprint planning, and backlog grooming for software development teams.

## Description
Connect your **VivifyScrum** account to any AI agent and simplify how you manage your Scrum and Kanban workflows through natural conversation.

### What you can do

- **Board Management** — List all boards and organizations, and retrieve detailed configuration metadata for specific project spaces.
- **Task Control** — Create, list, and update items (tasks and stories) directly on your agile boards.
- **Sprint Planning** — List sprints for a board to track progress and plan future development cycles.
- **Team Coordination** — Query team lists and organization members to manage access and visibility.
- **Operational Tracking** — Monitor worklogs for time tracking and list configured webhooks for event monitoring.

### How it works

1. Subscribe to this server
2. Enter your VivifyScrum API Token (found in your account profile settings)
3. Start managing your agile projects from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers & Scrum Masters** — quickly retrieve board items and sprint statuses via simple AI queries.
- **Agile Teams** — update task descriptions and check worklogs without leaving the workspace.
- **Product Owners** — monitor project progress and organization structure directly from the AI assistant.


## Available Tools (12)
- **get_worklogs**: Get board worklogs
- **list_boards**: List all boards
- **list_board_items**: List items on a board
- **list_organizations**: List all organizations
- **list_sprints**: List board sprints
- **list_teams**: List all teams
- **list_webhooks**: List configured webhooks
- **update_item**: Update an item
- **create_item**: Create a new task/story
- **get_account_info**: Get account details
- **get_board**: Get board details
- **get_item**: Get item details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VivifyScrum** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all boards in my VivifyScrum account."

**🤖 AI Agent:**
> I've retrieved your boards. You have access to: 'Product Development' (Scrum), 'Marketing Content' (Kanban), and 'Customer Support'. Which one would you like to open?

---

**👤 You:**
> "Show me the tasks for the 'Product Development' board."

**🤖 AI Agent:**
> I've fetched the items. There are 5 active tasks including 'Implement MCP Server', 'Fix login bug', and 'Design new logo'. Would you like details on any specific task?

---

**👤 You:**
> "Create a new task named 'Verify API Scopes' on board '88231'."

**🤖 AI Agent:**
> Success! The task 'Verify API Scopes' has been created on board 88231 (ID: task_10293). Shall I add a description to it?


## ❓ FAQ

**Q: Can I list all the tasks assigned to a specific board?**
Yes! Use the `list_board_items` tool and provide the Board ID. Your agent will retrieve all tasks and stories for that project.

**Q: How do I see the active sprints for my project?**
Run the `list_sprints` query with your Board ID. The agent will return a list of all sprints associated with that board, including their current status.

**Q: Is it possible to track time logs via AI?**
Absolutely. Use the `get_worklogs` tool with your Board ID to retrieve the history of time tracking entries for that project.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vivifyscrum](https://vinkius.com/mcp/vivifyscrum)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **VivifyScrum** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vivifyscrum` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **VivifyScrum** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vivifyscrum": {
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
