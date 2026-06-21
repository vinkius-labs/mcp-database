# Checkly MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/checkly)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/checkly-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/checkly-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage application monitoring and E2E testing via Checkly — track API uptime, trigger checks, and monitor performance directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Checkly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my monitors in Checkly and their last status."

**🤖 AI Agent:**
> Retrieving your monitors... I found 5 active checks: 'Main API' (Passing), 'Checkout Flow' (Passing), 'Auth Service' (Failing), and 2 heartbeats. Would you like details on the failing check?

---

**👤 You:**
> "Show me the response time graph for the 'Checkout Flow' check."

**🤖 AI Agent:**
> Retrieving performance data for 'Checkout Flow'... Over the last 24 hours, average response time was 450ms, with a peak of 1.2s at 3 AM. Uptime remains at 100%.

---

**👤 You:**
> "Check the status of my heartbeat monitors."

**🤖 AI Agent:**
> Checking heartbeats... You have 2 active heartbeats: 'Hourly DB Cleanup' (Active, Last ping 45m ago) and 'Daily Report Sync' (Active, Last ping 12h ago). Both are within their expected intervals.


## Installation & Usage

To install and use the **Checkly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/checkly](https://vinkius.com/mcp/checkly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
