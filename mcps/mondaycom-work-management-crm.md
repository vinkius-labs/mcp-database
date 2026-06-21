# Monday.com (Work Management & CRM) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mondaycom-work-management-crm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage work via Monday.com — list project boards, track task items, and audit team workspaces.

## Description
Connect your **Monday.com** account to any AI agent and take full control of your enterprise work management, project tracking, and team collaboration through natural conversation.

### What you can do

- **Board Orchestration** — List all managed project boards and retrieve detailed structural configurations including custom columns and dimension mappings directly from your agent
- **Task & Item Monitoring** — List discrete task items (rows) bounded inside specific boards and retrieve detailed column values representing literal project data securely
- **Workspace Navigation** — Explore high-level organizational 'Workspaces' (folders) to understand your department's reporting taxonomy and project groupings natively
- **Team Audit** — Enumerate explicitly bounded team users and member identities to cross-reference task ownership and resource assignments across your organization
- **Credential Identity** — Verify your active caller identity and metadata context to ensure your agent is targeting the correct account boundaries securely
- **Metadata Inspection** — Deep-dive into specific Board or Workspace IDs to retrieve precise GraphQL node representations and project insights instantly

### How it works

1. Subscribe to this server
2. Enter your Monday.com API Token
3. Start managing your work platform from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — monitor project statuses and audit task distributions through natural conversation without manual board navigation
- **Team Leads** — track resource assignments and verify column mappings across multiple boards directly from your workspace
- **Operations Managers** — manage organizational workspaces and retrieve rapid project summaries to maintain team alignment efficiently


## Available Tools (13)
- **get_me**: Get current user profile
- **archive_item**: Can be unarchived later from the board settings.

Archive a board item
- **create_item**: Create a new item in a board
- **create_update**: Add a comment/update to an item
- **delete_item**: The item and its updates will be removed.

Permanently delete a board item
- **get_board**: Get structure of a specific board
- **list_boards**: List Monday.com project boards
- **list_groups**: List groups (sections) in a board
- **list_items**: List task items in a board
- **list_subitems**: List sub-items of a board item
- **list_updates**: List updates/comments for an item
- **list_users**: List team members in the account
- **list_workspaces**: List Monday.com workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Monday.com (Work Management & CRM)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all boards in my Monday.com account"

**🤖 AI Agent:**
> I've retrieved 3 project boards from your account: 'Product Roadmap 2026' (ID: 12345), 'Marketing Campaign' (ID: 67890), and 'Inventory Sync' (ID: 13579). Which one would you like to list the tasks for?

---

**👤 You:**
> "Show me all tasks in the 'Product Roadmap 2026' board"

**🤖 AI Agent:**
> Retrieving items from 'Product Roadmap 2026'… I've identified 12 tasks. Highlights include 'API Integration' (Status: Done), 'Mobile UI Design' (Status: Working on it), and 'Beta Testing' (Status: Stuck). Would you like to see the assignee for any of these?

---

**👤 You:**
> "List all active team members in our Monday account"

**🤖 AI Agent:**
> I've retrieved your Monday.com user directory. There are 25 active members, including 'Alex Smith' (Admin), 'Sarah Johnson' (Member), and 'Mark Rivera'. I can help you find their internal IDs for task assignments if you'd like.


## ❓ FAQ

**Q: Can I see the column structure of a Monday board through my agent?**
Yes. Use the `get_board` tool with a specific Board ID. Your agent will retrieve the detailed structural configuration, exposing the custom column types and titles used to organize your project data.

**Q: How do I list the tasks (items) within a specific board?**
The `list_items` tool retrieves all discrete GraphQL nodes representing rows in a board. Your agent will return the task names and their associated column values, helping you audit project progress without opening the browser.

**Q: Can my agent navigate between different organizational workspaces?**
Absolutely. Use the `list_workspaces` tool to identify the top-level directory structure of your Monday account. Your agent will report the workspace names and IDs, allowing you to locate boards grouped by department or team.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mondaycom-work-management-crm](https://vinkius.com/mcp/mondaycom-work-management-crm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Monday.com (Work Management & CRM)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mondaycom-work-management-crm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Monday.com (Work Management & CRM)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mondaycom-work-management-crm": {
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
