# Orkes Conductor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/orkes-conductor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Orchestrate microservice workflows via Orkes Conductor — list definitions, track running executions, search workflow history, and inspect task states from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Orkes Conductor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all registered workflow definitions."

**🤖 AI Agent:**
> Found 12 workflow definitions. 1) 'order-processing' v3 — 8 tasks, including payment validation and shipping triggers. 2) 'user-onboarding' v2 — 5 tasks with email verification fork. 3) 'data-pipeline-daily' v1 — 4 tasks for ETL orchestration. Want me to inspect the graph of any of these?

---

**👤 You:**
> "Are there any failed workflows in the last 24 hours?"

**🤖 AI Agent:**
> Found 3 failed executions in the last 24 hours. 1) order-processing (ID: abc-123) — failed at 'payment-validation' task at 14:23 UTC. Error: 'Gateway timeout'. 2) user-onboarding (ID: def-456) — failed at 'send-welcome-email' at 16:45. Error: 'SMTP connection refused'. 3) data-pipeline-daily (ID: ghi-789) — timed out at 'extract-transform' at 03:12. Want me to get the full execution trace for any?

---

**👤 You:**
> "How many instances of the order-processing workflow are currently running?"

**🤖 AI Agent:**
> 8 instances of 'order-processing' currently running. 5 are at the 'payment-validation' stage, 2 at 'shipping-trigger', and 1 at 'inventory-check'. Average execution time so far: 4.2 seconds. No instances are stuck or timed out. Want me to inspect one?


## ❓ FAQ

**Q: Can I search for failed workflows across my entire history?**
Yes. The search tool supports Elasticsearch query syntax — search by status (FAILED, TIMED_OUT), workflow type, date ranges, or correlation IDs. Ask your agent 'show me all failed workflows from the last 24 hours' and it returns matching executions with their IDs, failure reasons, and timestamps.

**Q: What's the difference between workflow definitions and running instances?**
Definitions are the blueprints — the graph schema with tasks, operators, and branching logic. Running instances are actual executions of those definitions, each with their own input data, current state, and task-by-task progress. Think of definitions as classes and instances as objects.

**Q: Does this integration support triggering new workflow executions?**
Currently, this integration focuses on observability — listing definitions, monitoring running instances, and searching execution history. It does not trigger new workflow executions. For launching workflows, use the Orkes Conductor UI or direct API calls.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/orkes-conductor](https://vinkius.com/mcp/orkes-conductor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Orkes Conductor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `orkes-conductor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Orkes Conductor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "orkes-conductor": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
