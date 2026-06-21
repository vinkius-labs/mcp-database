# GitScrum MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gitscrum)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gitscrum-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gitscrum-mcp)
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


## Available Tools
- **list_labels**: List labels in a project
- **get_me**: Get authenticated user profile
- **list_project_members**: List members in a project
- **my_role**: Get my role in the workspace
- **create_project**: Create a new project
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


## Installation & Usage

To install and use the **GitScrum** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gitscrum](https://vinkius.com/mcp/gitscrum)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
