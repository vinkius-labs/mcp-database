# Azure DevOps MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/azure-devops)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/azure-devops-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/azure-devops-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage work items, track builds, and coordinate releases across your Azure DevOps organization with full pipeline visibility.

## Description
Connect your **Azure DevOps** account to any AI agent and simplify how you manage your software development lifecycle, track work items, and monitor pipelines through natural conversation.

### What you can do

- **Project Oversight** — List all projects in your organization and retrieve detailed metadata and configurations.
- **Work Item Tracking** — List and query recent tasks, bugs, and user stories to manage your team's backlog.
- **Git Repository Control** — Query all Git repositories within a project to monitor code storage.
- **Pipeline Monitoring** — List CI/CD pipelines and retrieve the history of recent build executions and statuses.
- **Team Coordination** — List project teams to understand organizational structure and distribution.
- **Operational Status** — Fetch real-time metadata for projects and work items directly via AI commands.

### How it works

1. Subscribe to this server
2. Enter your Azure DevOps Organization and Personal Access Token (PAT)
3. Start managing your DevOps ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers & Engineers** — quickly check pipeline statuses and verify work item details via simple AI queries.
- **DevOps Specialists** — monitor build history and manage repositories directly from the workspace.
- **Product Owners** — get instant bird's-eye views of work item progress and project health via the AI assistant.


## Available Tools
- **list_builds**: List recent builds
- **list_pipelines**: List CI/CD pipelines
- **list_projects**: List Azure DevOps projects
- **list_repositories**: List Git repositories
- **list_project_teams**: List teams in a project
- **list_work_items**: List recent work items


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Azure DevOps** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in my Azure DevOps organization."

**🤖 AI Agent:**
> I've retrieved your projects. You have access to: 'Mobile App', 'Internal Tools', and 'Infrastructure-as-Code'. Which one would you like to see work items for?

---

**👤 You:**
> "Show me the last 5 work items for the 'Mobile App' project."

**🤖 AI Agent:**
> I've fetched the work items. There are 5 recent items including 'Bug #8823: Login crash', 'Story #8824: Add dark mode', and 'Task #8825: Update SDK'. Would you like more details on the login crash?

---

**👤 You:**
> "What is the status of the latest build for project 'Internal Tools'?"

**🤖 AI Agent:**
> Retrieving build history... The latest build for 'Internal Tools' (ID: 10293) was 'Succeeded' 2 hours ago. It was triggered by Mike Ross on the 'main' branch.


## Installation & Usage

To install and use the **Azure DevOps** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/azure-devops](https://vinkius.com/mcp/azure-devops)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
