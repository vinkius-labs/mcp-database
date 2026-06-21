# Hevo Data (ETL & Data Pipeline) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hevo-data-etl-data-pipeline)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hevo-data-etl-data-pipeline-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hevo-data-etl-data-pipeline-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Hevo Data (ETL & Data Pipeline)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hevo-data-etl-data-pipeline](https://vinkius.com/mcp/hevo-data-etl-data-pipeline)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
