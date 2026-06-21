# ntfy (Push Notifications) MCP Server

Send and receive push notifications via ntfy topics directly from your AI agent to any device.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ntfy-push-notifications)

## Overview
**Category:** productivity
**Tools Count:** 2

## Description
Connect your **ntfy** instance to any AI agent and manage real-time alerts and notifications through natural conversation. ntfy is an HTTP-based pub-sub service that allows you to send notifications to your phone or desktop via scripts or APIs.

### What you can do

- **Instant Publishing** — Send messages to any ntfy topic with custom titles, priorities, and tags (emojis).
- **Message Polling** — Retrieve cached messages from a topic to stay updated on previous alerts or system logs.
- **Rich Notifications** — Attach clickable URLs, custom icons, and even files to your push notifications.
- **Scheduled Alerts** — Use the delay parameter to schedule notifications for the future.
- **Advanced Formatting** — Send notifications with Markdown support for better readability on supported clients.

### How it works

1. Subscribe to this server
2. Enter your ntfy instance URL (e.g., `https://ntfy.sh`) and an optional access token
3. Start sending alerts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — Automate deployment alerts and system monitoring notifications directly from the terminal or IDE.
- **Developers** — Send debugging info or long-running task completions to your phone.
- **Power Users** — Create custom workflows that bridge AI agents with mobile push notifications without complex setups.


## Available Tools
- **poll_messages**: Poll cached messages from a ntfy topic
- **publish_message**: Topics are created on the fly.

Publish a push notification to a ntfy topic


## Installation & Usage

To install and use the **ntfy (Push Notifications)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ntfy-push-notifications](https://vinkius.com/mcp/ntfy-push-notifications)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
