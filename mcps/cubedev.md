# Cube.dev MCP Server

Access your Cube semantic layer — execute queries, inspect generated SQL, manage pre-aggregations, and explore data metadata directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cubedev)

## Overview
**Category:** brain-trust
**Tools Count:** 15

## Description
Connect your **Cube.dev** instance to any AI agent to bridge the gap between natural language and your data warehouse. This server allows your agent to interact with Cube's semantic layer, ensuring consistent metrics and high-performance data retrieval.

### What you can do

- **Data Querying** — Execute complex REST API queries using `load_query` to fetch aggregated data with measures, dimensions, and filters.
- **SQL Inspection** — Use `get_sql` and `execute_cube_sql` to debug or run raw queries against the SQL API for deep data investigation.
- **Metadata Exploration** — Retrieve cube definitions, views, and segments via `get_meta` to understand your data model without leaving the chat.
- **Performance Management** — Trigger and monitor background pre-aggregation builds with `trigger_pre_aggregation_job` to ensure your dashboards stay fast.
- **Cloud Management** — List deployments and environments if using Cube Cloud to manage your infrastructure context.

### How it works

1. Subscribe to this server
2. Provide your Cube API URL and Secret Token
3. Start asking questions about your data metrics and model structure

### Who is this for?

- **Data Engineers** — quickly verify data models and trigger cache refreshes via CLI or AI interface.
- **Analytics Engineers** — debug generated SQL and inspect metadata to ensure metric consistency.
- **Product Managers** — get instant answers to data questions by letting the AI query the semantic layer directly.


## Available Tools
- **check_live**: Check if Cube deployment is live
- **check_ready**: Check if Cube deployment is ready
- **convert_query**: Convert a SQL query to a REST API query format
- **execute_cube_sql**: Execute a raw SQL query against the SQL API
- **generate_meta_token**: Requires CUBE_CLOUD_API_KEY.

Generate a JWT for the Metadata API
- **get_entity**: Get detailed metadata for a specific entity
- **get_meta**: Get metadata for cubes and views
- **get_pre_aggregation_job_status**: Get status of pre-aggregation jobs
- **get_sql**: Useful for debugging.

Get generated SQL for a Cube query
- **list_data_sources**: List configured data sources
- **list_deployments**: Requires CUBE_CLOUD_API_KEY.

List all Cube Cloud deployments
- **list_entities**: List all cubes and views
- **list_environments**: Requires CUBE_CLOUD_API_KEY.

List environments for a deployment
- **load_query**: Use this to get aggregated data.

Execute a Cube query and return results
- **trigger_pre_aggregation_job**: Trigger a pre-aggregation build job


## Installation & Usage

To install and use the **Cube.dev** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cubedev](https://vinkius.com/mcp/cubedev)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
