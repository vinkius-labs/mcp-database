# DVC MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dvc)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dvc-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dvc-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage ML experiments via DVC — track projects and views, audit experiments history, and monitor model runs directly from any AI agent.

## Description
Connect your **DVC Studio** account to any AI agent and take full control of your machine learning experiments and data versioning workflows through natural conversation.

### What you can do

- **Project Orchestration** — Expose registered organization workspaces and validate available physical repositories connected within DVC Studio limits
- **Experiment Navigation** — Iterate through explicitly generated model runs mapping precise metric arrays and discovering logged metrics history cleanly
- **View Management** — Extract explicit UI configuration layouts and dashboard settings to retrieve structural workspace representations natively
- **Repository Auditing** — Analyze specific identifier boundaries resolving internal team mappings and parsing direct repository metadata constraints
- **Metric Inspection** — Retrieve complex structural arrays defining precisely which metrics were captured during specific experiment epochs
- **Identity Oversight** — Identify the exact authorized token holder exposing mapping roles and organization scopes dynamically to verify permissions

### How it works

1. Subscribe to this server
2. Enter your DVC Studio Client Access Token (found in DVC Studio Profile Settings > Tokens)
3. Start managing your ML experiments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists** — monitor model experiments and track metrics without leaving the development environment
- **ML Engineers** — verify project repository connections and audit model run histories using natural language
- **Team Leads** — monitor organization workspaces and experiment progress through natural conversation
- **DevOps Engineers** — test and debug DVC Studio integrations and verify access token permissions in real-time


## Available Tools
- **list_views**: List views
- **get_view**: Get view
- **list_projects**: List projects
- **get_project**: Get project
- **list_experiments**: List experiments
- **get_user**: Get user profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DVC** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all projects in my DVC Studio account"

**🤖 AI Agent:**
> I found 3 projects: 'Credit-Scoring-Model', 'Image-Classification-V2', and 'NLP-Pipeline'. Which one would you like to explore for experiments?

---

**👤 You:**
> "Show me the last 5 experiments for project 'Credit-Scoring-Model'"

**🤖 AI Agent:**
> Retrieving experiments... I found 5 recent runs. The best one achieved an accuracy of 0.94 (ID: exp-a1b2). The most recent run finished 10 minutes ago with an accuracy of 0.92 (ID: exp-c3d4).

---

**👤 You:**
> "What are my dashboard views in DVC?"

**🤖 AI Agent:**
> Retrieving views... You have 2 active dashboard layouts: 'Main-Metrics-Grid' and 'Validation-Plots'. Would you like the detailed settings for either of them?


## Installation & Usage

To install and use the **DVC** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dvc](https://vinkius.com/mcp/dvc)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
