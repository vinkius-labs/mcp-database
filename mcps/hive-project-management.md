# Hive (Project Management) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hive-project-management)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage projects via Hive — create actions, track initiatives, and organize workspaces.

## Description
Connect your **Hive** account to any AI agent and take full control of your project management and team collaboration through natural conversation.

### What you can do

- **Workspace Management** — List all available workspaces and navigate across different tenant environments effortlessly
- **Project Tracking** — Analyze grouping schemas linking large initiatives and monitor the status of team projects directly from your agent
- **Action Items** — Create and list operational tasks (actions), linking precise items and checking team assignments in real-time
- **Detailed Inspection** — Retrieve exact metadata and structural details for specific action IDs to understand progress and blockers
- **Taxonomy & Labels** — Discover discrete visual categorizations and taxonomy matrices used to organize your workspace items
- **Workflow Templates** — Enumerate active repeatable workflows and action templates to maintain process consistency across your team

### How it works

1. Subscribe to this server
2. Enter your Hive API Key
3. Start managing your team's productivity from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — track initiatives and list actions to prepare for weekly syncs through natural conversation
- **Team Leads** — create new tasks and monitor team assignments without switching context from your communication tool
- **Operations Teams** — audit workspace labels and action templates to ensure standardized project delivery workflows


## Available Tools
- **list_workspaces**: List workspaces
- **list_projects**: List projects
- **list_actions**: List actions
- **create_action**: Create action
- **get_action**: Get action
- **list_labels**: List labels
- **list_templates**: List action templates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hive (Project Management)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all projects in my 'Marketing' workspace (ID: ws-marketing)"

**🤖 AI Agent:**
> I've found 4 active projects in the Marketing workspace: 'Q2 Social Campaign', 'Brand Refresh', 'Email Newsletter Automation', and 'Annual Event Planning'. Would you like the status of the social campaign?

---

**👤 You:**
> "Create a new action called 'Finalize Budget' in workspace 'ws-finance'"

**🤖 AI Agent:**
> Action 'Finalize Budget' created successfully in your Finance workspace. It's currently unassigned and has no labels. Would you like me to assign it to Sarah or add a 'Priority' label?

---

**👤 You:**
> "What are the action templates available in the 'Engineering' workspace?"

**🤖 AI Agent:**
> I've identified 3 action templates in Engineering: 'Bug Report', 'Feature Specification', and 'Code Review Checklist'. You can use these templates to ensure all required fields are filled when creating new actions.


## ❓ FAQ

**Q: Can I create new tasks directly through my agent?**
Yes. Use the `create_action` tool to generate new tasks in a specific workspace. You provide the title and workspace ID, and your agent will handle the backend orchestration to create the action instantly.

**Q: How do I find my Workspace ID?**
Ask your agent to `list_workspaces`. It will return a list of all workspaces you have access to, along with their unique IDs, which are required for project and action operations.

**Q: Can I see the templates we have defined for repeatable workflows?**
Absolutely. Use the `list_templates` tool to see all action templates in a workspace. This helps your agent understand the predefined workflows your team uses for consistent project delivery.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hive-project-management](https://vinkius.com/mcp/hive-project-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hive (Project Management)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hive-project-management` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hive (Project Management)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hive-project-management": {
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
