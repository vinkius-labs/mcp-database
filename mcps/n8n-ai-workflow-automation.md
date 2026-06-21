# n8n (AI Workflow Automation) MCP Server

Manage workflow automation via n8n — audit active workflows, track execution logs, and monitor credentials.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/n8n-ai-workflow-automation)

## Overview
**Category:** ship-it
**Tools Count:** 7

## Description
Connect your **n8n** instance to any AI agent and take full control of your node-based workflow automation, execution diagnostics, and project orchestration through natural conversation.

### What you can do

- **Workflow Orchestration** — List all managed automation workflows and retrieve detailed JSON logic nodes, including link mappings and trigger configurations directly from your agent
- **Execution Diagnostics** — Extract historical execution logs to track success/failure boundaries and retrieve absolute trace logs for rapid debugging of automation failures
- **Node-Level Inspection** — Deep-dive into specific execution IDs to extract bounded node-level output blocks and identify exact processing errors natively
- **Credential Audit** — List metadata mapping saved automation credentials to verify system types and IDs without exposing literal secure tokens
- **Collaborative Visibility** — Enumerate provisioned team users and assigned roles to verify access targets across your n8n infrastructure securely
- **Organizational Tags** — List arbitrary category tags used to group and sort complex workflow logic dimensions across your automation workspace
- **Metadata Inspection** — Retrieve precise graph representations for specific workflows to understand the underlying logic and data transformation flows instantly

### How it works

1. Subscribe to this server
2. Enter your n8n Base URL and API Key
3. Start managing your automation node from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Automation Engineers** — verify workflow designs and debug execution failures through natural conversation without manual dashboard navigation
- **Software Developers** — test node-based automation logic and retrieve execution traces directly from your workspace terminal
- **IT Operations Teams** — monitor automation health and audit credential mappings across multiple n8n instances efficiently


## Available Tools
- **list_instance_users**: List collaborators on the n8n instance
- **list_workflows**: List n8n automation workflows
- **list_stored_credentials**: List metadata for saved credentials
- **list_workflow_executions**: List recent workflow executions
- **get_execution_details**: Get trace logs for a specific execution
- **get_workflow_details**: Get details for a specific workflow
- **list_workflow_tags**: List workflow organizational tags


## Installation & Usage

To install and use the **n8n (AI Workflow Automation)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/n8n-ai-workflow-automation](https://vinkius.com/mcp/n8n-ai-workflow-automation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
