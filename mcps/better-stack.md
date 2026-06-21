# Better Stack MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/better-stack)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/better-stack-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/better-stack-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Monitor uptime and incidents via Better Stack — list monitors, heartbeats, and on-call schedules directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Better Stack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all monitors that are currently down."

**🤖 AI Agent:**
> I've checked your monitors. Currently, 2 services are down: 'Primary API' (ID: mon_123) and 'Auth Gateway' (ID: mon_456). Would you like to see the incident details for these?

---

**👤 You:**
> "Show me the on-call schedule for this week."

**🤖 AI Agent:**
> Retrieving on-call data... For the 'Core Infrastructure' rotation, Sarah Miller is on-call until Friday, and John Doe will take over for the weekend.

---

**👤 You:**
> "Check status of heartbeat 'daily-backup'."

**🤖 AI Agent:**
> The heartbeat 'daily-backup' (ID: hb_992) is currently healthy. Its last ping was received 2 hours ago, which is within the expected 24-hour window.


## Installation & Usage

To install and use the **Better Stack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/better-stack](https://vinkius.com/mcp/better-stack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
