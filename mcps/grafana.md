# Grafana MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/grafana)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage observability via Grafana — search and inspect dashboards, monitor alerts, and handle data sources directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grafana** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for dashboards tagged with 'production'"

**🤖 AI Agent:**
> Searching dashboards... I found 3 matching dashboards: 'K8s Cluster Overview' (UID: abc-123), 'HTTP Response Metrics' (UID: def-456), and 'Database Performance'. Which one would you like me to inspect for panels?

---

**👤 You:**
> "Show me the queries for dashboard 'abc-123'"

**🤖 AI Agent:**
> Retrieving dashboard 'abc-123'... I found 5 panels. Highlights: 'CPU Usage' uses PromQL `sum(rate(node_cpu_seconds_total...))`, and 'Request Latency' uses `histogram_quantile(0.95, sum(rate(http_request_duration_seconds_bucket...)))`. Would you like the full JSON or more queries?

---

**👤 You:**
> "Are there any firing alerts right now?"

**🤖 AI Agent:**
> Checking alert rules... Yes, I found 1 firing alert: 'High Error Rate' on service 'API-v1'. It has been firing for 15 minutes. All other 12 alert rules are currently in 'Normal' state.


## ❓ FAQ

**Q: Can my agent search for specific dashboards in my Grafana instance?**
Yes. Use the 'search_dashboards' tool. You can provide an optional query string to match titles or tags. The agent will return basic info including the unique UID required for deeper inspection.

**Q: How do I extract the PromQL or SQL queries from a dashboard panel via chat?**
Use the 'get_dashboard' tool with the dashboard UID. Your agent will retrieve the full JSON configuration, including all panels and their underlying data queries, enabling you to review the exact metrics logic natively.

**Q: Can I see firing alerts through the agent?**
Absolutely. Use the 'list_alerts' tool. The agent retrieves all configured alert rules and their current statuses, allowing you to identify which monitors are currently in a firing state synchronousy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/grafana](https://vinkius.com/mcp/grafana)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grafana** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `grafana` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grafana** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grafana": {
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
