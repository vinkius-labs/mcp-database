# UptimeRobot MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uptimerobot)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/uptimerobot-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/uptimerobot-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Monitor and manage your website uptime seamlessly. List, create, and resolve monitor alerts directly from your AI agent, 24/7.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UptimeRobot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my monitors and highlight any that are currently down."

**🤖 AI Agent:**
> You currently have 15 active Uptime monitors. 14 are responding properly (Status: UP). 1 monitor (`API Authentication Service`, ID 9923812) is currently DOWN. It has been failing ping requests for the last 14 minutes. Do you want me to fetch the complete log history for that failed process?

---

**👤 You:**
> "Create an HTTP monitor for our newly deployed marketing site (`https://marketing.vinkius.com/`)."

**🤖 AI Agent:**
> I have successfully created an HTTP monitor named 'marketing.vinkius.com'. Its unique ID is `1884931`. Your account indicates you have 34 monitor slots still freely accessible. Please keep in mind it might take approximately 2–5 minutes before it collects its first meaningful round of SLA availability stats.

---

**👤 You:**
> "Delete alert contact 'old-devops@acme.com'. Our team rotated users."

**🤖 AI Agent:**
> I've permanently removed notification target ID `78233` (old-devops@acme.com) from UptimeRobot global alert contacts list safely. Future downtimes will no longer dispatch there. Would you like me to create an external endpoint webhook alert point to replace it immediately in the pipeline?


## Installation & Usage

To install and use the **UptimeRobot** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uptimerobot](https://vinkius.com/mcp/uptimerobot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
