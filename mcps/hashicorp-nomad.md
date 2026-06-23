# HashiCorp Nomad MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hashicorp-nomad)
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


## Available Tools (10)
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


## ❓ FAQ

**Q: How do I get my Nomad Address?**
Your Nomad Address is the URL where your Nomad server is reachable, usually including the port (e.g., http://nomad.example.com:4646).

**Q: Is an ACL Token required?**
Only if ACLs are enabled on your Nomad cluster. If enabled, you must provide a Secret ID with sufficient permissions to query the requested resources.

**Q: Can I use namespaces with this server?**
Yes! You can specify a target namespace in the authentication settings. The server will then filter all job and allocation queries to that specific namespace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hashicorp-nomad](https://vinkius.com/mcp/hashicorp-nomad)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HashiCorp Nomad** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hashicorp-nomad` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HashiCorp Nomad** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hashicorp-nomad": {
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
