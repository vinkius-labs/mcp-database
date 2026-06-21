# Sumo Logic MCP Server

Manage logs, metrics, and collectors via Sumo Logic — run search jobs, monitor infrastructure, and manage collectors directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sumo-logic-alternative)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 19

## Description
Connect your **Sumo Logic** account to any AI agent to streamline your observability and log management workflows through natural conversation.

### What you can do

- **Log Search Jobs** — Create, poll, and retrieve results from asynchronous search jobs (`create_search_job`, `get_search_job_status`) for deep log analysis.
- **Collector Management** — List, create, and update Hosted or Installed Collectors (`list_collectors`, `create_hosted_collector`) to manage data ingestion.
- **Source Configuration** — Manage data sources within your collectors to ensure proper log flow and visibility.
- **Metrics Querying** — Execute metrics queries (`execute_metrics_query`) to monitor system performance and health in real-time.
- **User Administration** — List and manage users within your Sumo Logic organization to maintain secure access.

### How it works

1. Subscribe to this server
2. Enter your Sumo Logic Access ID, Access Key, and API URL
3. Start querying logs and managing infrastructure from Claude, Cursor, or any MCP-compatible client

No more switching between dashboards to find that one error log. Your AI acts as a dedicated SRE or DevOps engineer.

### Who is this for?

- **DevOps Engineers** — instantly search for production errors and check collector health without leaving the terminal or IDE
- **Security Analysts** — run quick log queries to investigate potential threats and manage user access
- **SREs** — monitor system metrics and manage data ingestion sources through simple natural language commands


## Available Tools
- **create_hosted_collector**: Create a new Hosted Collector
- **create_search_job**: Returns a SEARCH_JOB_ID which must be polled for status.

Create an asynchronous log search job
- **create_source**: Create a new Source within a Collector
- **create_user**: Create a new user
- **delete_collector**: Delete a Collector
- **delete_search_job**: Delete a search job to free up concurrent slots
- **delete_source**: Delete a Source
- **delete_user**: Delete a user
- **execute_metrics_query**: Execute metrics query and retrieve time-series data
- **get_collector**: Get details for a specific Collector by ID
- **get_search_job_messages**: Get raw log messages from a completed search job
- **get_search_job_records**: Get aggregated records from a completed search job
- **get_search_job_status**: Poll the status of a search job
- **get_source**: Get details for a specific Source
- **list_collectors**: List all Installed and Hosted Collectors
- **list_sources**: List all Sources within a specific Collector
- **list_users**: List all users in the organization
- **update_collector**: Update an existing Collector
- **update_source**: Update an existing Source


## Installation & Usage

To install and use the **Sumo Logic** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sumo-logic-alternative](https://vinkius.com/mcp/sumo-logic-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
