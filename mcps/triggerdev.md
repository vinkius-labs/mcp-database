# Trigger.dev MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/triggerdev)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/triggerdev-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/triggerdev-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Equip your AI agent with direct access to Trigger.dev — manage background jobs, monitor task runs, and inspect workflow executions without opening the dashboard.

## Description
Connect **Trigger.dev** to your AI agent and manage your background job infrastructure conversationally.

### What you can do

- **Job Monitoring** — List active, completed, and failed task runs with execution times, statuses, and error details.
- **Project Overview** — Query projects, environments, and their associated job definitions.
- **Run Inspection** — Drill into individual runs to view payloads, outputs, logs, and retry history.
- **Environment Management** — Switch between dev, staging, and production environments to inspect runs across your deployment pipeline.

### How it works

1. Subscribe to the Trigger.dev integration on the marketplace.
2. Generate a Secret API Key from your Trigger.dev dashboard (Project → API Keys section — keys start with `tr_dev_` or `tr_prod_`).
3. Ask your AI agent to list job runs, check failures, or inspect task outputs.

### Who is this for?

- **Backend Developers** — Monitor background job health, debug failed runs, and verify task outputs without leaving your code editor.
- **DevOps Engineers** — Track job execution across environments and identify bottlenecks in your processing pipeline.
- **Technical Leads** — Get instant visibility into production job queues during incident response without switching to the Trigger.dev dashboard.


## Available Tools
- **list_projects**: List all projects
- **list_runs**: List task runs
- **get_run**: Get run details
- **trigger_task**: Trigger a background task
- **cancel_run**: Cancel a running task
- **replay_run**: Replay a completed task
- **list_schedules**: List cron schedules
- **list_environments**: List deployment environments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Trigger.dev** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Are there any failed background jobs in production?"

**🤖 AI Agent:**
> I found 2 failed runs in the last 24 hours: 'process-webhook' failed with a timeout error (3 retries exhausted) and 'sync-inventory' failed due to a database connection error. Both occurred between 3:00-3:15 AM UTC.

---

**👤 You:**
> "Show me the details of the last 'process-webhook' run."

**🤖 AI Agent:**
> Run ID: run_abc123. Status: FAILED. Duration: 30.2s (timeout at 30s). Error: 'Request timeout after 30000ms at postWebhook step'. Input payload: {event: 'order.created', id: 'ord_xyz'}. Retries: 3/3 exhausted.

---

**👤 You:**
> "How many jobs ran successfully today?"

**🤖 AI Agent:**
> Today's stats: 1,247 total runs — 1,238 successful (99.3%), 7 failed (0.6%), and 2 currently running. Average execution time: 2.4 seconds. Most active task: 'process-order' with 892 runs.


## Installation & Usage

To install and use the **Trigger.dev** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/triggerdev](https://vinkius.com/mcp/triggerdev)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
