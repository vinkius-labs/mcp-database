# Grafana MCP Server

Manage observability via Grafana — search and inspect dashboards, monitor alerts, and handle data sources directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/grafana)

## Overview
**Category:** loved-by-devs
**Tools Count:** 4

## Description
Connect your **Grafana** instance to any AI agent and take full control of your application observability, dashboard inspections, and alerting workflows through natural conversation.

### What you can do

- **Dashboard Discovery Orchestration** — Search for Grafana dashboards by title or tag to retrieve unique UIDs and metadata natively within your chat
- **Panel & Query Inspection** — Retrieve the full configuration of any dashboard by UID, extracting precise PromQL, LogQL, or SQL queries and panel layouts flawlessly
- **Data Source Auditing** — List all configured data sources including Prometheus, Loki, CloudWatch, and SQL databases to verify connectivity boundaries securely
- **Alert Monitoring Oversight** — Enumerate active alert rules and retrieve current firing states to monitor system health and resolve incidents synchronously
- **Observability Navigation** — Analyze specific localized variables decoding active monitoring routes and extracting structural constraints from your Grafana environment
- **SRE Command Center** — Verify dashboard UIDs and retrieve query strings to debug performance regressions or analyze log patterns using natural language

### How it works

1. Subscribe to this server
2. Enter your Grafana Instance URL and Service Account Token (found in Administration > Users & Access > Service accounts)
3. Start inspecting your observability stack from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SRE & DevOps Engineers** — monitor alert rules and inspect dashboard queries without manual navigation in the Grafana UI
- **Cloud Architects** — audit data source configurations and verify dashboard organization using natural language
- **Software Developers** — extract PromQL or LogQL queries from existing panels to verify metrics and logs during development
- **Incident Responders** — quickly find relevant dashboards and check alert statuses during active troubleshooting


## Available Tools
- **search_dashboards**: Returns basic info including the UID. To inspect the panels and queries of a dashboard, use get_dashboard with the uid.

Search Grafana dashboards by title or tag
- **get_dashboard**: Requires the dashboard UID, which you can get from search_dashboards.

Get full dashboard configuration including panels and queries
- **list_datasources**: ) are available in this Grafana instance.

List all configured data sources in Grafana
- **firing_alerts**: Returns alerting rules that are currently in "firing" state, including their labels and annotations.

Get currently firing alerts from Grafana Unified Alerting


## Installation & Usage

To install and use the **Grafana** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/grafana](https://vinkius.com/mcp/grafana)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
