# Tinybird Data Platform MCP Server

Analyze real-time data via Tinybird — manage Data Sources, inspect Pipes, and query endpoints directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tinybird-data-platform)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

## Description
Connect your AI agent to **Tinybird**, the real-time data platform for developers. This integration allows you to oversee your analytical infrastructure, manage ingestion storage (Data Sources), and interact with transformation logic (Pipes) through natural conversation.

### What you can do

- **Infrastructure Oversight** — List and inspect all your Data Sources and Pipes in real-time
- **Transformation Analysis** — Retrieve SQL logic and nodes for any Pipe to understand how data is being processed
- **Live Querying** — Execute published Pipes or run arbitrary SQL queries (ClickHouse dialect) to explore your data directly via the agent
- **Operational Metrics** — Check ingestion stats, row counts, and storage sizes for your analytical units
- **Access Control** — List and audit authentication tokens and workspace configurations

### How it works

1. Subscribe to this server
2. Enter your **Tinybird Admin Token** (found in your Tinybird workspace settings)
3. Start analyzing and managing your real-time data flows via chat

### Who is this for?

- **Data Engineers** — quickly audit pipe logic and data source states during development
- **Product Analysts** — run quick SQL queries or check pipe outputs without opening the dashboard
- **DevOps Teams** — monitor ingestion performance and token scopes via AI assistance


## Available Tools
- **execute_sql_query**: Execute an arbitrary SQL query against the Tinybird workspace
- **get_datasource_details**: Get comprehensive information for a specific Data Source
- **get_pipe_details**: Get detailed information for a specific Pipe
- **get_datasource_stats**: Retrieve ingestion and usage statistics for a Data Source
- **list_datasources**: Retrieve a list of all Data Sources in the current workspace
- **list_pipe_nodes**: List all SQL nodes within a specific Pipe
- **list_pipes**: Retrieve a list of all Pipes in the current workspace
- **list_auth_tokens**: Retrieve a list of all authentication tokens in the workspace
- **list_workspaces**: Retrieve a list of available workspaces
- **query_pipe_data**: Execute a Pipe and retrieve the results as JSON


## Installation & Usage

To install and use the **Tinybird Data Platform** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tinybird-data-platform](https://vinkius.com/mcp/tinybird-data-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
