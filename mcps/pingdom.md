# Pingdom MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pingdom)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pingdom-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pingdom-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Monitor website uptime and performance via Pingdom — list checks, track response times, and manage alerts directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pingdom** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current uptime checks and their status."

**🤖 AI Agent:**
> I've retrieved 10 checks. 'Main Site' is UP, 'Checkout API' is UP, but 'Legacy Support Portal' is currently DOWN. Would you like to see the error log for the down service?

---

**👤 You:**
> "What was the average response time for the 'Main Site' check (ID: 12345) today?"

**🤖 AI Agent:**
> The average response time for 'Main Site' today is 342ms. Performance has been stable with a slight spike to 580ms around 10:00 AM UTC.

---

**👤 You:**
> "Pause the uptime check for ID 98765 for our scheduled maintenance."

**🤖 AI Agent:**
> Check 98765 has been successfully paused. Remember to ask me to resume it once the maintenance is finished!


## Installation & Usage

To install and use the **Pingdom** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pingdom](https://vinkius.com/mcp/pingdom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
