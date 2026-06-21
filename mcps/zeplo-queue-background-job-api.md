# Zeplo (Queue & Background Job API) MCP Server

Schedule, queue, and manage background jobs and webhooks via Zeplo directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zeplo-queue-background-job-api)

## Overview
**Category:** developer-tools
**Tools Count:** 17

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


## Installation & Usage

To install and use the **Zeplo (Queue & Background Job API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zeplo-queue-background-job-api](https://vinkius.com/mcp/zeplo-queue-background-job-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
