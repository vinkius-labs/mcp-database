# Redash MCP Server

Connect to Redash to manage SQL queries, execute data visualizations, and monitor dashboards directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/redash)

## Overview
**Category:** data-analytics
**Tools Count:** 17

## Description
Connect your **Redash** instance to any AI agent to interact with your data through natural language. This server allows you to bridge the gap between raw data and actionable insights.

### What you can do

- **Query Management** — List, create, and update SQL queries. Archive old queries to keep your workspace clean.
- **Data Execution** — Execute queries on-demand, handle parameters, and fetch fresh or cached results.
- **Dashboard Access** — Browse and retrieve dashboard configurations and visualizations.
- **Data Source Inspection** — Check the status and configuration of your connected data sources.
- **Job Tracking** — Monitor the progress of long-running query executions (jobs).

### How it works

1. Subscribe to this server
2. Provide your Redash Base URL and API Key
3. Start asking your AI to run reports or fetch data metrics

### Who is this for?

- **Data Analysts** — Quickly iterate on SQL queries and check results without switching tabs.
- **Business Intelligence Leads** — Monitor dashboard statuses and share insights via chat.
- **Engineers** — Test data source connections and manage query objects programmatically through the agent.


## Available Tools
- **archive_dashboard**: Archive the specified dashboard
- **archive_query**: Archive the specified query
- **create_dashboard**: Create a new dashboard object
- **create_query**: Create a new query object
- **execute_query**: Parameters must be provided for parameterized queries.

Initiates a new query execution or returns a cached result
- **get_cached_query_result**: Get a cached result for a query ID (non-parameterized only)
- **get_dashboard**: Returns an individual dashboard object
- **get_data_source**: Get data source details
- **get_job**: SUCCESS includes query_result_id.

Returns the status of a query task (job)
- **get_query_result**: Returns a query result by its result ID
- **get_query**: Get an individual query object
- **list_dashboards**: Returns a paginated array of dashboard objects
- **list_queries**: List Redash queries
- **test_data_source**: Test connection for a data source
- **update_dashboard**: Edit an existing dashboard object
- **update_data_source**: Configure a data source (e.g., SSH tunnel)
- **update_query**: Edit an existing query object


## Installation & Usage

To install and use the **Redash** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/redash](https://vinkius.com/mcp/redash)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
