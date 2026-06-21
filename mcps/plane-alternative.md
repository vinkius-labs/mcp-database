# Plane MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plane-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage projects, issues, and product roadmaps via Plane — create projects, toggle features, and organize workspaces directly from your AI agent.

## Description
Connect your **Plane** workspace to any AI agent to streamline your open-source project management. Take full control of your project lifecycle and feature configurations through natural language.

### What you can do

- **Project Lifecycle** — List all projects in a workspace, create new ones with custom identifiers, or retrieve specific project details instantly.
- **Feature Management** — Dynamically enable or disable project modules such as Epics, Cycles, Modules, Pages, and Intakes to suit your team's workflow.
- **Workspace Organization** — Keep your workspace clean by archiving, unarchiving, or deleting projects that are no longer active.
- **Project Metadata** — Update project names, descriptions, and lead assignments without leaving your conversation or code editor.

### How it works

1. Subscribe to this server
2. Enter your Plane API Key
3. Start managing your agile workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — Quickly spin up new projects and configure necessary features like Epics or Cycles for upcoming sprints.
- **Engineering Leads** — Audit project settings and archive completed work directly from the terminal or chat interface.
- **DevOps Teams** — Automate project creation and workspace maintenance as part of larger organizational workflows.


## Available Tools
- **archive_project**: Archive a project
- **create_project_label**: Create a project label
- **create_project**: Create a new project
- **delete_project**: Delete a project
- **get_project_features**: ) are enabled for a project.

Get project features
- **get_project_label**: Get a specific project label
- **get_project**: Retrieve a specific project
- **list_project_labels**: List project labels
- **list_projects**: List all projects in a workspace
- **unarchive_project**: Unarchive a project
- **update_project_features**: Update project features
- **update_project**: Update an existing project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plane** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all projects in the 'vinkius-dev' workspace."

**🤖 AI Agent:**
> I've found 3 projects in 'vinkius-dev': 'Mobile App' (MOB), 'Backend API' (API), and 'Marketing Site' (MKT). Which one would you like to explore?

---

**👤 You:**
> "Create a new project named 'Customer Portal' with identifier 'PORT' in workspace 'vinkius-dev'."

**🤖 AI Agent:**
> Project 'Customer Portal' has been successfully created with the identifier PORT in your workspace.

---

**👤 You:**
> "Enable Epics and Cycles for project 'PORT' in workspace 'vinkius-dev'."

**🤖 AI Agent:**
> I have updated the features for project 'PORT'. Epics and Cycles are now enabled.


## ❓ FAQ

**Q: Can I enable or disable specific features like Epics or Cycles for a project?**
Yes! You can use the `update_project_features` tool to toggle capabilities including epics, modules, cycles, views, pages, and intakes for any specific project.

**Q: How do I see all the projects currently active in my workspace?**
Simply use the `list_projects` tool by providing your workspace slug. The agent will return a list of all projects, including their names and identifiers.

**Q: Is it possible to archive a project that is no longer needed?**
Yes, you can use the `archive_project` tool to move a project to the archive. If you change your mind, you can also use `unarchive_project` to bring it back.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plane-alternative](https://vinkius.com/mcp/plane-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plane** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `plane-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plane** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plane-alternative": {
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
