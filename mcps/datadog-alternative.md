# Datadog MCP Server

Monitor infrastructure, APM and logs via Datadog — query metrics, audit monitors, search logs and track incidents from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/datadog-alternative)

## Overview
**Category:** loved-by-devs
**Tools Count:** 16

## Description
Connect your **Datadog** account to any AI agent and gain full observability over your entire infrastructure, applications and logs through natural conversation.

### What you can do

- **Monitor Management** — List, create, update, mute and unmute alert monitors across metric, anomaly, log, service check and synthetics types
- **Metrics Querying** — Query raw metric timeseries data with Datadog's query syntax to analyze CPU, memory, custom business metrics and more
- **Log Search** — Search structured and unstructured log events using the same query syntax as the Log Explorer, filtering by service, host, status and any indexed attribute
- **Dashboard Discovery** — List all dashboards, view their widget configurations and audit shared access without opening the Datadog app
- **Synthetics & SLOs** — Audit your synthetic test coverage and Service Level Objectives to track SLA compliance across teams
- **Incident Tracking** — View active and recently resolved incidents with severity, responder assignments and postmortem status
- **Infrastructure Inventory** — List all monitored hosts with their tags, metrics summary and agent version
- **Team & User Auditing** — Review team membership, user roles and access permissions to maintain organizational security

### How it works

1. Subscribe to this server
2. Enter your Datadog API Key and Application Key
3. Start monitoring your stack from Claude, Cursor, or any MCP-compatible client

Stop context-switching to the Datadog dashboard every time an alert fires. Your AI acts as a dedicated SRE.

### Who is this for?

- **SREs & On-Call Engineers** — instantly triage monitors, search error logs and check incident status without opening Datadog
- **Engineering Managers** — audit monitor coverage, review SLO compliance and track team ownership across services
- **Developers** — query metrics, inspect log events and verify synthetics directly from your IDE


## Available Tools
- **create_monitor**: Requires the monitor type (metric, anomaly, service check, event, log, process, rum, synthetics), a query string (e.g. "avg(last_5m):avg:system.cpu.user{host:myhost} > 80"), a notification message (using @user, @slack, @pagerduty) and a name. Optionally set tags, priority, renotify interval and threshold windows.

Create a new Datadog monitor
- **list_dashboards**: Use to discover available dashboards before opening a specific one.

List all Datadog dashboards
- **get_dashboard**: Provide the dashboard ID.

Get details for a specific Datadog dashboard
- **get_monitor**: Provide the numeric monitor ID.

Get details for a specific Datadog monitor
- **list_hosts**: Each host reports CPU, memory, disk, network metrics plus custom tags. Optionally filter by a tag string (e.g. "env:production") to narrow results.

List hosts monitored by Datadog
- **list_incidents**: Each incident has a title, severity, status (active, resolved), timeline, responder assignments and postmortem status. Use to audit ongoing incidents and review resolution patterns.

List Datadog incident management records
- **list_monitors**: Monitors track metrics, anomalies, service checks and events. Each monitor has a type (metric, anomaly, service check, event, log), name, query string, notification message and current status. Use this to audit your alerting coverage.

List all Datadog monitors
- **mute_monitor**: Useful during maintenance windows or known incidents. Provide the monitor ID. Optionally set an end timestamp for auto-unmute or a scope to mute only specific sub-alerts.

Mute a Datadog monitor
- **query_metrics**: The query string uses Datadog syntax like "avg:system.cpu.user{host:myhost}". Provide Unix timestamps for the from/to range. Useful for analyzing metric trends without opening a dashboard.

Query Datadog metrics timeseries
- **search_logs**: Supports filtering by source, service, status, host and any indexed attribute. Example query: "service:api status:error". Returns matching log entries with full context, host info and trace ID if available.

Search Datadog logs
- **list_slos**: Each SLO defines a target availability percentage (e.g. 99.9%) for a service over a time window (7d, 30d, 90d). Useful for auditing SLA compliance across teams.

List Datadog Service Level Objectives
- **list_synthetics_tests**: Each test has a type, target URL, status, locations and check frequency. Use to audit your synthetic test coverage and verify endpoints are being monitored.

List Datadog Synthetics tests
- **list_teams**: Teams group users for ownership of monitors, dashboards, SLOs and incidents. Each team has a name, handle, description and user membership list.

List Datadog teams
- **unmute_monitor**: Provide the monitor ID. Optionally set a scope to unmute only specific sub-alerts.

Unmute a Datadog monitor
- **update_monitor**: Provide the monitor ID and any fields to update: name, query, message, tags, priority or thresholds. Only the fields you provide will be changed.

Update an existing Datadog monitor
- **list_users**: Use to audit access, identify inactive accounts and verify user permissions.

List Datadog users


## Installation & Usage

To install and use the **Datadog** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datadog-alternative](https://vinkius.com/mcp/datadog-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
