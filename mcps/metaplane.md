# Metaplane MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/metaplane)
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


## ❓ FAQ

**Q: How do I find my Metaplane API Key?**
Log in to Metaplane, go to your Account Settings, and you can generate or copy your API Key from the API section.

**Q: Can I trigger a monitor run manually?**
Yes! Use the `trigger_monitor_run` tool and provide the monitor ID to start a data quality check immediately.

**Q: Is my data observability data secure?**
Absolutely. Your token is encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/metaplane](https://vinkius.com/mcp/metaplane)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Metaplane** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `metaplane` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Metaplane** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "metaplane": {
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
