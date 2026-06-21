# Dagster MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dagster)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dagster-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dagster-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Orchestrate data pipelines via Dagster — monitor jobs, track runs, manage software-defined assets, and audit schedules directly from any AI agent.

## Description
Connect your **Dagster** (Plus or open-source) instance to any AI agent and take full control of your data orchestration and asset management through natural conversation.

### What you can do

- **Job Orchestration** — List and audit all data jobs available in your Dagster server to understand active pipeline boundaries
- **Run Monitoring** — Fetch chronological history of recent job runs and retrieve detailed status and execution logs for specific run IDs
- **Asset Tracking** — Enumerate software-defined assets to identify data dependencies and verify physical storage mappings
- **Schedules & Sensors** — List all configured job schedules and active sensors listening for external events to audit automation triggers
- **Environment Audit** — Identify deployment boundaries and verify instance connectivity across Dagster Plus or self-hosted clusters

### How it works

1. Subscribe to this server
2. Enter your Dagster URL and User API Token (found in Deployment Settings > Tokens)
3. Start managing your data pipelines from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Engineers** — monitor pipeline health and identify failed runs without leaving the chat or IDE
- **Analytics Engineers** — track software-defined assets and verify data freshness in real-time
- **Data Platform Teams** — audit job schedules and sensor configurations across organizational deployments
- **SREs** — monitor Dagster agent health and verify instance connectivity through natural language


## Available Tools
- **list_jobs**: List all jobs from Dagster
- **list_runs**: List recent runs from Dagster
- **get_run**: Get run details from Dagster
- **list_assets**: List all assets from Dagster
- **list_schedules**: List all schedules from Dagster
- **list_sensors**: List all sensors from Dagster


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dagster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all jobs in my Dagster deployment"

**🤖 AI Agent:**
> I found 5 jobs in your deployment including 'daily_etl_job', 'ml_training_pipeline', and 'sensor_triggered_sync'. Which one would you like to audit for recent runs?

---

**👤 You:**
> "Show me the status of the last 5 runs"

**🤖 AI Agent:**
> Here are the last 5 runs. The most recent (ID: 123) for 'daily_etl_job' finished with status 'Success'. Run 121 failed. Would you like to see the error logs for the failed run?

---

**👤 You:**
> "What assets are currently defined in my project?"

**🤖 AI Agent:**
> I found 12 software-defined assets including 'raw_customer_data', 'cleaned_sales_table', and 'monthly_metrics_view'. I can provide the materialization history for any of these assets.


## Installation & Usage

To install and use the **Dagster** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dagster](https://vinkius.com/mcp/dagster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
