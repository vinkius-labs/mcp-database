# Conduit MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/conduit)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/conduit-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/conduit-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI agent to observe data streams, manage integration pipelines, and monitor nodes on the Conduit platform.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Conduit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve the current status of all major pipelines running in the production Conduit instance."

**🤖 AI Agent:**
> I checked your pipelines successfully. Of the 8 tracked major pipelines running on the queried instance: 7 are currently marked as 'Running' with no latency spikes or recorded disruption alerts. Pipeline ID 'PG_to_Snowflake_04' is however marked 'Degraded' due to a destination connector timeout 4 minutes ago. Do you want further logs related to this degraded element specifically to review the exact recorded error response logged safely here?

---

**👤 You:**
> "Check if there's a configured destination connector named 's3-analytics-bucket' and briefly describe its configuration parameters."

**🤖 AI Agent:**
> Yes, I located the 's3-analytics-bucket' destination connector attached to your integration pipelines successfully. This configured destination strictly utilizes the official 'builtin:s3' plugin structure. The setup parameters authenticate via attached AWS Keys (redacted), targeting an external region of 'us-east-1', and output streams correctly in a structured JSON payload referencing an established logical path.

---

**👤 You:**
> "Pause the pipeline 'MySQL-to-Kafka' immediately."

**🤖 AI Agent:**
> I'm sorry, but for safety reasons, I can only inspect pipelines and display logs. I cannot pause, modify, or delete pipelines. Please use the Conduit dashboard to execute this action.


## Installation & Usage

To install and use the **Conduit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/conduit](https://vinkius.com/mcp/conduit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
