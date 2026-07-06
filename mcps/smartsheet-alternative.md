# Smartsheet MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/smartsheet-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage sheets, reports, and rows on Smartsheet with AI agents.

## Description
Connect your **Smartsheet** account to any AI agent to automate your enterprise work management and collaboration orchestration. Smartsheet provides a powerful platform for tracking projects and data, and this integration allows you to retrieve sheet metadata, manage rows, and search through workspaces through natural conversation.

### What you can do

- **Sheet & Data Orchestration** — List all managed sheets and retrieve detailed profile metadata, including columns and structural definitions programmatically.
- **Row Lifecycle Management** — Add, update, and delete rows within your sheets with full control over cell data directly from the AI interface.
- **Workspace & Report Control** — Access and monitor your workspaces and reports to maintain a clear overview of your projects via natural language.
- **Search & Discovery Intelligence** — Search through specific sheets to quickly find the information you need and retrieve filtered data results.
- **Operational Monitoring** — Access user profiles and monitor system health to ensure reliable data synchronization between Smartsheet and your AI workflows.

### How it works

1. Subscribe to this server
2. Enter your Smartsheet Access Token from your account settings
3. Start managing your enterprise work from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — quickly update project statuses and monitor report details without switching between sheets.
- **Operations Teams** — automate the retrieval of resource data and manage team rows via natural conversation.
- **Data Analysts** — streamline the retrieval of sheet metadata and monitor data collection directly within the chat.


## Available Tools (12)
- **get_sheet_details**: Get sheet data
- **get_workspace_details**: Get workspace info
- **list_sheet_columns**: List sheet fields
- **list_available_reports**: List filtered reports
- **list_sheets**: List Smartsheet sheets
- **list_platform_users**: List company users
- **list_workspaces**: List project workspaces
- **search_within_sheet**: Find data in sheet
- **update_sheet_rows**: Rows must be provided as a JSON array with IDs.

Modify existing rows
- **add_sheet_rows**: Rows must be provided as a JSON array.

Append new rows
- **remove_sheet_row**: Delete a row
- **get_my_profile**: Get user info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Smartsheet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active sheets in my Smartsheet account."

**🤖 AI Agent:**
> I've retrieved your sheets. You have 5 active ones including 'Project Roadmap', 'Budget Tracker', and 'Team Tasks'. Which one would you like to open?

---

**👤 You:**
> "Show me all active project sheets with their task completion rates and upcoming deadlines."

**🤖 AI Agent:**
> 8 active project sheets. "Product Launch Q2" (156 rows): 72% complete, 12 tasks due this week, 3 overdue (critical path items). "Website Redesign" (89 rows): 45% complete, on track, next milestone Friday. "Data Migration" (234 rows): 88% complete, final testing phase. "Marketing Campaign" (67 rows): 34% complete, 5 blocked tasks. "Office Relocation" (45 rows): 60% complete. 3 additional sheets at various stages. Total tasks across all sheets: 734. Overdue: 18 (2.5%). Resource conflicts: 4 team members over-allocated.

---

**👤 You:**
> "Create a new project sheet from the Agile Sprint template and add the engineering team as collaborators."

**🤖 AI Agent:**
> Project sheet created: "Sprint 14 - API Platform". Template: Agile Sprint (columns: Story, Points, Assignee, Status, Priority, Sprint, Epic). 6 team members added as editors: Sarah Chen, James Park, Alex Rivera, Lisa Wang, David Kim, Maria Santos. Default views created: Board (Kanban by Status), Gantt (timeline), Calendar (due dates). Automation rules: status change notifications, overdue alerts, sprint burndown chart updates. Sprint dates set: May 19-30. Ready for backlog import.


## ❓ FAQ

**Q: How do I find my Smartsheet Access Token?**
Log in to Smartsheet, navigate to **Account** > **Personal Settings** > **API Access**, and generate a new access token for your integration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smartsheet-alternative](https://vinkius.com/mcp/smartsheet-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Smartsheet** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `smartsheet-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Smartsheet** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "smartsheet-alternative": {
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
