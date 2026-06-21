# Tingyun / 听云 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tingyun)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tingyun-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tingyun-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Leading APM and observability platform — manage applications, alerts, and performance metrics via AI.

## Description
Empower your AI agent to orchestrate your entire digital performance stack with **Tingyun** (听云), the premier APM and observability platform. By connecting Tingyun to your agent, you transform complex application monitoring, incident response, and performance auditing into a natural conversation. Your agent can instantly list monitored applications, retrieve real-time performance summaries, browse active alerts, and query specific metric data without you ever needing to navigate the Tingyun console. Whether you are troubleshooting a production bottleneck or auditing system health across a distributed architecture, your agent acts as a real-time site reliability assistant, keeping your performance data accurate and your systems responsive.

### What you can do

- **Application Orchestration** — List all APM applications and retrieve detailed health and performance summaries.
- **Incident Control** — Monitor active alerts and browse alert policies to identify and respond to performance issues.
- **Infrastructure Auditing** — List application instances, external service calls, and database dependencies.
- **Metric Querying** — Retrieve specific metric data points for applications to analyze trends and anomalies.
- **User Experience Insights** — Browse Real User Monitoring (RUM) browser applications to audit frontend performance.

### How it works

1. Subscribe to this server
2. Enter your Tingyun API Key and Secret Key
3. Start managing your observability stack through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & SRE Teams** — automate incident response and monitor application health through natural language queries.
- **Engineering Managers** — coordinate performance reviews and audit system dependencies directly from your AI-powered workspace.
- **Technical Analysts** — retrieve system metrics and perform bottleneck analysis via a unified AI interface.
- **Tingyun Power Users** — integrate your existing observability workflows into your AI-driven daily routines.


## Available Tools
- **get_account_info**: Get account metadata
- **get_app_summary**: Get application summary
- **get_metrics**: Query metric data
- **list_alerts**: List active alerts
- **list_app_instances**: List application instances
- **list_applications**: List APM applications
- **list_browser_apps**: List RUM browser applications
- **list_databases**: List monitored databases
- **list_external_services**: List external service calls
- **list_alert_policies**: List alert policies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tingyun / 听云** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all applications monitored by Tingyun."

**🤖 AI Agent:**
> I've retrieved your monitored applications. You have 12 APM applications, including 'Checkout Service', 'User API', and 'Auth Gateway'. Which one would you like to check the summary for?

---

**👤 You:**
> "Show me the performance summary for application ID 12345."

**🤖 AI Agent:**
> I've retrieved the summary for app 12345. Average response time is 150ms, error rate is 0.05%, and Apdex score is 0.95. Would you like to see the database dependency list?

---

**👤 You:**
> "Check for any critical alerts in Tingyun from today."

**🤖 AI Agent:**
> I've checked for alerts. There is 1 Critical alert for 'High Latency' on the 'Payment Service' and 2 Warnings regarding disk usage. Should I retrieve the alert detail for the high latency incident?


## Installation & Usage

To install and use the **Tingyun / 听云** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tingyun](https://vinkius.com/mcp/tingyun)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
