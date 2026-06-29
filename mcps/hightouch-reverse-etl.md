# Hightouch (Reverse ETL) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hightouch-reverse-etl)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Synchronize data via Hightouch — list syncs, monitor runs, and manage data models.

## Description
Connect your **Hightouch** account to any AI agent and take full control of your Reverse ETL workflows and data synchronization through natural conversation.

### What you can do

- **Sync Orchestration** — List all data synchronization schedules and retrieve detailed metrics and schemas tied to specific syncs directly from your agent
- **Run History** — Extract historical execution states and success logs to monitor the performance and reliability of your sync runs
- **Data Modeling** — Audit SQL definitions bounding your warehouse analytics pipelines and inspect the data models driving your syncs
- **Source Management** — Enumerate active Data Warehouse connections and securely map inbound schemas from platforms like Snowflake or BigQuery
- **Destination Audit** — Identify connected SaaS nodes (Salesforce, HubSpot, Slack) receiving synchronized outbound objects from your warehouse

### How it works

1. Subscribe to this server
2. Enter your Hightouch API Key
3. Start managing your data synchronization from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Engineers** — monitor sync health and audit SQL model definitions through natural conversation without opening the UI
- **Analytics Engineers** — verify warehouse source connections and ensure data models are correctly mapped to outbound destinations
- **Growth Operations** — check sync run histories and success rates to ensure critical marketing and sales data is always up-to-date


## Available Tools (6)
- **list_syncs**: List all syncs
- **get_sync**: Get sync details
- **list_sync_runs**: List sync runs
- **list_models**: List all models
- **list_sources**: List all sources
- **list_destinations**: List all destinations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hightouch (Reverse ETL)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current Hightouch syncs"

**🤖 AI Agent:**
> I've found 5 active syncs. Highlights include 'Snowflake to Salesforce' (ID: sync-001), 'BigQuery to HubSpot' (ID: sync-004), and 'Postgres to Slack' (ID: sync-007). Would you like the status of the most recent run for any of these?

---

**👤 You:**
> "Show me the last 5 runs for sync ID 'sync-001'"

**🤖 AI Agent:**
> Retrieving run history for 'sync-001'… The last 5 runs all finished with a 'Success' status. A total of 12,450 rows were processed in the most recent run (finished 2 hours ago). Would you like to see if any errors were logged in previous weeks?

---

**👤 You:**
> "Which data sources are connected to our Hightouch account?"

**🤖 AI Agent:**
> I've identified 3 connected data sources: 'Production Snowflake', 'Stripe BigQuery Dataset', and 'Internal Postgres'. All connections are showing as 'Active'. Would you like to see the available models for 'Production Snowflake'?


## ❓ FAQ

**Q: Can I check the SQL definition of a data model through my agent?**
Yes. Use the `list_models` tool to retrieve pure SQL definitions bounding your warehouse analytics pipelines. This allows your agent to audit transformation logic without you needing to dive into the Hightouch UI.

**Q: How do I monitor the success rate of my sync runs?**
The `list_sync_runs` tool provides historical execution states and success tracking for any specific Sync ID. Your agent can aggregate these logs to report on overall reliability and identify transient failures.

**Q: Can I see which SaaS apps are receiving data from Hightouch?**
Absolutely. Use the `list_destinations` tool to identify all connected SaaS nodes accepting synchronized outbound objects. This helps you audit exactly where your warehouse data is being pushed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hightouch-reverse-etl](https://vinkius.com/mcp/hightouch-reverse-etl)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hightouch (Reverse ETL)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hightouch-reverse-etl` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hightouch (Reverse ETL)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hightouch-reverse-etl": {
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
