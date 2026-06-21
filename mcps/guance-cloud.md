# Guance Cloud / 观测云 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/guance-cloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/guance-cloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/guance-cloud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Modern observability platform — manage monitors, dashboards, and events via AI.

## Description
Empower your AI agent to orchestrate your entire observability stack with **Guance Cloud** (观测云), the leading next-generation monitoring platform. By connecting Guance Cloud to your agent, you transform complex system monitoring, log analysis, and incident response into a natural conversation. Your agent can instantly list your monitors, retrieve detailed dashboard configurations, browse system events, and even execute Data Query Language (DQL) statements without you ever needing to navigate the Guance console. Whether you are troubleshooting a production outage or auditing resource usage, your agent acts as a real-time site reliability assistant, keeping your infrastructure data accurate and your systems healthy.

### What you can do

- **Workspace Orchestration** — Retrieve detailed metadata and status information for your Guance Cloud workspace.
- **Monitoring Control** — List and retrieve detailed configurations for all system monitors and alert rules.
- **Event Auditing** — Browse real-time observability events, including alerts, errors, and system changes.
- **Data Querying** — Execute powerful DQL statements to retrieve specific metrics and logging data via natural language.
- **Operations Insights** — Monitor billing usage and manage API access keys for your organizational infrastructure.

### How it works

1. Subscribe to this server
2. Enter your Guance Cloud API Key (DF-API-KEY)
3. Start managing your observability stack through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SRE & DevOps Engineers** — automate incident response and monitor system health through natural language queries.
- **Infrastructure Leads** — coordinate monitoring strategies and audit dashboard configurations directly from your AI-powered workspace.
- **Technical Analysts** — retrieve system metrics and perform log analysis via a unified AI interface.
- **Guance Cloud Users** — integrate your existing observability workflows into your AI-driven daily routines.


## Available Tools
- **get_billing**: Get billing usage
- **get_event**: Get event details
- **get_monitor**: Get monitor details
- **get_workspace**: Get workspace information
- **list_access_keys**: List workspace access keys
- **list_dashboards**: List all dashboards
- **list_events**: ) from the workspace.

List observability events
- **list_log_sources**: List log data sources
- **list_monitors**: List all monitors
- **query_data**: Query Guance data (DQL)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Guance Cloud / 观测云** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active monitors in Guance Cloud."

**🤖 AI Agent:**
> I've retrieved your active monitors. You have 15 monitors configured, including 'High CPU Alert', 'API Latency', and 'Database Connection'. Would you like to check the status of the alerts?

---

**👤 You:**
> "Show me recent events from the last hour."

**🤖 AI Agent:**
> I've listed 5 events from the last hour. There was 1 Critical alert for 'Storage Full' and 4 Information events regarding system updates. Should I retrieve the details for the Critical alert?

---

**👤 You:**
> "Query average CPU usage using DQL."

**🤖 AI Agent:**
> I've executed the DQL query. The average CPU usage across your 'Production' cluster over the last 15 minutes is 42%. Would you like a breakdown by individual host?


## Installation & Usage

To install and use the **Guance Cloud / 观测云** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/guance-cloud](https://vinkius.com/mcp/guance-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
