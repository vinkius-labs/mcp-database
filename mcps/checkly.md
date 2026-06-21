# Checkly MCP Server

Manage application monitoring and E2E testing via Checkly — track API uptime, trigger checks, and monitor performance directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/checkly)

## Overview
**Category:** loved-by-devs
**Tools Count:** 8

## Description
Connect your **Checkly** account to any AI agent and take full control of your application monitoring and synthetic testing through natural conversation. Streamline how you ensure the uptime and performance of your APIs and web apps.

### What you can do

- **Check Oversight** — List and retrieve details for all API and Browser monitors natively
- **Live Execution** — Manually trigger check runs to verify system health on-demand flawlessly
- **Performance Intelligence** — Access detailed performance metrics and response times for any monitor securely
- **Alert Management** — List and audit all configured alert channels (Slack, Email, PagerDuty) flawlessly
- **Reliability Tracking** — Monitor heartbeat and cron jobs to ensure your background tasks are running flawlessly
- **System Metadata** — Retrieve core account information and organizational structures directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Checkly API Key and Account ID (obtained from your settings)
3. Start managing your monitoring stack from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — monitor API uptime and trigger manual checks using natural language
- **SREs** — audit performance metrics and alert configurations without opening the dashboard
- **Backend Developers** — verify API health and review check results straight from their chat interface
- **QA Automation Engineers** — monitor the status of browser-based synthetic tests


## Available Tools
- **get_checkly_account_info**: Retrieve core account and organization metadata
- **get_check_performance_metrics**: Retrieve performance metrics for a specific check
- **get_check_details**: Get detailed information for a specific check
- **list_checkly_alert_channels**: List all configured alert channels (Slack, Email, PagerDuty, etc)
- **list_checkly_checks**: List all API and Browser checks
- **list_check_groups**: List groups of checks
- **list_checkly_heartbeats**: List all heartbeat (cron) monitors
- **trigger_check_run**: Manually trigger a check to run immediately


## Installation & Usage

To install and use the **Checkly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/checkly](https://vinkius.com/mcp/checkly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
