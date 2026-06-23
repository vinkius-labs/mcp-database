# Datadog MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/datadog-extended)
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


## Available Tools (16)
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


## ❓ FAQ

**Q: Can I silence noisy monitors during scheduled maintenance?**
Yes. The `mute_monitor` action silences a specific monitor by its ID, suppressing all alert notifications. This is ideal during deployment windows or planned maintenance. Use `search_monitors` to find the monitor by name or tag first, then mute it by ID.

**Q: Does Datadog require two credentials to connect?**
Yes. You need your **API Key** (found in Organization Settings > API Keys) and your **Base URL**, which depends on your Datadog site region: `https://api.datadoghq.com` for US1, `https://api.datadoghq.eu` for EU, or `https://api.us3.datadoghq.com` for US3. The API Key is sent via the `DD-API-KEY` header.

**Q: Can I run time-series metric queries with custom time ranges?**
Yes. The `query_metrics` tool accepts a Datadog metric query string (e.g., `avg:system.cpu.user{host:web-01}`), a start epoch timestamp, and an end epoch timestamp. It returns the time-series data points for that metric across the specified window.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datadog-extended](https://vinkius.com/mcp/datadog-extended)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `datadog-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Datadog** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "datadog-extended": {
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
