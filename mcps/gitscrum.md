# GitScrum MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gitscrum)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage workspaces, projects, workflows, and labels via GitScrum — browse your organizational structure and configure boards directly from any AI agent.

## Description
### What you can do

- **Browse workspaces** — list all your organizational workspaces and retrieve details for each one
- **Manage projects** — list, create, and inspect projects with full metadata including members and settings
- **Configure workflows** — view and manage Kanban column definitions and workflow templates
- **Organize with labels** — list, create, and update color-coded labels to categorize work
- **Access your profile** — retrieve the authenticated user's profile across all workspaces

### How it works

1. Subscribe to the GitScrum integration from the marketplace
2. Generate a personal API token in GitScrum Settings → API and enter it along with your company slug
3. Start asking your AI agent to explore workspaces, create projects, or configure boards — works in Claude, Cursor, and any MCP-compatible client

Your agent becomes your command center for the organizational backbone of GitScrum.

### Who is this for?

- **Engineering managers** — quickly audit workspace structure and project configurations without switching tabs
- **Team leads** — set up new projects with workflows and labels in seconds via natural language
- **Developers** — inspect project settings and member lists during planning sessions


## Available Tools (16)
- **find_project**: Find a project by name
- **get_project**: Get project details
- **list_projects**: List projects in a workspace
- **project_stats**: Get project statistics
- **get_task**: Get task details by UUID
- **list_tasks**: Filter by status (todo, in-progress, done). Essential for understanding project scope and workload.

List tasks in a project
- **list_workflows**: List workflows (columns) in a project
- **create_workspace**: Create a new workspace
- **get_workspace**: Get workspace details
- **list_workspaces**: List all GitScrum workspaces
- **workspace_stats**: Get workspace statistics
- **list_labels**: List labels in a project
- **get_me**: Get authenticated user profile
- **list_project_members**: List members in a project
- **my_role**: Get my role in the workspace
- **create_project**: Create a new project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GitScrum** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all the workspaces I have access to on GitScrum."

**🤖 AI Agent:**
> I found 3 workspaces on your account: 'Acme Engineering' (slug: acme-eng), 'Design Studio' (slug: design-studio), and 'Internal Ops' (slug: internal-ops). The first one has 12 active projects. Which workspace would you like to explore?

---

**👤 You:**
> "Create a new project called 'Mobile App v2' in the acme-eng workspace with a description."

**🤖 AI Agent:**
> Done! 'Mobile App v2' has been created in the acme-eng workspace with slug 'mobile-app-v2'. It's set up with the default workflow columns: To Do, In Progress, Review, and Done. Shall I add custom labels or invite team members?

---

**👤 You:**
> "What labels are available in the web-app project?"

**🤖 AI Agent:**
> The web-app project has 5 labels: 🔴 'Critical' (#E74C3C), 🟡 'Enhancement' (#F39C12), 🔵 'Frontend' (#3498DB), 🟢 'Backend' (#27AE60), and 🟣 'DevOps' (#9B59B6). Would you like to create additional labels or apply any of these to tasks?


## ❓ FAQ

**Q: Can my AI agent list all workspaces and drill into specific project details?**
Absolutely. Use `list_workspaces` to browse all your organizational workspaces, then `list_projects` to see every project within a workspace. Your agent returns full metadata including member counts, settings, and creation dates — all without leaving your conversation.

**Q: I need to set up a new project with custom workflows and labels — can I do it all conversationally?**
Yes. Tell your agent to create the project, then ask it to configure the workflow columns and create color-coded labels. The agent chains `create_project`, `list_workflows`, and `create_label` tools automatically to set up your board exactly as you describe it.

**Q: Does this integration let me modify or delete projects?**
This core integration focuses on workspace exploration, project creation, and configuration management — including workflows and labels. For task-level operations like CRUD, subtasks, and checklists, use the dedicated GitScrum Tasks integration. All actions respect your GitScrum account permissions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gitscrum](https://vinkius.com/mcp/gitscrum)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GitScrum** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gitscrum` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GitScrum** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gitscrum": {
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
