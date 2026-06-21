# QStash (Serverless Message Queue) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qstash-serverless-message-queue)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage serverless messaging, task scheduling, and webhooks via Upstash QStash — publish messages, manage queues, and handle DLQs directly.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **QStash (Serverless Message Queue)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Publish a POST request to https://api.example.com/webhook with a 1-hour delay."

**🤖 AI Agent:**
> I've published the message to your destination. It is scheduled for delivery in 1 hour. Message ID: msg_82391.

---

**👤 You:**
> "List all my current QStash queues and their status."

**🤖 AI Agent:**
> I found 3 queues: 'image-processing' (Active), 'email-service' (Paused), and 'webhooks-main' (Active).

---

**👤 You:**
> "Check the Dead Letter Queue and retry the message with ID msg_123."

**🤖 AI Agent:**
> I've located the message in the DLQ and successfully triggered a retry for msg_123.


## ❓ FAQ

**Q: How can I schedule a message to be sent later?**
Use the `publish_message` tool and provide the `delay` parameter (e.g., '10m' for 10 minutes) or a `not_before` Unix timestamp.

**Q: What happens if a message fails all retry attempts?**
The message is moved to the Dead Letter Queue (DLQ). You can use `list_dlq` to find it and `retry_dlq_message` to attempt delivery again.

**Q: Can I manage recurring tasks like cron jobs?**
Yes! You can use `list_schedules` to see existing ones, and `pause_schedule` or `resume_schedule` to control them.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qstash-serverless-message-queue](https://vinkius.com/mcp/qstash-serverless-message-queue)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **QStash (Serverless Message Queue)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `qstash-serverless-message-queue` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **QStash (Serverless Message Queue)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "qstash-serverless-message-queue": {
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
