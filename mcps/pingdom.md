# Pingdom MCP Server

Monitor website uptime and performance via Pingdom — list checks, track response times, and manage alerts directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pingdom)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **Pingdom** account to any AI agent and take full control of your website monitoring and reliability workflows through natural conversation.

### What you can do

- **Uptime Visibility** — List all monitoring checks and retrieve real-time status (up, down, unconfirmed).
- **Performance Tracking** — Fetch average response times and detailed outage history for any specific check.
- **Log Auditing** — Retrieve raw check results to investigate specific errors or latency spikes.
- **Global Infrastructure Oversight** — List all Pingdom probe locations to understand your monitoring coverage.
- **Alert Management** — List notification contacts and pause or resume checks during maintenance windows.

### How it works

1. Subscribe to this server
2. Enter your Pingdom API Token
3. Start monitoring your infrastructure directly from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps Engineers** — quickly check if a service is down or audit recent outages while investigating incidents.
- **Site Reliability Engineers (SRE)** — monitor response time trends and verify probe locations directly from the IDE.
- **System Administrators** — pause uptime checks during scheduled maintenance to avoid false alerts.


## Available Tools
- **get_check_details**: Get details for a specific check
- **get_check_outages**: List outages for a specific check
- **get_average_response_time**: Get average response time for a check
- **list_uptime_checks**: List all Pingdom uptime checks
- **list_alert_contacts**: List alert notification contacts
- **list_maintenance_windows**: List scheduled maintenance windows
- **list_pingdom_probes**: List all Pingdom monitoring locations (probes)
- **list_check_results**: List individual check results/logs
- **pause_uptime_check**: Pause a specific uptime check
- **resume_uptime_check**: Resume a specific uptime check


## Installation & Usage

To install and use the **Pingdom** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pingdom](https://vinkius.com/mcp/pingdom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
