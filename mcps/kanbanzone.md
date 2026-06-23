# KanbanZone MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kanbanzone)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage projects visually with multi-board Kanban views, WIP limits, and process metrics that streamline team delivery.

## Description
Connect your **KanbanZone** account to any AI agent and manage kanban boards through natural conversation.

### What you can do

- **Board Management** — List boards, inspect column layouts, and configure settings
- **Card Operations** — Create, update, move, and archive cards across columns
- **Swimlane Organization** — Browse and manage swimlanes for categorized workflows
- **WIP Monitoring** — Track work-in-progress limits per column
- **Activity Tracking** — View card history and board activity logs

### How it works

1. Subscribe to this server
2. Enter your KanbanZone API Token
3. Start managing boards from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — organize work and track workflow stages
- **Agile Teams** — manage sprint boards with WIP limits
- **Operations** — visualize and automate process workflows


## Available Tools (8)
- **create_cards**: Add multiple cards to a board
- **create_webhook**: Create a new board webhook
- **delete_webhook**: Remove a board webhook
- **list_boards**: List all Kanban boards
- **list_cards**: List cards on a board
- **list_webhooks**: List webhooks for a board
- **move_card**: Move a card to a different column
- **update_card**: Update an existing card


## 💬 Prompt Examples

Here are some examples of how you can interact with the **KanbanZone** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all boards and cards in the 'Development' board by column."

**🤖 AI Agent:**
> Boards: 3. Development (28 cards), Marketing (15), Operations (12). Development: Backlog (8), To Do (6/8), In Progress (5/5 at limit), Review (4), Testing (2), Done (3). Swimlanes: Frontend, Backend, DevOps. ⚠️ In Progress at WIP limit.

---

**👤 You:**
> "Create a card 'Fix login bug' and move 'API migration' to Done."

**🤖 AI Agent:**
> Card created! 'Fix login bug' in To Do, Priority: High, Swimlane: Frontend. To Do: 6→7. Card moved! 'API migration' → Done ✅. In Progress: 5→4 (below WIP). Done: 3→4.

---

**👤 You:**
> "Show swimlane breakdown and board activity for today."

**🤖 AI Agent:**
> Swimlanes: Frontend (10 cards, 2 in progress), Backend (12 cards, 2 in progress), DevOps (6 cards, 1 in progress). Today's activity: 8 actions. 3 cards moved, 2 created, 1 archived, 2 updated. Most active: Sarah (4 actions).


## ❓ FAQ

**Q: Can I create and move cards across board columns?**
Yes. Create cards in any column, move them across workflow stages, update details and assignees, and archive completed work.

**Q: How does KanbanZone authentication work?**
KanbanZone uses **HTTP Basic Auth** with the API Token against `integrations.kanbanzone.io/v1`. This differs from the standard Bearer token pattern.

**Q: Can I organize work using swimlanes?**
Yes. Browse and manage swimlanes to categorize cards by project, team, or priority within each board.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kanbanzone](https://vinkius.com/mcp/kanbanzone)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **KanbanZone** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kanbanzone` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **KanbanZone** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kanbanzone": {
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
