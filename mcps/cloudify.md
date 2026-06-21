# Cloudify MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudify)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cloudify-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cloudify-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Orchestrate cloud infrastructure via Cloudify — manage blueprints, deployments, and monitor workflow executions directly from any AI agent.

## Description
Connect your **Cloudify Manager** to any AI agent and take full control of your multi-cloud orchestration through natural conversation.

### What you can do

- **Blueprint Management** — List and audit OASIS TOSCA blueprints parsing root Cloudify manager templates
- **Deployment Tracking** — Retrieve exact structural matching of actualized runtime schemas and manage infrastructure states
- **Workflow Executions** — Monitor install, uninstall, and heal transactions to track deployment events in real-time
- **Node Inspections** — Resolve deeply nested infrastructure nodes and audit lifecycle properties (started, created, deleted)
- **Plugin Auditing** — Discover installed Python abstractions for AWS, GCP, and other cloud integrations

### How it works

1. Subscribe to this server
2. Enter your Cloudify Manager URL and API Token
3. Start orchestrating your infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Cloud Engineers** — manage complex orchestration blueprints and deployments using natural language
- **DevOps Teams** — monitor workflow executions and node states without digging through the manager UI
- **Platform Architects** — audit multi-cloud integrations and plugin configurations across environments
- **SREs** — quickly identify failed executions and verify infrastructure lifecycle states


## Available Tools
- **list_blueprints**: Identify bounded logical arrays managing top-level orchestration schemas
- **get_blueprint**: Perform structural extraction of properties driving active blueprint schemas
- **list_deployments**: Retrieve the exact structural matching verifying actualized runtime schemas
- **get_deployment**: Extracts explicitly attached internal structural states pulling precise execution topologies
- **list_executions**: Identify precise active cluster limits spanning deployment workflow bounds
- **list_nodes**: Identify exact literal limits pushing specific instances routing orchestration rules
- **list_plugins**: Extracts explicit capabilities mapping native orchestration limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cloudify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all blueprints in Cloudify Manager"

**🤖 AI Agent:**
> I found 5 blueprints. The active ones are: 'aws-three-tier', 'gcp-k8s-cluster', and 'hybrid-db-template'. Which one would you like to inspect?

---

**👤 You:**
> "Show me the execution history for deployment 'web-app-prod'"

**🤖 AI Agent:**
> Retrieving executions for 'web-app-prod'... The last workflow was 'install' which finished successfully. There is a 'heal' execution from yesterday that was triggered automatically.

---

**👤 You:**
> "What nodes are currently in the 'started' state for deployment 'db-cluster'?"

**🤖 AI Agent:**
> Analyzing nodes for 'db-cluster'... I found 3 nodes in 'started' state: 'primary-node-1', 'replica-node-1', and 'load-balancer-internal'. All instances are healthy.


## Installation & Usage

To install and use the **Cloudify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudify](https://vinkius.com/mcp/cloudify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
