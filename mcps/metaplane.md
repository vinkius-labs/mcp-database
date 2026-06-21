# Metaplane MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/metaplane)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/metaplane-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/metaplane-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Data observability via Metaplane — track monitors, incidents, and data quality metrics.

## Description
Connect your **Metaplane** account to any AI agent and take full control of your data observability and quality through natural conversation.

### What you can do

- **Monitor Oversight** — List all configured data monitors and fetch detailed metadata and health statuses
- **Incident Management** — Retrieve real-time incident histories and track resolutions for data quality alerts
- **Automated Execution** — Programmatically trigger monitor runs to validate data quality on demand
- **Connection Visibility** — Enumerate connected databases, warehouses, and schemas to understand your data lineage
- **Alert Configuration** — List and inspect active notification settings and alert rules

### How it works

1. Subscribe to this server
2. Enter your Metaplane API Key
3. Start managing your data quality from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_account_info**: Get account information
- **get_incident**: Get details for a specific incident
- **get_monitor**: Get details for a specific monitor
- **get_monitor_runs**: Get run history for a monitor
- **list_configured_alerts**: List configured alerts
- **list_data_connections**: List all data source connections
- **list_incidents**: List data incidents
- **list_monitors**: List all data monitors
- **list_connection_schemas**: List schemas for a connection
- **trigger_monitor_run**: Trigger a monitor run


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Metaplane** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my data monitors in Metaplane."

**🤖 AI Agent:**
> Retrieving monitors... I found 5 active monitors including 'Postgres Row Count' and 'Snowflake Schema Change'.

---

**👤 You:**
> "Show recent incidents for the last 24 hours."

**🤖 AI Agent:**
> Checking incidents... There is one active high-severity incident: 'Null values detected in production.users'.

---

**👤 You:**
> "Trigger a run for monitor ID 'mon_12345'."

**🤖 AI Agent:**
> Triggering run... Monitor 'mon_12345' (Postgres Volume) has been started and is currently processing.


## Installation & Usage

To install and use the **Metaplane** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/metaplane](https://vinkius.com/mcp/metaplane)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
