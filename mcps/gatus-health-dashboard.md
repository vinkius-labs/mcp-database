# Gatus (Health Dashboard) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gatus-health-dashboard)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gatus-health-dashboard-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gatus-health-dashboard-mcp)
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


## Installation & Usage

To install and use the **Gatus (Health Dashboard)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gatus-health-dashboard](https://vinkius.com/mcp/gatus-health-dashboard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
