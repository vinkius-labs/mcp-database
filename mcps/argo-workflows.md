# Argo Workflows MCP Server

Automate Kubernetes orchestrations via Argo Workflows — monitor, list, and inspect active pods, crons, and workflow templates directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/argo-workflows)

## Overview
**Category:** loved-by-devs
**Tools Count:** 6

## Description
Connect your **Argo Workflows** cluster to any AI agent and take full control of your infrastructure orchestration through natural conversation.

### What you can do

- **Active Workflows** — List and query all running, pending, or recently completed workflow executions across your Kubernetes namespaces
- **Deep Inspection** — Dive into specific workflow instances to inspect their precise resource trees, node statuses, and pod parameters to catch failures
- **Templates & Crons** — Browse parameterized, reusable WorkflowTemplates and analyze recurring CronWorkflows orchestrating scheduled jobs
- **Historical Archives** — Search archived workflows that hit your database to understand historical infrastructure patterns

### How it works

1. Subscribe to this server
2. Enter your Argo Cluster Server URL and RBAC Bearer Token
3. Start querying your execution trees from Claude, Cursor, or any MCP-compatible client

No more wrestling with `kubectl` CLI tools or constantly refreshing the Argo Web UI to find out why a step failed. Your AI acts as your ultimate DevOps copilot.

### Who is this for?

- **DevOps & Platform Teams** — debug pipeline failures, check node statuses, and audit running jobs without leaving your terminal or chat workflow
- **Data Engineers** — monitor complex ETL workflows and scheduled cron operations seamlessly
- **SREs** — quickly query the health of the Argo server and retrieve historical archiving metrics


## Available Tools
- **list_workflows**: List workflows in a Kubernetes namespace
- **get_workflow**: Get detailed resource tree and status for an Argo workflow
- **list_workflow_templates**: List workflow templates defined in a namespace
- **list_cron_workflows**: List scheduled cron workflows in a namespace
- **list_archived_workflows**: List archived workflows from Argo history
- **get_server_info**: Get Argo Workflows server information


## Installation & Usage

To install and use the **Argo Workflows** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/argo-workflows](https://vinkius.com/mcp/argo-workflows)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
