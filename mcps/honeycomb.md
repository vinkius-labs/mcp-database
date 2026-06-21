# Honeycomb MCP Server

Automate observability via Honeycomb — manage datasets, queries, and markers directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/honeycomb)

## Overview
**Category:** brain-trust
**Tools Count:** 12

## Description
Connect your **Honeycomb.io** observability platform to any AI agent and take full control of your telemetry data, query specifications, and incident markers through natural conversation.

### What you can do

- **Dataset Oversight** — List all event sources, retrieve detailed metadata, and monitor last access times for your datasets.
- **Query Management** — Define new query specifications and execute them to retrieve granular performance insights.
- **Marker Automation** — Create timeline annotations (e.g., for deployments or outages) to contextualize your data visualization.
- **Schema Insights** — List and inspect columns within specific datasets to understand your event structure.
- **Team Collaboration** — Access shared boards and retrieve information about your Honeycomb team configuration.
- **Incident Analysis** — Use AI to run complex queries and retrieve results for rapid troubleshooting and RCA.

### How it works

1. Subscribe to this server
2. Enter your Honeycomb API Key and select your Region (US or EU)
3. Start querying your telemetry from Claude, Cursor, or any MCP-compatible client

No more manual configuration of complex query DSLs for simple status checks. Your AI assistant acts as a dedicated Observability Engineer or SRE Analyst.

### Who is this for?

- **SREs & DevOps** — instantly retrieve query results and create markers during incident response.
- **Software Engineers** — monitor the performance of new deployments by inspecting specific dataset trends.
- **Platform Leads** — maintain a real-time overview of dataset usage and board sharing across the organization.


## Available Tools
- **create_marker**: Pass details as a JSON string in "body_json" (requires message). Use "__all__" for team-wide markers.

Create a new marker (e.g., deploy, maintenance) on a dataset timeline
- **create_query_specification**: Pass the specification as a JSON string in "query_json". Returns a query ID for execution.

Create a new query specification for a dataset
- **run_query**: Poll for results using "get_query_result" with the returned result ID.

Execute a query specification and return a result ID
- **get_dataset_details**: Get metadata for a specific dataset
- **get_team_details**: Retrieve information about the Honeycomb team
- **get_query_result**: Retrieve the results of an executed query
- **list_honeycomb_boards**: List all boards (dashboards) shared with the team
- **list_dataset_columns**: List all columns (fields) defined in a specific dataset
- **list_datasets**: Use this to find the "slug" required for markers and queries.

List all datasets in your Honeycomb team
- **list_markers**: List markers (annotations) for a dataset
- **list_queries**: List query specifications for a specific dataset
- **list_triggers**: List triggers (alerts) defined for a dataset


## Installation & Usage

To install and use the **Honeycomb** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/honeycomb](https://vinkius.com/mcp/honeycomb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
