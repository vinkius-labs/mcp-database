# QStash (Serverless Message Queue) MCP Server

Manage serverless messaging, task scheduling, and webhooks via Upstash QStash — publish messages, manage queues, and handle DLQs directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/qstash-serverless-message-queue)

## Overview
**Category:** developer-tools
**Tools Count:** 38

## Description
Connect your **Upstash QStash** account to any AI agent to orchestrate serverless messaging and background tasks through natural language.

### What you can do

- **Message Publishing** — Send messages to URLs or URL Groups with custom delays, retries, and deduplication via `publish_message`.
- **Queue Management** — Create and manage FIFO queues with controlled parallelism for reliable task processing using `upsert_queue` and `list_queues`.
- **Scheduling** — List, pause, and resume cron-based schedules for recurring background jobs with `list_schedules`.
- **DLQ Handling** — Inspect and retry failed messages in the Dead Letter Queue to ensure no data loss using `list_dlq` and `retry_dlq_message`.
- **Flow Control** — Monitor and adjust rate limits and parallelism across your messaging infrastructure with `list_flow_control_keys`.

### How it works

1. Subscribe to this server
2. Enter your QStash Token from the Upstash Console
3. Start orchestrating your serverless workflows from Claude, Cursor, or any MCP-compatible client.

### Who is this for?

- **Backend Developers** — trigger webhooks and background jobs directly from the code editor.
- **DevOps Engineers** — monitor message queues, logs, and DLQs without leaving the terminal or chat.
- **System Architects** — design and test complex messaging workflows using natural language commands.


## Available Tools
- **batch_messages**: Send multiple messages in a single request
- **bulk_cancel_messages**: Cancel multiple messages based on filters
- **bulk_delete_dlq**: Delete all messages from the DLQ
- **bulk_retry_dlq**: Retry all messages in the DLQ
- **cancel_message**: Stop a pending message from being delivered
- **delete_dlq_message**: Delete a message from the DLQ
- **delete_queue**: Delete a queue
- **delete_schedule**: Delete a schedule
- **delete_url_group**: Delete a URL Group
- **enqueue_message**: Add a message to a specific queue for FIFO or controlled parallelism
- **get_dlq_message**: Get details of a specific DLQ message
- **get_flow_control_key**: Get details of a specific flow control key
- **get_global_parallelism**: Get global parallelism configuration
- **get_keys**: Retrieve QStash signing keys
- **get_message**: Retrieve details of a message currently in flight or being retried
- **get_queue**: Get details of a specific queue
- **get_schedule**: Get details of a specific schedule
- **get_url_group**: Get details of a specific URL Group
- **list_dlq**: List messages in the Dead Letter Queue (DLQ)
- **list_flow_control_keys**: List all flow control keys
- **list_logs**: Retrieve QStash logs/events
- **list_queues**: List all queues
- **list_schedules**: List all schedules
- **list_url_groups**: List all URL Groups (Topics)
- **pause_flow_control**: Pause a flow control key
- **pause_queue**: Pause a queue
- **pause_schedule**: Pause a schedule
- **pin_flow_control**: Pin configuration for a flow control key
- **publish_message**: Publish a message to a destination URL or URL Group
- **remove_endpoints**: Remove endpoints from a URL Group
- **reset_flow_control_rate**: Reset the rate limit for a flow control key
- **resume_flow_control**: Resume a paused flow control key
- **resume_queue**: Resume a paused queue
- **resume_schedule**: Resume a paused schedule
- **retry_dlq_message**: Retry a message from the DLQ
- **unpin_flow_control**: Unpin configuration for a flow control key
- **upsert_queue**: Create or update a queue
- **upsert_url_group**: Create or update a URL Group (Topic)


## Installation & Usage

To install and use the **QStash (Serverless Message Queue)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qstash-serverless-message-queue](https://vinkius.com/mcp/qstash-serverless-message-queue)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
