# Airbyte MCP Server

Monitor your Airbyte data pipelines via AI — track sync jobs, list sources, and check connections instantly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/airbyte)

## Overview
**Category:** brain-trust
**Tools Count:** 7

## Description
Connect your **Airbyte** data integration instance to your AI agent to unlock conversational monitoring for your ETL/ELT pipelines. Let your agent audit your modern data stack automatically without touching the dashboard.

### What you can do

- **Monitor Connections** — Retrieve the full list of your configured connections linking sources to destinations
- **Track Jobs** — View historical synchronization runs, success rates, and identify failing sync jobs instantly
- **Audit Sources & Destinations** — List all your active data origins (like Postgres, Stripe) and targets (Snowflake, BigQuery)
- **Granular Inspection** — Fetch detailed UUID configuration and statuses for a specific source or active connection
- **Workspace Analytics** — Verify your active Airbyte workspaces and general environment configurations

### How it works

1. Subscribe to this server
2. Enter your Airbyte API URL and API Key
3. Let your agent run diagnostic queries via Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Engineers** — let the agent check yesterday's sync job success rate or debug a failing database connection
- **Analytics Engineers** — quickly list configured warehouse destinations and verify infrastructure paths
- **Data Analysts** — get a high-level summary of all active data sources pumping into the main data lake


## Available Tools
- **list_sources**: List all Airbyte sources
- **get_source**: Get details of a specific Airbyte source
- **list_destinations**: List all Airbyte destinations
- **list_connections**: List all Airbyte sync connections
- **get_connection**: Get details of a specific Airbyte connection
- **list_jobs**: List synchronization jobs for a connection
- **list_workspaces**: List workspaces


## Installation & Usage

To install and use the **Airbyte** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/airbyte](https://vinkius.com/mcp/airbyte)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
