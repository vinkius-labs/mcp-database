# Better Stack MCP Server

Automate incident management via Better Stack — monitor uptime, manage incidents, and control on-call schedules securely from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/better-stack-1)

## Overview
**Category:** ship-it
**Tools Count:** 10

## Description
Connect your **Better Stack (Better Uptime)** account to any AI agent and empower it to act as your Level 1 Site Reliability Engineer (SRE). Let your AI diagnose incidents, manage escalations, and audit monitoring configs securely via conversation.

### What you can do

- **Incident Response** — Rapidly list firing incidents, inspect technical downtime payloads, acknowledge alerts, and force resolve states inline
- **Uptime Monitors** — Fetch exact definitions of active HTTP endpoint pings, DNS probes, and latency constraints across your fleet
- **Cron Heartbeats** — Investigate passive tracking endpoints validating background workers and server limits
- **On-Call Management** — Expose active shifts and team schedules to determine explicitly who is getting paged in real-time
- **Status Pages** — Read configured public dashboards tracking your global infrastructure

### How it works

1. Subscribe to this server
2. Enter your Better Stack API Token
3. Empower Claude, Cursor, or your preferred agent to respond to alerts interactively

Stop switching context between your terminal and incident dashboards during critical outages.

### Who is this for?

- **DevOps & SREs** — audit on-call matrices safely, track firing pages, and orchestrate initial debugging workflows without leaving chat
- **Engineering Managers** — review recent downtime timelines and resolve dormant alerts quickly
- **Backend Developers** — rapidly debug failing cron heartbeats while simultaneously patching code


## Available Tools
- **list_monitors**: List all monitors on Better Stack (Better Uptime)
- **get_monitor**: Get full details of a specific Better Stack monitor
- **list_incidents**: List all explicit incidents on Better Stack
- **get_incident**: Retrieve the native timeline payload of an explicit incident
- **acknowledge_incident**: Acknowledge an ongoing explicit incident halting paging
- **resolve_incident**: Force resolve a specific incident
- **list_heartbeats**: List all configured cron heartbeats securely
- **get_heartbeat**: Get explicit details of a passive heartbeat node
- **list_status_pages**: List all explicit Status Pages
- **list_on_call**: List exact On-Call routing calendars


## Installation & Usage

To install and use the **Better Stack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/better-stack-1](https://vinkius.com/mcp/better-stack-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
