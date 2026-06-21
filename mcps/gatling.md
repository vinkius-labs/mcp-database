# Gatling MCP Server

Manage load testing via Gatling Enterprise — list and start simulations, monitor test runs and request stats, and handle generator pools directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gatling)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **Gatling Enterprise** account to any AI agent and take full control of your performance testing and high-scale load simulation through natural conversation.

### What you can do

- **Simulation Orchestration** — List all Gatling simulations defining load scenarios and retrieve IDs, class names, and team associations natively
- **Live Test Execution** — Trigger new performance test runs on Gatling Enterprise infrastructure and retrieve unique run IDs flawlessly
- **Test Run Monitoring** — Track execution progress, statuses, and peak virtual user (VU) counts for ongoing or completed simulations synchronously
- **Detailed Stats Retrieval** — Access full run details including request statistics, error counts, and injection start/end times limitlessly
- **Team & Quota Oversight** — Enumerate teams registered in Gatling Enterprise and monitor member counts and credit quotas securely
- **Artifact Management** — List uploaded test packages and artifacts to verify versions and upload timestamps across your environment
- **Resource Pool Auditing** — Retrieve the list of load generator pools, identifying regions and instance counts to verify scaling capacity
- **Autonomous Aborting** — Stop all load generators for a running simulation immediately to manage system resources and prevent overruns

### How it works

1. Subscribe to this server
2. Enter your Gatling Enterprise API Token (found in Settings > API Tokens)
3. Start managing your load testing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Performance & QA Engineers** — trigger load tests and monitor simulation results without manual dashboard checks
- **SRE & DevOps Teams** — audit team quotas and verify load generator pool capacity using natural language
- **Developers** — test and debug performance scenario configurations and verify request stats in real-time
- **Ops Managers** — monitor virtual user peaks and credit consumption through the chat interface


## Available Tools
- **list_simulations**: Simulations define load scenarios with VU populations. Returns names, IDs, class names, and team associations.

List all simulations on Gatling Enterprise
- **get_simulation**: Get full details of a Gatling simulation
- **start_simulation**: Returns run ID.

Start a Gatling simulation run
- **abort_simulation**: Abort a running Gatling simulation
- **list_runs**: List runs for a Gatling simulation
- **get_run**: Get full details of a Gatling run
- **list_teams**: List teams on Gatling Enterprise
- **list_packages**: List uploaded packages/artifacts on Gatling Enterprise
- **list_tokens**: List API tokens on Gatling Enterprise
- **list_pools**: List load generator pools on Gatling Enterprise


## Installation & Usage

To install and use the **Gatling** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gatling](https://vinkius.com/mcp/gatling)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
