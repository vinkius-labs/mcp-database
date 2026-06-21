# Datadog MCP Server

Monitor applications via Datadog — query performance metrics, search logs, and list active monitors directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/datadog)

## Overview
**Category:** industry-titans
**Tools Count:** 11

## Description
Connect your **Datadog** account to any AI agent and take full control of your infrastructure monitoring and log management through natural conversation.

### What you can do

- **Metric Auditing** — Execute static queries targeting numeric telemetry datastores to resolve specific DDQL metrics objects generated dynamically
- **Log Investigation** — Perform structural extraction matching target string traces inside Datadog logs to evaluate status boundaries across your apps
- **Monitor Management** — Discover explicit system rule endpoints bounding configured triggers against alert metrics to verify health states
- **Telemetry Extraction** — Fetch timestamp arrays natively from numeric logged endpoints to analyze performance trends over specific time intervals
- **Log Filtering** — Apply ISO boundary mappings to compare logging payloads and identify exactly when errors or bottlenecks occurred

### How it works

1. Connect the Datadog integration to your AI assistant.
2. Authorize using your Datadog API Key, APP Key, and Site.
3. Monitor your entire cloud infrastructure using natural language.

### Who is this for?

- **DevOps Engineers** — monitor system health and audit alerts without switching to the Datadog dashboard
- **Software Developers** — search through application logs and verify metric telemetry directly from the IDE or chat
- **SREs** — monitor active alerts and analyze performance trends during incident response
- **System Admins** — audit monitor configurations and verify system boundaries through natural language


## Available Tools
- **list_dashboards**: Returns a list of dashboard identifiers, titles, layout types (timeboard/screenboard), and direct access URLs.

List all dashboards
- **query_metrics**: Resolves time-series data within the specified UNIX timestamp range. Returns metric points, scope tags, and unit metadata for infrastructure and application monitoring.

Query time-series metrics
- **list_downtimes**: Returns scope tags, recurring schedules, and current status to identify planned maintenance periods.

List scheduled downtimes
- **list_slos**: Returns SLO definitions including target percentages, time windows, and current compliance status for monitor-based or metric-based objectives.

List Service Level Objectives
- **search_logs**: Interacts with the log storage boundary to retrieve entries matching the query syntax, including timestamps, status levels, and structured attributes.

Search application logs
- **list_monitors**: Filters results by operational state (alert, warn, no data, ok) and returns monitor metadata including type, query, and current status.

List monitors by state
- **get_monitor**: Resolves notification settings, threshold values, and historical status changes for the given monitor ID.

Get monitor details
- **mute_monitor**: Interacts with the alerting boundary to set temporary silence periods, optionally with an automatic expiration timestamp.

Mute a monitor
- **list_events**: Returns a collection of events including titles, priority levels, and source identifiers (e.g., monitor alerts, deployment events).

List events
- **get_dashboard**: Resolves all widget configurations, template variables, and layout structures for visualization rendering.

Get dashboard details
- **list_hosts**: Returns host metadata including agent version, active tags, and associated cloud provider attributes.

List infrastructure hosts


## Installation & Usage

To install and use the **Datadog** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datadog](https://vinkius.com/mcp/datadog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
