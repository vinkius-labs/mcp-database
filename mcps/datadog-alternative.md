# Datadog MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/datadog-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Monitor infrastructure, APM and logs via Datadog — query metrics, audit monitors, search logs and track incidents from any AI agent.

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


## Available Tools (16)
- **create_monitor**: Requires the monitor type (metric, anomaly, service check, event, log, process, rum, synthetics), a query string (e.g. "avg(last_5m):avg:system.cpu.user{host:myhost} > 80"), a notification message (using @user, @slack, @pagerduty) and a name. Optionally set tags, priority, renotify interval and threshold windows.

Create a new Datadog monitor
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
- **list_dashboards**: Use to discover available dashboards before opening a specific one.

List all Datadog dashboards
- **unmute_monitor**: Provide the monitor ID. Optionally set a scope to unmute only specific sub-alerts.

Unmute a Datadog monitor
- **update_monitor**: Provide the monitor ID and any fields to update: name, query, message, tags, priority or thresholds. Only the fields you provide will be changed.

Update an existing Datadog monitor
- **list_users**: Use to audit access, identify inactive accounts and verify user permissions.

List Datadog users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Datadog** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all monitors that are currently in alert state."

**🤖 AI Agent:**
> I've scanned your Datadog monitors and found 3 currently in Alert state: 'High CPU Usage on web01' (metric alert, triggered 12m ago), 'API Latency P99 > 500ms' (query alert, triggered 5m ago) and 'Database Connection Pool Exhausted' (service check, critical). Would you like me to check the recent logs for any of these?

---

**👤 You:**
> "Search for error logs from the payment-service in the last hour."

**🤖 AI Agent:**
> I found 14 error logs for payment-service. The most common pattern is a 'ConnectionTimeout: upstream service did not respond within 30s' from host prod-web-03, occurring 9 times in the last hour. Would you like the full log entry with stacktrace?

---

**👤 You:**
> "What's our API error rate over the past 24 hours?"

**🤖 AI Agent:**
> I queried the metric `sum:api.http.5xx{env:production}.as_count()` for the past 24h. The error rate peaked at 142 errors/min at 14:30 UTC and has been trending down to ~15 errors/min currently. The 24h average is 38 errors/min. Would you like me to correlate this with recent deployments?


## ❓ FAQ

**Q: What's the difference between Datadog API Key and Application Key?**
The **API Key** authenticates your requests to the Datadog platform and is required for all endpoints. The **Application Key** is an additional layer of authorization that controls what actions your integration can perform. Both are generated in Organization Settings > API and Application Keys. Most Datadog API endpoints require both keys.

**Q: Can I mute a monitor during a maintenance window?**
Yes! Use the `mute_monitor` action with the monitor ID. You can optionally set an `end` timestamp (ISO 8601) for the mute to automatically expire, or specify a `scope` to mute only certain sub-alerts (e.g. 'env:staging'). Use `unmute_monitor` to re-enable notifications.

**Q: What query syntax does the metrics endpoint use?**
Datadog uses a specific query format: `[function]:[metric]{[tags]}`. For example: `avg:system.cpu.user{host:web01}` returns the average CPU user time for host web01. Common functions include `avg`, `sum`, `max`, `min`, `count`. Time windows are specified in the query as `avg(last_5m):...` or passed as `from`/`to` Unix timestamps to the tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datadog-alternative](https://vinkius.com/mcp/datadog-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Datadog** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `datadog-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Datadog** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "datadog-alternative": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
