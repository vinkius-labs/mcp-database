# Uptime.com MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uptimecom)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/uptimecom-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/uptimecom-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Monitor website and API uptime from 30+ global locations with instant alerts when downtime hits any of your services.

## Description
Connect your **Uptime.com** monitoring account to any AI agent and simplify how you monitor site reliability, manage alerts, and perform root cause analysis through natural conversation.

### What you can do

- **Check Management** — List, create, and update monitor checks (HTTP, API, ICMP) to ensure your services are always online.
- **Alert Oversight** — Retrieve a history of recent UP/DOWN transitions and stay notified of critical outages.
- **Incident Analysis** — Get detailed Root Cause Analysis (RCA) for alerts to understand why a failure occurred.
- **Performance Metrics** — Query uptime statistics and performance data for any specific monitor check.
- **Team Coordination** — List contact groups and third-party integrations (Slack, PagerDuty) to manage notification flows.
- **Infrastructure Monitoring** — List global monitoring nodes to understand your testing coverage.

### How it works

1. Subscribe to this server
2. Enter your Uptime.com API Token (found in your account settings)
3. Start monitoring your uptime from Claude, Cursor, or any MCP client

### Who is this for?

- **SRE & DevOps Engineers** — quickly retrieve RCA reports and check performance stats via simple AI queries.
- **Web Administrators** — create new monitor checks and verify site health directly from the workspace.
- **Product Owners** — monitor uptime metrics and recent alert history to measure service reliability via the AI assistant.


## Available Tools
- **create_check**: g., HTTP, API).

Create a new check
- **delete_check**: Delete a monitor check
- **get_account_info**: com account.

Get account profile
- **get_check**: Get check details
- **get_root_cause_analysis**: Get alert RCA
- **get_check_stats**: Get check statistics
- **list_recent_alerts**: List recent monitor alerts
- **list_checks**: List all monitor checks
- **list_contact_groups**: List contact groups
- **list_integrations**: ).

List active integrations
- **list_monitoring_nodes**: List global nodes
- **update_check**: Update a check


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Uptime.com** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active monitor checks in my account."

**🤖 AI Agent:**
> I've retrieved your checks. You have 5 monitors active including 'Main Website' (UP), 'API Gateway' (UP), and 'Staging Server' (DOWN). Which one would you like more details on?

---

**👤 You:**
> "Show me the recent alerts history."

**🤖 AI Agent:**
> I've fetched the alert history. There were 2 downtime events today: 'Staging Server' (Down for 15m) and 'API Gateway' (Down for 2m). Both are currently back online. Shall I retrieve the RCA for the Staging Server outage?

---

**👤 You:**
> "What is the uptime percentage for the 'Main Website' check?"

**🤖 AI Agent:**
> Retrieving statistics... The 'Main Website' (ID: 10293) has an uptime of 99.98% over the last 30 days, with an average response time of 150ms. No significant failures detected recently.


## Installation & Usage

To install and use the **Uptime.com** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uptimecom](https://vinkius.com/mcp/uptimecom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
