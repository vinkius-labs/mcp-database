# Trigger.dev (Background Tasks & Jobs) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/triggerdev-background-tasks-jobs)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage background tasks and jobs via Trigger.dev — trigger tasks, monitor runs, manage schedules, and configure environment variables directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Trigger.dev (Background Tasks & Jobs)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Trigger the 'image-processing' task with payload { 'url': 'https://example.com/img.jpg' }."

**🤖 AI Agent:**
> Task triggered successfully. Run ID: run_abc123. Status: QUEUED. You can check its progress using get_run.

---

**👤 You:**
> "List the last 5 failed runs for the 'sync-data' task."

**🤖 AI Agent:**
> I've found 5 failed runs for 'sync-data'. The most recent failure (ID: run_xyz789) occurred at 10:30 AM with error: 'Connection Timeout'. Would you like to replay it?

---

**👤 You:**
> "Create a daily schedule for the 'cleanup-logs' task at midnight."

**🤖 AI Agent:**
> Schedule created for 'cleanup-logs' with cron '0 0 * * *'. Deduplication key: 'daily-cleanup-logs'. The task will now run automatically every day at midnight UTC.


## ❓ FAQ

**Q: Can I trigger multiple background tasks at once?**
Yes! You can use the `batch_trigger_tasks` tool to trigger up to 1,000 tasks in a single batch request, which is highly efficient for high-volume workflows.

**Q: How do I check the output or error of a specific job run?**
Use the `get_run` tool with the specific Run ID. It will return the full status, payload, output, and any attempt details or error logs associated with that run.

**Q: Can I schedule a task to run automatically using a cron expression?**
Absolutely. Use the `create_schedule` tool to define a task identifier, a cron expression (e.g., '0 0 * * *'), and a deduplication key to automate recurring background jobs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/triggerdev-background-tasks-jobs](https://vinkius.com/mcp/triggerdev-background-tasks-jobs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Trigger.dev (Background Tasks & Jobs)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `triggerdev-background-tasks-jobs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Trigger.dev (Background Tasks & Jobs)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "triggerdev-background-tasks-jobs": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
