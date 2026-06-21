# Trigger.dev (Background Tasks & Jobs) MCP Server

Manage background tasks and jobs via Trigger.dev — trigger tasks, monitor runs, manage schedules, and configure environment variables directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/triggerdev-background-tasks-jobs)

## Overview
**Category:** developer-tools
**Tools Count:** 19

## Description
Connect your **Trigger.dev** account to any AI agent to orchestrate complex background workflows and monitor job execution through natural language.

### What you can do

- **Task Orchestration** — Trigger individual tasks or batch up to 1,000 tasks in a single request using `trigger_task` and `batch_trigger_tasks`.
- **Run Monitoring** — Retrieve detailed status, payloads, and outputs for specific runs with `get_run`, or list runs with advanced filtering using `list_runs`.
- **Lifecycle Management** — Cancel in-progress runs, replay failed executions, and update run metadata for real-time progress tracking.
- **Scheduling** — Create and manage imperative cron schedules to automate recurring tasks with `create_schedule`.
- **Environment Control** — Manage environment variables and control queue concurrency or pause/resume operations directly via the API.

### How it works

1. Subscribe to this server
2. Enter your Trigger.dev Secret Key
3. Start managing your background jobs from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Backend Engineers** — monitor and debug production jobs without leaving the terminal or IDE.
- **DevOps Teams** — automate task triggers and manage environment configurations via chat.
- **Product Managers** — check the status of critical data processing runs or batch operations.


## Available Tools
- **batch_trigger_tasks**: Trigger multiple tasks in a single request
- **cancel_run**: Cancel an in-progress run
- **complete_waitpoint**: Complete a waitpoint
- **create_batch**: Create a batch (Phase 1)
- **create_env_var**: Create an environment variable
- **create_schedule**: Create an IMPERATIVE schedule (cron)
- **create_waitpoint_token**: Create a waitpoint token
- **delete_env_var**: Delete an environment variable
- **get_batch_results**: Retrieve batch results
- **get_run**: Retrieve a specific run
- **list_env_vars**: List environment variables
- **list_runs**: List runs in an environment
- **list_schedules**: List schedules
- **override_queue_concurrency**: Override queue concurrency
- **pause_resume_queue**: Pause or resume a queue
- **replay_run**: Replay a run
- **trigger_task**: dev.

Trigger a task by its identifier
- **update_env_var**: Update an environment variable
- **update_run_metadata**: Update run metadata


## Installation & Usage

To install and use the **Trigger.dev (Background Tasks & Jobs)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/triggerdev-background-tasks-jobs](https://vinkius.com/mcp/triggerdev-background-tasks-jobs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
