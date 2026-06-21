# Linear MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linear)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Streamline issue tracking and project management via Linear — list teams, query issues, create comments and inspect cycles directly from any AI agent.

## Description
Connect your **Linear** workspace to any AI agent and take full control of your issue tracking and sprint workflows through natural conversation.

### What you can do

- **User & Team Discovery** — Retrieve the authenticated user profile and list all teams configured in your Linear workspace
- **Issue Management** — List, search, inspect and create issues with full metadata including assignees, labels, priority and state
- **Project Oversight** — Browse all active projects, view their status and drill into specific project details by ID
- **Comments & Collaboration** — Add comments to issues to keep your team context aligned without switching to the Linear app
- **Cycle Tracking** — List all sprint cycles for any team, including start/end dates and completion progress
- **Label Organization** — View all issue labels used for categorization across teams

### How it works

1. Subscribe to this server
2. Enter your Linear Personal API Key
3. Start managing your sprints from Claude, Cursor, or any MCP-compatible client

No more tab-switching to check issue status or hunt for the right assignee. Your AI acts as an on-demand engineering manager.

### Who is this for?

- **Engineering Managers** — instantly pull issue summaries, check cycle progress and audit sprint health without opening Linear
- **Developers** — create and update issues, add comments and check assignees directly from your IDE
- **Product Teams** — monitor project statuses and search across issues to understand feature scope and blockage


## Available Tools (12)
- **create_comment**: The body supports Linear Markdown format including @mentions and ~~strikethrough~~.

Add a comment to a Linear issue
- **create_issue**: Requires the team ID and issue title. Optionally set description, assignee, priority (0=No priority, 1=Urgent, 2=High, 3=Normal, 4=Low) and label IDs.

Create a new Linear issue
- **list_cycles**: Each cycle has a number, name, start date, end date and completion progress percentage.

List Linear cycles (sprints) for a team
- **get_issue**: Use the issue ID (UUID) or the human-readable identifier (e.g. TEAM-123).

Get full details for a Linear issue
- **get_project**: Get details for a specific Linear project
- **list_issues**: Optionally filter by team ID to get issues for a specific team only.

List Linear issues
- **list_labels**: Optionally filter by team ID. Each label has a name, color and optional description.

List Linear issue labels
- **list_projects**: Projects group issues across multiple teams. Use optional limit to control how many results to fetch.

List Linear projects
- **search_issues**: Optionally filter results to a specific team. Returns issues with identifier, title, state, priority, assignee and URL.

Search Linear issues by text
- **list_teams**: Each team has a unique ID, name, key prefix and optional description. Use this to discover teams before querying their issues or cycles.

List all Linear teams
- **update_issue**: Provide the issue ID (UUID) and only the fields you want to change.

Update an existing Linear issue
- **get_viewer**: Useful to verify which account the API token belongs to.

Get current authenticated Linear user details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Linear** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all unresolved issues assigned to the Engineering team."

**🤖 AI Agent:**
> I've queried your Engineering team and found 7 open issues. The highest priority items are 'Fix auth token refresh bug' (ENG-142) and 'Implement pagination for API responses' (ENG-138). Would you like full details on either?

---

**👤 You:**
> "Create a new issue in the Backend team titled 'Add rate limiting to /api/search endpoint' with high priority."

**🤖 AI Agent:**
> Done! I've created issue **BE-217** titled 'Add rate limiting to /api/search endpoint' with priority High in the Backend team. You can view it at linear.app/yourco/issue/BE-217.

---

**👤 You:**
> "What's the current sprint cycle progress for the Mobile team?"

**🤖 AI Agent:**
> The Mobile team's active cycle is #47 (Mar 31 — Apr 13) with 62% completion. There are 14 issues in this cycle, 5 of which are already done. Would you like the list of remaining open issues?


## ❓ FAQ

**Q: How do I find my Linear Personal API Key?**
Go to [**Linear Settings > API**](https://linear.app/settings/api) and click **Create API Key**. Give it a descriptive name like 'Vinkius MCP' and copy the generated key immediately — it won't be shown again.

**Q: Can I create new issues with assignees and labels?**
Yes! Use the `create_issue` tool with the required `team_id` and `title` parameters. Optionally provide `assignee_id`, `priority` (0-4), `description` in Markdown and `label_ids` as a comma-separated list. The agent will return the created issue's identifier and URL.

**Q: Does the agent have access to delete issues or modify team settings?**
No. This server focuses on read operations and safe mutations — creating issues, updating fields and adding comments. Destructive actions like deletion or team configuration changes are not exposed, keeping your workspace secure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linear](https://vinkius.com/mcp/linear)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Linear** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `linear` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Linear** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linear": {
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
