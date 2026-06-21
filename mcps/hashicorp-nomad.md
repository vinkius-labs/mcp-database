# HashiCorp Nomad MCP Server

Manage workloads and orchestration via Nomad — track jobs, nodes, and deployments directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hashicorp-nomad)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

## Description
Connect your **HashiCorp Nomad** cluster to your AI agent and take control of your orchestration and workload management through natural conversation.

### What you can do

- **Job Oversight** — List all registered jobs and fetch their complete configuration and current status.
- **Cluster Health** — Monitor active client nodes and retrieve detailed resource usage and status info.
- **Deployment Tracking** — Follow the progress of rolling updates and manage canary deployments.
- **Workload Management** — List all running instances (allocations) and inspect specific task details.
- **Operational Control** — Manually promote successful deployments or fail underperforming ones to trigger rollbacks.
- **Deep Inspection** — Fetch complete metadata for specific jobs, nodes, or allocations using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your Nomad Address and (Optional) ACL Token
3. Start managing your cluster from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps & SRE Engineers** — quickly check cluster health or job status without opening the Nomad UI.
- **Developers** — monitor the progress of your service deployments and task allocations in real-time.
- **Infrastructure Managers** — automate the retrieval of node and workload data for reporting and monitoring.


## Available Tools
- **fail_deployment**: Mark a deployment as failed
- **get_allocation**: Get specific allocation details
- **get_deployment**: Get specific deployment details
- **get_job**: Get specific job details
- **get_node**: Get specific node info
- **list_allocations**: List all task allocations
- **list_deployments**: List recent deployments
- **list_jobs**: List all Nomad jobs
- **list_nodes**: List all client nodes
- **promote_deployment**: Promote a deployment


## Installation & Usage

To install and use the **HashiCorp Nomad** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hashicorp-nomad](https://vinkius.com/mcp/hashicorp-nomad)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
