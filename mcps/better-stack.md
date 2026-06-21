# Better Stack MCP Server

Monitor uptime and incidents via Better Stack — list monitors, heartbeats, and on-call schedules directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/better-stack)

## Overview
**Category:** ship-it
**Tools Count:** 10

## Description
Connect your **Better Stack (formerly Better Uptime)** account to any AI agent and orchestrate your infrastructure monitoring and incident management through natural conversation.

### What you can do

- **Uptime Monitoring** — List, create, and manage all your HTTP, Ping, and Keyword monitors to ensure service availability.
- **Incident Response** — Retrieve real-time updates on active incidents and historical reports for post-mortems.
- **On-Call Coordination** — Access on-call schedules and rotations to see who is responsible for system health.
- **Heartbeat Management** — Monitor cron jobs and recurring tasks through heartbeat monitors.
- **Status Page Oversight** — List and verify your public status pages directly from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Better Stack API Token
3. Start monitoring your infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & SREs** — quickly check monitor statuses and incident details during an outage without manual dashboard navigation.
- **Backend Developers** — verify heartbeat logs for cron jobs straight from their code editor.
- **Engineering Managers** — retrieve on-call summaries and incident history for reporting.


## Available Tools
- **create_monitor**: Create a new uptime monitor
- **delete_monitor**: Delete a monitor
- **get_incident**: Get details of a specific incident
- **get_monitor**: Get specific monitor details
- **list_heartbeats**: List all heartbeat monitors
- **list_incidents**: List recent uptime incidents
- **list_monitors**: List all uptime monitors
- **list_on_calls**: List on-call schedules and rotations
- **list_status_pages**: List public status pages
- **update_monitor**: Update an existing monitor


## Installation & Usage

To install and use the **Better Stack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/better-stack](https://vinkius.com/mcp/better-stack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
