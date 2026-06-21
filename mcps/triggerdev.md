# Trigger.dev MCP Server

Equip your AI agent with direct access to Trigger.dev — manage background jobs, monitor task runs, and inspect workflow executions without opening the dashboard.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/triggerdev)

## Overview
**Category:** ship-it
**Tools Count:** 8

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


## Installation & Usage

To install and use the **Trigger.dev** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/triggerdev](https://vinkius.com/mcp/triggerdev)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
