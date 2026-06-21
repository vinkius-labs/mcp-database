# Temporal MCP Server

Monitor and manage distributed workflows in Temporal Cloud natively via your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/temporal)

## Overview
**Category:** ship-it
**Tools Count:** 7

## Description
Connect your **Temporal Cloud** (or self-hosted) cluster to any AI agent and bring the power of durable execution directly into your IDE or chat via natural conversation.

### What you can do

- **Workflows & Executions** — List, filter, and inspect active, running, or completed workflow executions
- **Workflow History** — Retrieve the complete sequence of events, activities, and signals to debug failures
- **Visibility Search** — Run complex SQL-like queries using Temporal Visibility syntax to find specific runs
- **Namespace Details** — Check retention periods, configurations, and metadata of your operational namespace
- **Schedules & Cron** — Browse all recurring workflows and predict the next execution schedules

### How it works

1. Subscribe to this server
2. Enter your Temporal Address, Namespace, and API Key (or cert pathway)
3. Start querying cluster states strictly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Engineers** — debug failed workflow runs and retrieve precise event histories without opening the Temporal UI
- **Platform Teams** — audit namespaces and search attributes to ensure data consistency globally
- **Site Reliability Engineers (SREs)** — query complex visibility logs during incident responses


## Available Tools
- **get_workflow_history**: Retrieves the event history for a workflow execution
- **get_namespace_details**: Retrieves information about the current namespace
- **get_workflow_details**: Retrieves details for a specific workflow execution
- **list_schedules**: Lists all workflow schedules
- **list_search_attributes**: Lists custom search attributes available in the namespace
- **list_workflows**: Returns workflow IDs, run IDs, and statuses.

Lists all workflow executions in the configured namespace
- **search_workflows**: g., WorkflowType="MyType" AND Status="Running").

Search workflows using Temporal Visibility Query syntax


## Installation & Usage

To install and use the **Temporal** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/temporal](https://vinkius.com/mcp/temporal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
