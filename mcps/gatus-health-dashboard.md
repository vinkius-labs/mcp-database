# Gatus (Health Dashboard) MCP Server

Monitor infrastructure health via Gatus — list endpoints, check real-time status, and analyze performance metrics directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gatus-health-dashboard)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 4

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


## Installation & Usage

To install and use the **Gatus (Health Dashboard)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gatus-health-dashboard](https://vinkius.com/mcp/gatus-health-dashboard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
