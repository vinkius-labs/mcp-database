# Axiom MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/axiom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Manage logs and observability data via Axiom — ingest data, run APL queries, and manage datasets or monitors directly from any AI agent.

## Description
Connect your **Axiom** account to any AI agent to streamline your observability and log management workflows through natural conversation.

### What you can do

- **Data Ingestion & Querying** — Ingest JSON, NDJSON, or CSV data and run complex Axiom Processing Language (APL) queries to analyze logs in real-time.
- **Dataset Management** — List, create, and update datasets to organize your telemetry and infrastructure data efficiently.
- **Monitoring & Alerts** — Manage monitors and notifiers to stay informed about system performance, errors, and anomalies.
- **Dashboards & Annotations** — Access dashboards and create annotations to visualize trends and mark significant system events.
- **Organization Insights** — Retrieve user information, API tokens, and organization details to maintain secure and authorized access.

### How it works

1. Subscribe to this server
2. Enter your Axiom API Token and optional Organization ID
3. Start analyzing your logs and managing infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & SREs** — instantly query logs for errors, check monitor statuses, and manage alerts without leaving the terminal or chat.
- **Software Engineers** — debug production issues by running APL queries directly from the code editor to find specific trace IDs or logs.
- **Data Analysts** — ingest and analyze large datasets using Axiom's powerful processing language through simple natural language prompts.


## Available Tools (31)
- **create_annotation**: Create a new annotation
- **create_dashboard**: Create a new dashboard
- **create_dataset**: Create a new dataset
- **create_monitor**: Create a new monitor
- **create_notifier**: Create a new notifier
- **delete_annotation**: Delete an annotation
- **delete_dashboard**: Delete a dashboard
- **delete_dataset**: Delete a dataset
- **delete_monitor**: Delete a monitor
- **delete_notifier**: Delete a notifier
- **get_annotation**: Retrieve a specific annotation by ID
- **get_dashboard**: Retrieve a specific dashboard by UID
- **get_dataset**: Retrieve a specific dataset by ID
- **get_monitor**: Retrieve a specific monitor by ID
- **get_notifier**: Retrieve a specific notifier by ID
- **get_org**: Retrieve an organization by ID
- **get_user**: Retrieve a specific user by ID
- **ingest_data**: Ingest data into an Axiom dataset
- **list_annotations**: List all annotations
- **list_dashboards**: List all dashboards
- **list_datasets**: List all datasets
- **list_monitors**: List all monitors
- **list_notifiers**: List all notifiers
- **list_tokens**: List all API tokens
- **list_users**: List all users
- **run_query**: Run an APL query against Axiom data
- **update_annotation**: Update an existing annotation
- **update_dashboard**: Update an existing dashboard
- **update_dataset**: Update an existing dataset
- **update_monitor**: Update an existing monitor
- **update_notifier**: Update an existing notifier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Axiom** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my available Axiom datasets."

**🤖 AI Agent:**
> I've retrieved your datasets. You have 3 active datasets: 'production-logs' (ID: ds_123), 'staging-metrics' (ID: ds_456), and 'security-audit' (ID: ds_789).

---

**👤 You:**
> "Run an APL query to count errors in 'production-logs' from the last 24 hours."

**🤖 AI Agent:**
> Executing query: `['production-logs'] | where level == 'error' | summarize count()`... I found 142 error events in the specified timeframe. Would you like to see the specific error messages?

---

**👤 You:**
> "Create a new monitor named 'High Latency' that checks for response times over 500ms."

**🤖 AI Agent:**
> I've created the 'High Latency' monitor. It will run every 5 minutes using your APL query to detect threshold breaches. Monitor ID: mon_abc123.


## ❓ FAQ

**Q: Can I run complex log analysis using Axiom Processing Language (APL)?**
Yes! Use the `run_query` tool to execute any APL string. You can specify `start_time` and `end_time` to filter your data and get precise analytical results directly in the chat.

**Q: How do I send new log data to my Axiom datasets?**
You can use the `ingest_data` tool. Simply provide the `dataset_name`, the data `payload`, and the `content_type` (JSON, NDJSON, or CSV) to stream data into your Axiom account.

**Q: Is it possible to manage system monitors and alerts through this integration?**
Absolutely. You have access to a full suite of tools including `list_monitors`, `create_monitor`, and `update_monitor` to configure threshold or anomaly detection alerts based on your APL queries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/axiom](https://vinkius.com/mcp/axiom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Axiom** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `axiom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Axiom** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "axiom": {
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
