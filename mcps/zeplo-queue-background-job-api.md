# Zeplo (Queue & Background Job API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zeplo-queue-background-job-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Schedule, queue, and manage background jobs and webhooks via Zeplo directly from your AI agent.

## Description
Connect your **Zeplo** account to any AI agent to orchestrate background tasks, webhooks, and scheduled jobs through natural language.

### What you can do

- **Job Enqueueing** — Send HTTP requests to be processed in the background with automatic retries and delay options.
- **Scheduling** — Create CRON-like schedules or one-off delayed executions for your API endpoints.
- **Job Monitoring** — Retrieve the status, payload, and response data of any job using its unique ID.
- **Queue Management** — List recent jobs, filter by status (success, failure, pending), and manage your processing pipeline.
- **Lifecycle Control** — Cancel pending jobs or manually trigger retries for failed tasks without touching code.

### How it works

1. Subscribe to this server
2. Enter your Zeplo API Key
3. Start managing your serverless queues from Claude, Cursor, or any MCP-compatible client

No more checking dashboards to see why a webhook failed. Your AI can now monitor your background infrastructure and fix issues in real-time.

### Who is this for?

- **Backend Developers** — quickly enqueue test jobs and check execution logs directly from the terminal or IDE.
- **DevOps Engineers** — monitor queue health and retry failed production jobs using natural language commands.
- **Product Teams** — automate scheduled reports or notifications by asking the AI to set up Zeplo schedules.


## Available Tools
- **cancel_request**: Cancel a pending or scheduled request
- **create_queue**: Create a new queue
- **create_schedule**: Create a new schedule
- **create_token**: The token value is only returned once.

Create a new token for a workspace
- **delete_queue**: Delete a queue
- **delete_schedule**: Delete a schedule
- **enqueue_request**: Resolves queue from token.

Enqueue a new HTTP request
- **get_queue**: Get queue details and metrics
- **get_request**: Get request details and timeline
- **invite_team_member**: Invite a new member to the workspace team
- **list_queue_logs**: Get paginated request history for a queue
- **list_queues**: List queues in a workspace
- **list_schedules**: List schedules in a workspace
- **list_team**: List team members in a workspace
- **list_tokens**: List tokens in a workspace
- **update_queue**: Update a queue
- **update_schedule**: Update, pause, or resume a schedule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zeplo (Queue & Background Job API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Enqueue a POST request to https://api.myapp.com/sync with the JSON payload { "user_id": 123 }."

**🤖 AI Agent:**
> I've enqueued the job on Zeplo. The Job ID is `zeplo_abc123`. It is currently pending and will be executed immediately with automatic retries if it fails.

---

**👤 You:**
> "List the last 5 failed jobs and tell me why they failed."

**🤖 AI Agent:**
> I found 5 failed jobs. The most recent one (`zeplo_987`) failed because the endpoint returned a 500 Internal Server Error. The others failed due to timeout. Would you like me to retry any of them?

---

**👤 You:**
> "Schedule a GET request to https://api.service.com/health to run every hour."

**🤖 AI Agent:**
> I have created a schedule on Zeplo for that endpoint. It will trigger every hour starting now. You can monitor the executions using the `list_jobs` tool.


## ❓ FAQ

**Q: Can I schedule a job to run at a specific time in the future?**
Yes! Use the `enqueue_job` tool and specify a delay or a schedule parameter. You can tell the AI 'Schedule this request for tomorrow at 10am' and it will handle the timestamp conversion for Zeplo.

**Q: How do I check why a specific background job failed?**
You can use the `get_job` tool with the Job ID. The AI will retrieve the full execution log, including the response body and status code from your endpoint, helping you debug the failure instantly.

**Q: Is it possible to cancel a job that hasn't run yet?**
Absolutely. Use the `cancel_job` tool with the target Job ID. This is useful for stopping scheduled tasks or queued jobs that are no longer necessary.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zeplo-queue-background-job-api](https://vinkius.com/mcp/zeplo-queue-background-job-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zeplo (Queue & Background Job API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zeplo-queue-background-job-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zeplo (Queue & Background Job API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zeplo-queue-background-job-api": {
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
