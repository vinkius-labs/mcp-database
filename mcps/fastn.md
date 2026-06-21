# Fastn MCP Server

Automate and execute low-code workflows via Fastn — manage flow definitions, monitor executions, and handle connector credentials directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fastn)

## Overview
**Category:** developer-tools
**Tools Count:** 16

## Description
Connect your **Fastn** account to any AI agent to orchestrate complex backend workflows and real-time API flows through natural language.

### What you can do

- **Flow Execution** — Trigger Fastn flows instantly with custom JSON payloads and receive real-time responses via the API sync layer.
- **Workflow Management** — List, create, update, and publish flow definitions across different tenants to maintain your business logic.
- **Execution Monitoring** — Track execution history and drill down into step-by-step traces to debug or audit automated processes.
- **Credential Handling** — Securely store, retrieve, and rotate credentials for your various connectors and third-party integrations.
- **Platform Insights** — Monitor your platform usage, including daily quotas, summary metrics, and active space configurations.

### How it works

1. Subscribe to this server
2. Provide your Fastn API Key and Space ID
3. Start executing and managing your backend logic from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — deploy, test, and trigger flows without leaving your code editor or terminal.
- **DevOps Engineers** — monitor execution traces and manage environment credentials programmatically through the agent.
- **Product Teams** — trigger business logic flows and check automation statuses via natural conversation.


## Available Tools
- **archive_workflow**: Deactivate / archive a flow
- **cancel_execution**: Cancel a running execution
- **create_workflow**: Create a new flow definition
- **execute_flow**: The input object must match the Request Schema defined in the flow trigger.

Execute a Fastn flow instantly (API Real-Time Sync)
- **get_credentials**: Retrieve stored credentials
- **get_execution**: Get full step-by-step execution trace
- **get_quota_daily**: Daily usage breakdown
- **get_quota_summary**: Usage summary
- **get_quota_usage**: Current usage against plan limits
- **get_workflow**: Get a flow full specification
- **list_executions**: List execution history for a tenant
- **list_workflows**: List all flow definitions for a tenant
- **publish_workflow**: Deploy / publish a flow
- **rotate_credentials**: Rotate credentials
- **store_credentials**: Store connector credentials
- **update_workflow**: Update a flow definition


## Installation & Usage

To install and use the **Fastn** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fastn](https://vinkius.com/mcp/fastn)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
