# KanbanTool MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kanbantool)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Visualize your workflow with Kanban boards that show bottlenecks, track cycle times, and help your team deliver consistently.

## Description
Connect your **KanbanTool** account to any AI agent and manage kanban boards through natural conversation.

### What you can do

- **Board Management** — List all boards, inspect layouts, and configure columns
- **Task Management** — Create, move, update, and archive cards across columns
- **Workflow Tracking** — Monitor cards across workflow stages (To Do, In Progress, Done)
- **Team Collaboration** — Assign cards to team members and track workload
- **WIP Monitoring** — Track work-in-progress limits and bottlenecks
- **Activity History** — View card activity and changelog

### How it works

1. Subscribe to this server
2. Enter your KanbanTool subdomain and API Token
3. Start managing boards from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — manage tasks and monitor workflow progress
- **Development Teams** — track sprint boards and WIP limits
- **Operations** — organize work across stages and teams


## Available Tools
- **archive_task_card**: Archive a task card
- **create_task_card**: Add a new card to a board
- **get_board_details**: Get metadata and tasks for a board
- **get_user_profile**: Get current user profile
- **get_task_details**: Get details for a task
- **list_task_activities**: List history for a task
- **list_boards**: List your Kanban boards
- **list_shared_links**: List shared board links
- **list_board_tasks**: List tasks on a board
- **update_task_details**: Modify an existing task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **KanbanTool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all boards and the cards in the 'Sprint Board' by column."

**🤖 AI Agent:**
> Boards: 4. Sprint Board (42 cards), Product Roadmap (18), Bug Tracker (23), Onboarding (8). Sprint Board columns: Backlog (12 cards), To Do (8, WIP: 10), In Progress (6/5 ⚠️ over WIP), Review (4/4 at limit), Testing (3), Done (9). ⚠️ 'In Progress' exceeds WIP limit by 1. Would you like to move cards or create new ones?

---

**👤 You:**
> "Create a new card 'Implement OAuth' in To Do and move 'API Rate Limiting' to Done."

**🤖 AI Agent:**
> Card created! 'Implement OAuth' in To Do (card_4521). Priority: High. Assigned: Sarah Chen. To Do: 8 → 9 cards (WIP: 10). Card moved! 'API Rate Limiting' → Done ✅. In Progress: 6 → 5 cards (WIP restored). Done: 9 → 10 cards. Sprint velocity: 10 cards completed this sprint.

---

**👤 You:**
> "Show team workload and all cards assigned to Sarah."

**🤖 AI Agent:**
> Team workload: Sarah Chen — 8 cards (3 In Progress, 2 Review, 3 To Do). Mike Torres — 6 cards (2 In Progress, 4 To Do). Lisa Park — 5 cards (1 In Progress, 2 Testing, 2 To Do). Sarah's cards: 'Implement OAuth' (To Do, High), 'Refactor Auth Module' (In Progress, 2 days), 'Dashboard Redesign' (In Progress, 4 days), 'Write API Docs' (Review), 5 others. Sarah's average cycle time: 3.2 days.


## ❓ FAQ

**Q: Can I create and move cards across board columns?**
Yes. Create new cards in any column, move them across workflow stages, update details, and archive completed cards. Track card history and activity.

**Q: Does KanbanTool require a subdomain?**
Yes. Each KanbanTool account has a unique subdomain (e.g., `your-team`). Provide the subdomain and API Token. Bearer token against `https://{subdomain}.kanbantool.com/api/v3`.

**Q: Can I monitor WIP limits and identify bottlenecks?**
Yes. Track how many cards are in each column relative to WIP limits. Identify bottleneck columns where work is accumulating beyond limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kanbantool](https://vinkius.com/mcp/kanbantool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **KanbanTool** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `kanbantool` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **KanbanTool** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kanbantool": {
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
