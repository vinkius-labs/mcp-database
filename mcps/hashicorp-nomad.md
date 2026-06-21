# HashiCorp Nomad MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hashicorp-nomad)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hashicorp-nomad-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hashicorp-nomad-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage workloads and orchestration via Nomad — track jobs, nodes, and deployments directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HashiCorp Nomad** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active jobs in the 'production' namespace."

**🤖 AI Agent:**
> Retrieving jobs... In the 'production' namespace, I found 5 active jobs: 'API-Gateway' (Service), 'Redis-Cluster' (Service), and 3 batch processing jobs. Would you like the detailed status for the API Gateway?

---

**👤 You:**
> "Check the status of all client nodes in the cluster."

**🤖 AI Agent:**
> Fetching cluster nodes... You have 12 registered client nodes. 10 are 'ready' and healthy, while 2 are currently 'down' or unreachable. Shall I retrieve the resource usage for the healthy nodes?

---

**👤 You:**
> "Promote the deployment with ID 'dep-98765'."

**🤖 AI Agent:**
> Promotion initiated... The deployment 'dep-98765' has been successfully promoted. The rolling update will now continue to the remaining allocations. I'll monitor the status for you.


## Installation & Usage

To install and use the **HashiCorp Nomad** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hashicorp-nomad](https://vinkius.com/mcp/hashicorp-nomad)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
