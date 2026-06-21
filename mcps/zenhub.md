# ZenHub MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zenhub)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zenhub-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zenhub-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage agile boards, epics, and estimates via the ZenHub API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ZenHub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the ZenHub board for repository ID '12345678'."

**🤖 AI Agent:**
> I've retrieved the ZenHub board for repository 12345678. You have 5 pipelines: 'New Issues', 'Backlog', 'In Progress', 'Review/QA', and 'Done'. Would you like to see the issues in a specific pipeline?

---

**👤 You:**
> "Move issue #45 in repo '12345678' to the 'In Progress' pipeline (ID: '56789') in workspace '98765'."

**🤖 AI Agent:**
> Successfully moved issue #45 to the 'In Progress' pipeline in your ZenHub workspace.

---

**👤 You:**
> "What are the estimates for all issues in the current epic?"

**🤖 AI Agent:**
> For the current epic, I found 8 issues. Total estimated points: 34. Current distribution: 3 issues (8 pts), 2 issues (5 pts), 3 issues (3 pts).


## Installation & Usage

To install and use the **ZenHub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zenhub](https://vinkius.com/mcp/zenhub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
