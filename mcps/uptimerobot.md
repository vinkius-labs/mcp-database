# UptimeRobot MCP Server

Monitor and manage your website uptime seamlessly. List, create, and resolve monitor alerts directly from your AI agent, 24/7.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/uptimerobot)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 10

## Description
Connect your **UptimeRobot** account to any AI agent to actively manage your website monitors, alert contacts, and response times directly from your conversational workspace.

### What you can do

- **Uptime Monitors** — List all configured services natively, retrieve individual historical logs, create new endpoints to monitor (HTTP, Ping), edit configurations, or permanently delete monitors.
- **Alert Contacts** — Browse your configured alert notification targets (Email, Slack, Webhooks), create new distribution recipients, and manage who gets notified upon downtime.
- **Metrics & History** — Reset historical statistics for specific monitors quickly or retrieve the raw data array of up ratios and response times to graph or analyze.
- **Account Setup** — Extract UptimeRobot account usage to discover your remaining monitor slots limits and overall subscription features.

### How it works

1. Subscribe to this server
2. Enter your main UptimeRobot API Key
3. Start managing your uptime coverage from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — instantly setup standard monitoring checks for newly deployed microservices straight from the terminal/editor.
- **SRE Teams** — pull SLA metrics, uptime percentage stats, and incident reaction logs directly into your incident management context window.
- **System Administrators** — manage alert contacts by automatically adding new on-call employees to notification targets quickly.
- **Founders & Indie Hackers** — get a fast, bird's eye view summary report on your entire infrastructure uptime across all your apps without opening the dashboard.


## Available Tools
- **delete_alert_contact**: This action is irreversible.

Permanently deletes an alert contact
- **delete_uptime_monitor**: This action is irreversible.

Permanently deletes an uptime monitor
- **update_uptime_monitor**: Updates an existing monitor configuration
- **get_account_info**: Retrieves UptimeRobot account usage and limits
- **get_monitor_details**: Retrieves full details for a specific UptimeRobot monitor
- **list_alert_contacts**: Lists all configured alert notification targets (Email, Slack, Webhook, etc.)
- **list_monitors**: Returns pass/fail status, up ratio, and response times.

Lists all uptime monitors configured in UptimeRobot
- **create_alert_contact**: Type 2=Email, 11=Slack.

Creates a new alert notification target
- **create_uptime_monitor**: Provide a friendly name, URL, and type (1=HTTP, 3=Ping).

Creates a new uptime monitor
- **reset_monitor_logs**: Resets monitoring logs and statistics for a specific monitor


## Installation & Usage

To install and use the **UptimeRobot** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uptimerobot](https://vinkius.com/mcp/uptimerobot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
