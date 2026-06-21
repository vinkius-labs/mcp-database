# Anaplan MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/anaplan)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/anaplan-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/anaplan-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage Anaplan workspaces, models, and data actions (imports, exports, processes) directly via AI.

## Description
Connect your **Anaplan** account to your AI agent to automate financial planning, supply chain, and sales operations. This MCP server allows you to discover workspaces and models, and trigger complex data integration tasks using natural language.

### What you can do

- **Workspace & Model Discovery** — List all available workspaces and models to navigate your planning environment.
- **Execute Data Actions** — Trigger and monitor imports, exports, and processes (groups of actions) to move data in and out of Anaplan.
- **Task Monitoring** — Real-time tracking of asynchronous task statuses to ensure your data integrations complete successfully.
- **File Management** — List files within your models to keep track of historical imports and exports.

### How it works

1. Subscribe to this server
2. Provide your Anaplan Auth Token
3. Start managing your Anaplan environment directly through your AI chat interface.

### Who is this for?

- **FP&A Analysts** — Automate the triggering of planning processes and exports without manual intervention.
- **Supply Chain Managers** — Quickly run data imports for inventory updates via chat.
- **Operations Teams** — Monitor the status of long-running data syncs directly from your workspace.


## Available Tools
- **get_task_status**: Get status of a running task
- **list_exports**: List export actions for a model
- **list_files**: List files in a model (exports/imports)
- **list_imports**: List import actions for a model
- **list_models**: List Anaplan models. Optionally filter by workspaceId
- **list_processes**: List processes for a model
- **list_workspaces**: List available Anaplan workspaces
- **run_export**: Run an Anaplan export action
- **run_import**: Run an Anaplan import action
- **run_process**: Run an Anaplan process


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Anaplan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Anaplan workspaces and models."

**🤖 AI Agent:**
> I've retrieved your Anaplan environment. You have 2 workspaces: 'Finance_Production' (ID: abc...) and 'Supply_Chain_Test' (ID: def...). Within 'Finance_Production', there are 3 models available.

---

**👤 You:**
> "Run the 'Monthly Actuals' import in the Finance workspace."

**🤖 AI Agent:**
> I've started the 'Monthly Actuals' import task (ID: task_123). I will monitor the status for you. Currently, it is 'IN_PROGRESS'.

---

**👤 You:**
> "What's the status of the process task 'p_456'?"

**🤖 AI Agent:**
> The process task 'p_456' has completed successfully. All 3 sub-actions within the process were finished without errors.


## Installation & Usage

To install and use the **Anaplan** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/anaplan](https://vinkius.com/mcp/anaplan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
