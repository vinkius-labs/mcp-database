# Gatus (Health Dashboard) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gatus-health-dashboard)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Monitor infrastructure health via Gatus — list endpoints, check real-time status, and analyze performance metrics directly from any AI agent.

## Description
Connect your **Gatus** health dashboard to any AI agent to monitor your services and infrastructure through natural conversation.

### What you can do

- **Global Visibility** — List all monitored endpoints and their current health status across your entire infrastructure.
- **Deep Health Inspection** — Drill down into specific services to see recent results and status history using slugified keys.
- **Performance Statistics** — Retrieve performance metrics for individual endpoints to identify latency or reliability issues.
- **Metrics Export** — Access raw Prometheus-compatible metrics for deep technical analysis and custom reporting.

### How it works

1. Subscribe to this server
2. Enter your Gatus instance URL
3. Start monitoring your system health from Claude, Cursor, or any MCP-compatible client.

No more manual dashboard checking. Your AI acts as a 24/7 SRE assistant, providing instant insights into your service availability.

### Who is this for?

- **DevOps Engineers** — quickly audit service health and retrieve raw metrics without leaving the terminal or IDE.
- **SRE Teams** — investigate performance regressions and endpoint history through natural language queries.
- **Product Owners** — get high-level status reports on system availability during incidents.


## Available Tools
- **get_endpoint_health**: Get health status and recent results for a specific endpoint
- **get_endpoint_stats**: Get performance statistics for a specific endpoint
- **list_endpoints**: Get all monitored endpoints and their current status
- **get_metrics**: Get Prometheus-compatible metrics from Gatus


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gatus (Health Dashboard)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all monitored endpoints and their current status."

**🤖 AI Agent:**
> I've retrieved the status for 8 endpoints. 7 are 'Healthy' and 1 ('payment-gateway') is currently 'Unhealthy'. Would you like me to investigate the 'payment-gateway' results?

---

**👤 You:**
> "What is the health status of the 'core-api' endpoint?"

**🤖 AI Agent:**
> The 'core-api' endpoint is currently Healthy. The last check was successful with a 200 OK response and a latency of 45ms. Recent history shows 100% uptime over the last 24 hours.

---

**👤 You:**
> "Show me the performance statistics for 'database-service'."

**🤖 AI Agent:**
> Fetching stats for 'database-service'... Average latency is 12ms, with a 99th percentile of 85ms. There have been 0 failures in the last 500 requests.


## ❓ FAQ

**Q: Can I see the status of all my services at once?**
Yes! Use the `list_endpoints` tool to retrieve a complete list of all configured endpoints and their current health status across your Gatus instance.

**Q: How do I check the performance history of a specific service?**
You can use `get_endpoint_stats` with the endpoint's slugified key to see detailed performance statistics, or `get_endpoint_health` for recent health check results.

**Q: Does this server provide raw metrics for analysis?**
Yes, the `get_metrics` tool retrieves raw Prometheus-compatible metrics exported by Gatus, allowing your AI to perform deep technical analysis.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gatus-health-dashboard](https://vinkius.com/mcp/gatus-health-dashboard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gatus (Health Dashboard)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gatus-health-dashboard` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gatus (Health Dashboard)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gatus-health-dashboard": {
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
