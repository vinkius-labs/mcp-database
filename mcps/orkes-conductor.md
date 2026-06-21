# Orkes Conductor MCP Server

Orchestrate microservice workflows via Orkes Conductor — list definitions, track running executions, search workflow history, and inspect task states from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/orkes-conductor)

## Overview
**Category:** loved-by-devs
**Tools Count:** 6

## Description
Connect your **Orkes Conductor** cluster to any AI agent and get full visibility into your workflow orchestration layer — definitions, running instances, task states, and execution history.

### What you can do

- **Workflow Definitions** — List all registered workflow definitions with versions and descriptions, or inspect a specific workflow's graph schema with tasks, operators, and branching logic
- **Task Definitions** — List all registered task definitions available for orchestration within your workflows
- **Running Instances** — List actively running workflow instances filtered by workflow name to monitor what's currently executing
- **Execution Details** — Get deep state details for any workflow execution including input/output mappings, task-by-task trace histories, and exceptions
- **Workflow Search** — Search across all workflow executions using Elasticsearch queries, filtering by status, correlation ID, or workflow type

### How it works

1. Subscribe to this server
2. Enter your Orkes Access Key ID, Access Key Secret, and Base URL
3. Start monitoring your orchestrations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Platform engineers** — monitor running workflows and quickly identify stuck or failed executions without opening the Conductor UI
- **DevOps teams** — search execution history for failure patterns and audit workflow definitions during incident response
- **Architects** — inspect workflow graphs and task definitions to understand orchestration dependencies


## Available Tools
- **list_workflow_defs**: List all registered overarching Workflow Definitions via Orkes API
- **get_workflow_def**: Get a specific Workflow Definition explicitly by name
- **list_task_defs**: List all explicitly registered Task Definitions via Conductor API
- **list_running**: List active, running workflow instances by explicit workflow name
- **get_execution**: Get deep state details of a specific Workflow Execution
- **search_workflows**: Perform an elastic Search across all Workflow executions


## Installation & Usage

To install and use the **Orkes Conductor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/orkes-conductor](https://vinkius.com/mcp/orkes-conductor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
