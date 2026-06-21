# ZenHub MCP Server

Manage agile boards, epics, and estimates via the ZenHub API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zenhub)

## Overview
**Category:** developer-tools
**Tools Count:** 8

## Description
Connect your **ZenHub** account to any AI agent to streamline your agile project management on GitHub. This MCP server enables your agent to interact with pipelines, issues, estimates, and epics directly from natural language.

### What you can do

- **Board Visibility** — List all pipelines and issues for specific GitHub repositories or ZenHub workspaces
- **Agile Status Management** — Move issues between pipelines to update their workflow status instantly
- **Precision Estimating** — Set and retrieve story point estimates for any GitHub issue
- **Epic Oversight** — List and inspect ZenHub epics and their constituent issues
- **Release Tracking** — Access release reports and progress metadata for your projects

### How it works

1. Subscribe to this server
2. Enter your ZenHub API Token
3. Start managing your agile workflow from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Engineers** — Quickly update issue status and estimates from your IDE
- **Project Managers** — Monitor board health and epic progress via natural language commands
- **Scrum Masters** — Facilitate planning by querying release reports and team velocity metrics


## Available Tools
- **get_repo_board**: Get the ZenHub board for a repository
- **get_epic_data**: Get details for a specific epic
- **list_repo_epics**: List all ZenHub epics for a repository
- **set_issue_estimate**: Set the story point estimate for an issue
- **get_zenhub_issue_data**: Get ZenHub-specific metadata for a GitHub issue
- **move_issue_between_pipelines**: Move an issue to a different pipeline
- **list_release_reports**: List release reports for a repository
- **get_workspace_board**: Get the ZenHub board for a specific workspace and repository


## Installation & Usage

To install and use the **ZenHub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zenhub](https://vinkius.com/mcp/zenhub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
