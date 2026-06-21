# Healthchecks.io MCP Server

Monitor cron jobs and background tasks via Healthchecks.io — list checks, track pings, and manage alerts directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/healthchecksio)

## Overview
**Category:** developer-tools
**Tools Count:** 13

## Description
Connect your **Healthchecks.io** account to any AI agent to monitor and manage your cron jobs, background tasks, and scheduled services through natural conversation.

### What you can do

- **Check Management** — List, create, update, and delete monitoring checks for your infrastructure
- **Ping History** — Inspect recent pings and payloads to debug failed tasks or verify successful executions
- **Status Monitoring** — Pause or resume checks and track status 'flips' (up/down transitions) over time
- **Integration Overview** — List configured notification channels to ensure your team is alerted correctly
- **Deep Inspection** — Fetch specific check metadata and ping bodies to understand exactly why a service is failing

### How it works

1. Subscribe to this server
2. Enter your Healthchecks.io API Key
3. Start monitoring your background jobs from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly verify the health of scheduled tasks and investigate downtime without leaving the terminal
- **Software Developers** — check if background workers are running correctly during development and debugging
- **SRE Teams** — automate the auditing of monitoring coverage and integration status


## Available Tools
- **create_check**: Use the unique field to upsert if it already exists.

Create a new check
- **delete_check**: Delete a check
- **get_check**: Get a single check by UUID or unique key
- **get_ping_body**: Get the body of a specific ping
- **get_status**: Check the Healthchecks.io service status
- **list_badges**: io status badges.

List all status badges for the project
- **list_checks**: Can be filtered by tags or slug.

List all checks in the project
- **list_flips**: List status changes (flips) for a check
- **list_integrations**: List all integrations (channels) in the project
- **list_pings**: List recent pings for a check
- **pause_check**: Pause a check
- **resume_check**: Resume a check
- **update_check**: Update an existing check


## Installation & Usage

To install and use the **Healthchecks.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/healthchecksio](https://vinkius.com/mcp/healthchecksio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
