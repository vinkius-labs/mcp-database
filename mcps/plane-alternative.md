# Plane MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plane-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/plane-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/plane-alternative-mcp)
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


## Installation & Usage

To install and use the **Plane** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plane-alternative](https://vinkius.com/mcp/plane-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
