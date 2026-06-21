# Datadog MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/datadog-extended)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/datadog-extended-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/datadog-extended-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Monitor infrastructure, applications, and logs with unified observability that gives you full-stack visibility in real time.

## Description
Connect your **Datadog** account to any AI agent and take full control of your observability stack through natural conversation.

### What you can do

- **Monitor Management** — List, search, inspect, and mute monitors to control alert noise during maintenance windows
- **Dashboard Inspection** — Browse dashboards and retrieve full layouts, widgets, and template variables
- **Metric Queries** — Run time-series queries using Datadog syntax (e.g., `avg:system.cpu.user{*}`) with custom time ranges
- **Log Search** — Search log events using Datadog query syntax across all indexed log sources
- **Event Tracking** — Browse platform events and create custom events with tags and priority levels
- **Incident Management** — List active incidents with severity, status, responders, and timeline details
- **SLO Monitoring** — Review Service Level Objectives with targets, error budgets, and compliance status
- **Host Inventory** — Access all reporting hosts with metadata, tags, and agent versions

### How it works

1. Subscribe to this server
2. Enter your Datadog API Key and your site URL (e.g., `https://api.datadoghq.com` for US or `https://api.datadoghq.eu` for EU)
3. Start monitoring your infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SRE / DevOps Engineers** — query monitors, mute noisy alerts, and inspect incidents without opening the Datadog dashboard
- **Platform Teams** — run metric queries and validate SLO compliance through conversational AI
- **On-Call Engineers** — triage incidents, search error logs, and check host health during outages via natural language


## Available Tools
- **check_datadog_status**: Verify connectivity
- **create_event**: Create an event
- **get_dashboard**: Get dashboard details
- **get_incident**: Get incident details
- **get_monitor**: Get monitor details
- **list_dashboards**: List dashboards
- **list_events**: List events
- **list_hosts**: List hosts
- **list_incidents**: List incidents
- **list_metrics**: List metrics
- **list_monitors**: List monitors
- **list_slos**: List SLOs
- **mute_monitor**: Mute a monitor
- **query_metrics**: Query metric data
- **search_logs**: Search logs
- **search_monitors**: Search monitors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Datadog** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all monitors that are currently alerting and mute the noisiest one."

**🤖 AI Agent:**
> Found 4 monitors in Alert state. 1) 'High CPU - web-prod-01' (ID: 58291, triggered 47 times today). 2) 'Disk Space Low - db-replica-03' (ID: 58344, triggered 12 times). 3) 'API Latency P99 > 500ms' (ID: 58402, triggered 8 times). 4) 'Error Rate > 5%' (ID: 58415, triggered 3 times). Muting the noisiest one... Monitor 58291 'High CPU - web-prod-01' has been muted. No further alerts will fire until unmuted.

---

**👤 You:**
> "Search for error logs in production from the last hour."

**🤖 AI Agent:**
> Searching logs with query 'status:error env:production'... Found 234 error events in the last hour. Top sources: api-gateway (89 errors), payment-service (67 errors), user-auth (45 errors), notification-service (33 errors). The most frequent error: 'TimeoutException: upstream connection timed out' (124 occurrences). Would you like to see the full stack traces or check related incidents?

---

**👤 You:**
> "List all SLOs and tell me which ones are at risk of breaching their error budget."

**🤖 AI Agent:**
> Retrieved 8 SLOs. 2 are at risk: 1) 'API Availability (99.9%)' — current status: 99.82%, error budget remaining: 12% (7-day window). At current burn rate, budget will be exhausted in 2.3 days. 2) 'Checkout Latency P95 < 800ms' — current status: 99.1%, error budget remaining: 28%. The other 6 SLOs are healthy with >60% budget remaining. Would you like to inspect the monitors tied to the at-risk SLOs?


## Installation & Usage

To install and use the **Datadog** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datadog-extended](https://vinkius.com/mcp/datadog-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
