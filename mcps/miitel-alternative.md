# MiiTel MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/miitel-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/miitel-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/miitel-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Automate MiiTel voice intelligence — list export queues, generate CSVs, and import call or meeting records via AI.

## Description
Connect your **MiiTel** account to any AI agent to streamline your voice intelligence workflows. This server allows you to manage call and meeting histories, generate data exports, and import external records directly through natural language.

### What you can do

- **Data Exporting** — List and create CSV generation queues for comprehensive call and meeting history analysis.
- **Call Integration** — Import call history and audio data from external phone systems into MiiTel using webhooks.
- **Meeting Management** — Create meeting records in MiiTel Meetings with full participant and host metadata.
- **Queue Monitoring** — Track the status of your data export processes (Waiting, Processing, Completed, or Error).

### How it works

1. Subscribe to this server
2. Enter your MiiTel Tenant Code and API credentials
3. Start managing your voice data from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales Operations** — automate the export of call logs for CRM synchronization and performance analysis.
- **Data Analysts** — programmatically trigger CSV generations to feed business intelligence dashboards.
- **Support Teams** — centralize external telephony records into the MiiTel ecosystem for a unified view of customer interactions.


## Available Tools
- **create_call_record**: Create a call record via Incoming Webhook
- **create_meeting_record**: Create a meeting record via Incoming Webhook
- **create_queue**: Create a new CSV generation queue
- **list_queues**: List CSV generation queues


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MiiTel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my recent CSV export queues and their status."

**🤖 AI Agent:**
> I've retrieved your export queues. You have 3 recent requests: 2 are COMPLETED and 1 is currently PROCESSING. Would you like the details for the completed ones?

---

**👤 You:**
> "Create a new CSV export queue for meeting history."

**🤖 AI Agent:**
> I've initiated the `create_queue` action for a VIDEO_HISTORY_CSV_LIST. The process is now in the WAITING state. I'll let you know when it's ready.

---

**👤 You:**
> "Import a call record with ID 'webhook-123' for a call that ended at 2023-10-27T10:00:00Z."

**🤖 AI Agent:**
> I've successfully sent the call data to MiiTel using the `create_call_record` tool. The record is now being processed in your tenant.


## Installation & Usage

To install and use the **MiiTel** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/miitel-alternative](https://vinkius.com/mcp/miitel-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
