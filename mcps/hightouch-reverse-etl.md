# Hightouch (Reverse ETL) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hightouch-reverse-etl)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hightouch-reverse-etl-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hightouch-reverse-etl-mcp)
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


## Available Tools
- **list_destinations**: List all destinations
- **list_syncs**: List all syncs
- **get_sync**: Get sync details
- **list_sync_runs**: List sync runs
- **list_models**: List all models
- **list_sources**: List all sources


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


## Installation & Usage

To install and use the **Hightouch (Reverse ETL)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hightouch-reverse-etl](https://vinkius.com/mcp/hightouch-reverse-etl)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
