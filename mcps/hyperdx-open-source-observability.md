# HyperDX (Open Source Observability) MCP Server

Monitor logs, events, and alerts via HyperDX — search logs, manage alert rules, and inspect dashboards directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hyperdx-open-source-observability)

## Overview
**Category:** devops-cicd
**Tools Count:** 7

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


## Installation & Usage

To install and use the **HyperDX (Open Source Observability)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hyperdx-open-source-observability](https://vinkius.com/mcp/hyperdx-open-source-observability)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
