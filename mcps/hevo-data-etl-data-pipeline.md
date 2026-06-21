# Hevo Data (ETL & Data Pipeline) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hevo-data-etl-data-pipeline)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage data pipelines via Hevo — list pipelines, monitor destinations, and track usage.

## Description
Connect your **Hevo Data** account to any AI agent and take full control of your automated data integration and ETL orchestration through natural conversation.

### What you can do

- **Pipeline Orchestration** — List all running ETL pipelines and extract explicit routing mappings linking ingestion frequencies to specific IDs directly from your agent
- **Destination Monitoring** — Analyze global warehouse targets (BigQuery, Snowflake, Redshift) terminating your replication runs and ensuring data delivery
- **Transformation Models** — Track explicitly attached mappings and transformations bounding your staging logic to maintain data quality
- **Workflow Automation** — Discover orchestration bounds and DAG workflows connecting transformations natively across your entire data stack
- **Usage & Billing Audit** — Access account usage metrics and billing ceilings to monitor row replications and overall account health in real-time

### How it works

1. Subscribe to this server
2. Enter your Hevo Data API Key and Region (e.g. US, EU, AU, IN)
3. Start managing your data pipelines from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Engineers** — monitor ETL pipeline health and destination replication statuses through natural conversation without jumping between dashboards
- **Analytics Leads** — check transformation models and workflow orchestrations to ensure data is ready for reporting
- **Operations Teams** — track row usage and account billing ceilings to ensure data pipelines stay within organizational budgets


## Available Tools (6)
- **list_pipelines**: List all pipelines
- **get_pipeline**: Get pipeline details
- **list_destinations**: List all destinations
- **list_models**: List all models
- **list_workflows**: List all workflows
- **get_usage**: Get account usage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hevo Data (ETL & Data Pipeline)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active Hevo pipelines"

**🤖 AI Agent:**
> I've found 6 active pipelines. Highlights include 'Stripe to BigQuery' (ID: pipe-001), 'HubSpot to Snowflake' (ID: pipe-005), and 'Shopify to Redshift' (ID: pipe-008). Would you like to check the usage for any of these?

---

**👤 You:**
> "Show me the destinations for my 'Sales Data' pipeline"

**🤖 AI Agent:**
> The 'Sales Data' pipeline (ID: pipe-005) is currently replicating to 2 destinations: a BigQuery production dataset and a Snowflake staging warehouse. Both are showing 'Healthy' status. Would you like to see the last sync time?

---

**👤 You:**
> "How much of my row quota have I used this month?"

**🤖 AI Agent:**
> You've used 12.5 million rows out of your 20 million row monthly quota (62.5%). At current ingestion rates, you are projected to finish the month at 18.2 million rows. I can break down usage by pipeline if needed.


## ❓ FAQ

**Q: Can I check the status of my data destinations through my agent?**
Yes. Use the `list_destinations` tool to see all your warehouse targets. Your agent will provide the status and details of where your data is being replicated, ensuring delivery to platforms like BigQuery or Snowflake.

**Q: How do I find a specific pipeline's configuration?**
Use the `get_pipeline` tool with a unique Pipeline ID to extract explicit routing mappings and ingestion frequencies. This is perfect for auditing specific ETL flows without manual searching.

**Q: Can I monitor my account's row usage through a conversation?**
Absolutely. The `get_usage` tool retrieves real-time account usage metrics and billing ceilings, helping you track how many rows have been replicated and ensure you stay within your plan's limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hevo-data-etl-data-pipeline](https://vinkius.com/mcp/hevo-data-etl-data-pipeline)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hevo Data (ETL & Data Pipeline)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hevo-data-etl-data-pipeline` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hevo Data (ETL & Data Pipeline)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hevo-data-etl-data-pipeline": {
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
