# Databox MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/databox)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Visualize KPIs from hundreds of data sources in custom dashboards that keep your entire team focused on what matters.

## Description
Connect your **Databox** account to any AI agent and take full control of your business intelligence and data ingestion workflows through natural conversation.

### What you can do

- **Dataset Orchestration** — List and manage your database collections (tables) programmatically, including retrieving detailed schema metadata and primary key configurations
- **High-Fidelity Ingestion** — Programmatically push arrays of raw data records directly into Databox to coordinate real-time metric visualization and reporting
- **Source Architecture** — Access and manage your directory of data source integrations and connected accounts to maintain high-fidelity data feeds
- **Usage Monitoring** — Programmatically track your data storage statistics and API activity logs to coordinate your analytics budget and quotas
- **Operational Visibility** — Check authenticated user profiles and verify system connectivity directly through your agent for instant BI reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key (v1)** from your Databox dashboard (Account Settings > API Tokens)
3. Start pushing your business metrics and managing datasets from Claude, Cursor, or any MCP client

No more manual metric logging or digging through complex SQL transformations in the dashboard. Your AI acts as your dedicated data engineer and BI coordinator.

### Who is this for?

- **Data Analysts** — instantly ingest new data points and verify dataset structures using natural language commands
- **Marketing & Sales Ops** — automate the reporting of custom metrics and monitor storage limits without leaving your workspace
- **Operations Leads** — track API activity logs and manage data source connections through simple AI queries


## Available Tools
- **create_data_source**: Create a new data source
- **create_dataset**: Create a new dataset
- **delete_dataset**: Delete a dataset
- **get_dataset_details**: Get details for a specific dataset
- **get_current_user**: Get authenticated user profile
- **get_storage_statistics**: Get data storage stats
- **list_accounts**: List all Databox accounts
- **list_data_sources**: List data sources for an account
- **list_datasets**: List all datasets
- **list_activity_logs**: List API activity logs
- **list_dataset_metrics**: List metrics in a dataset
- **push_metrics_data**: Ingest data into a dataset


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Databox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all datasets in my Databox account."

**🤖 AI Agent:**
> I've retrieved your datasets. You currently have 3 collections: 'Daily Sales' (ID: ds_123), 'User Engagement', and 'API Logs'. Which one would you like to push data to?

---

**👤 You:**
> "Push record to 'ds_123': value 1500, date '2026-04-16'."

**🤖 AI Agent:**
> Data pushed successfully! I've ingested the value 1500 for 2026-04-16 into the 'Daily Sales' dataset. The metric is now being processed for your dashboards.

---

**👤 You:**
> "Show my storage usage and API activity logs."

**🤖 AI Agent:**
> Retrieving metrics... You're using 45% of your data storage quota. Recent logs show 10 successful pushes to 'Daily Sales' in the last hour. Everything is running smoothly.


## ❓ FAQ

**Q: How do I find my Databox API Key?**
Log in to your account, navigate to **Account Settings** > **API Tokens**, and copy your unique v1 API Key.

**Q: Can I create new datasets via AI?**
Yes! Use the `create_dataset` tool. You'll need to specify a title, a source ID, and an array of primary keys for the table structure.

**Q: Does it support real-time data pushing?**
The `push_metrics_data` tool allows for immediate ingestion of data records, making them available for visualization in Databox instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/databox](https://vinkius.com/mcp/databox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Databox** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `databox` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Databox** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "databox": {
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
