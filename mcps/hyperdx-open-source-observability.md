# HyperDX (Open Source Observability) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hyperdx-open-source-observability)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hyperdx-open-source-observability-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hyperdx-open-source-observability-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [devops-cicd](../categories/devops-cicd.md)

Monitor logs, events, and alerts via HyperDX — search logs, manage alert rules, and inspect dashboards directly from your AI agent.

## Description
Connect your **HyperDX** instance to any AI agent to gain deep visibility into your infrastructure and applications through natural conversation.

### What you can do

- **Log & Event Analysis** — Search through logs and structured events using powerful query filters to debug issues in real-time.
- **Alert Management** — List, create, and delete alert rules to stay on top of system health and performance regressions.
- **Dashboard Inspection** — Retrieve a list of all dashboards and fetch specific dashboard details to visualize metrics and trends.
- **Time-based Filtering** — Query data using relative time ranges (like 15m, 1h, 24h) or specific ISO 8601 timestamps for precise troubleshooting.

### How it works

1. Subscribe to this server
2. Enter your HyperDX API Key
3. Start debugging and monitoring from Claude, Cursor, or any MCP-compatible client

No more jumping between tabs to correlate logs with alerts. Your AI acts as an on-call engineer or SRE assistant.

### Who is this for?

- **DevOps Engineers** — quickly check error rates and system logs without switching to a browser
- **SREs** — manage alert thresholds and investigate incidents directly from the terminal or chat interface
- **Developers** — fetch logs for specific services or trace IDs while staying in the flow of coding


## Available Tools
- **list_alerts**: Returns a list of all configured alert rules
- **create_alert**: Create a new alert rule
- **list_dashboards**: Retrieve all dashboards in the organization
- **delete_alert**: Delete a specific alert rule by ID
- **list_events**: Use query parameter for filtering.

Retrieve events (structured logs or spans) from HyperDX
- **get_dashboard**: Retrieve details for a specific dashboard
- **list_logs**: Use query parameter for filtering (e.g., level:error service:auth).

Retrieve a list of logs based on search criteria


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HyperDX (Open Source Observability)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all logs with level:error for the auth service from the last hour."

**🤖 AI Agent:**
> I've retrieved the logs for the auth service. I found 12 error entries in the last hour, mostly related to 'Invalid Token' exceptions. Would you like to see the full details of the most recent one?

---

**👤 You:**
> "Create a new alert named 'High Error Rate' that triggers when errors exceed 50 in 5 minutes."

**🤖 AI Agent:**
> Successfully created the alert 'High Error Rate'. It is configured to monitor the query 'level:error' and will trigger if the count exceeds 50 within a 5-minute interval.

---

**👤 You:**
> "Show me all my available dashboards in HyperDX."

**🤖 AI Agent:**
> I found 3 dashboards in your organization: 'System Health', 'API Performance', and 'User Analytics'. Which one would you like to inspect in detail?


## Installation & Usage

To install and use the **HyperDX (Open Source Observability)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hyperdx-open-source-observability](https://vinkius.com/mcp/hyperdx-open-source-observability)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
