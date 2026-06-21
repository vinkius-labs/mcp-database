# Conduit MCP Server

Equip your AI agent to observe data streams, manage integration pipelines, and monitor nodes on the Conduit platform.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/conduit)

## Overview
**Category:** developer-tools
**Tools Count:** 8

## Description
Connect your AI agent seamlessly with **Conduit**, the modern data integration and synchronization platform. Utilizing natural language interactions, users can instruct the AI to oversee active streaming health, check connectors, and extract pipeline logs without accessing the conventional web dashboard interfaces.

### What you can do

- **Pipeline Management** — Request status overviews of active, paused, or degraded data integration pipelines efficiently.
- **Connector Auditing** — Ask the agent to locate specific connectors (source or destination) mapped to your critical infrastructure.
- **Log Evaluation** — Fetch recent application logs or streaming output reports via conversation to debug integration errors on the fly.

### How it works

1. Append this integration into your AI application interface securely.
2. Authorize connections providing the target instance Base URL, corresponding API Key, and an active Admin Password if applicable.
3. Chat natively instructing your agent to inspect and orchestrate streams through plain text inputs directly.

### Who is this for?

- **Data Engineers** — Instantly review health metrics regarding continuous synchronization services running between complex databases.
- **DevOps Professionals** — Confirm that new pipeline deployments successfully connected endpoints after infrastructure modifications.
- **System Administrators** — Request aggregate tracking reports validating if crucial operational data streams function continuously overnight.


## Available Tools
- **get_run_status**: Returns detailed status, timing, and error information.

Retrieve the current status of a specific workflow run
- **get_workflow**: Returns source, destination, and current status.

Retrieve detailed information about a specific workflow
- **list_connections**: Retrieve a list of all active source and destination connections
- **list_available_destinations**: Retrieve available data destination connector types supported by Conduit
- **list_workflow_runs**: Returns the execution history with status and timestamps for each run.

Retrieve the history of runs for a specific workflow
- **list_available_sources**: Retrieve available data source connector types supported by Conduit
- **list_workflows**: Use this as a starting point to discover workflow IDs for subsequent operations.

Retrieve a list of all data integration workflows in Conduit
- **trigger_workflow**: Use list_workflows first to find the workflow ID.

Manually trigger a run for a specific workflow


## Installation & Usage

To install and use the **Conduit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/conduit](https://vinkius.com/mcp/conduit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
