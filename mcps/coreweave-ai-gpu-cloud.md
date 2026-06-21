# CoreWeave (AI GPU Cloud) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coreweave-ai-gpu-cloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Manage high-performance AI infrastructure on CoreWeave — provision GPU clusters, configure VPCs, and orchestrate inference gateways directly from your AI agent.

## Description
Connect your **CoreWeave** account to any AI agent to manage specialized GPU cloud infrastructure through natural language conversation.

### What you can do

- **Kubernetes Clusters (CKS)** — List, create, and manage bare-metal Kubernetes clusters optimized for intensive AI and ML workloads.
- **Network Isolation (VPC)** — Configure Virtual Private Clouds to ensure secure, isolated networking for your compute resources.
- **Inference Gateways** — Orchestrate gateways for routing and authenticating traffic to your deployed AI models.
- **Deployment Monitoring** — List and inspect inference deployments to ensure your services are running at peak performance.
- **Resource Lifecycle** — Full CRUD operations for clusters, VPCs, and gateways to automate your infrastructure scaling.

### How it works

1. Subscribe to this server
2. Enter your CoreWeave API Token
3. Start managing your GPU cloud from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **ML Engineers** — Provision and scale GPU clusters without leaving your development environment.
- **DevOps Teams** — Automate VPC setup and gateway routing for production-grade AI services.
- **AI Researchers** — Quickly inspect cluster status and deployment health during model training or testing phases.


## Available Tools
- **get_vpc**: Get details for a specific VPC
- **create_capacity_claim**: Create a new Inference Capacity Claim
- **create_cluster**: Create a new CKS cluster
- **update_cluster**: Requires an updateMask in the payload.

Update a CKS cluster
- **update_deployment**: Update an Inference Deployment
- **update_gateway**: Update an Inference Gateway
- **update_vpc**: Update a VPC
- **create_deployment**: Create a new Inference Deployment
- **create_gateway**: Create a new Inference Gateway
- **create_vpc**: Create a new VPC
- **delete_capacity_claim**: Delete an Inference Capacity Claim
- **delete_cluster**: Delete a CKS cluster
- **delete_deployment**: Delete an Inference Deployment
- **delete_gateway**: Delete an Inference Gateway
- **delete_vpc**: Delete a VPC
- **get_cluster**: Get details for a specific CKS cluster
- **list_capacity_claims**: List all Inference Capacity Claims
- **list_clusters**: List all CoreWeave Kubernetes Service (CKS) clusters
- **list_deployments**: List all Inference Deployments
- **list_gateways**: List all Inference Gateways
- **list_vpcs**: List all Virtual Private Clouds (VPCs)
- **query_logs**: Query Loki logs
- **query_metrics**: Query Prometheus metrics
- **update_capacity_claim**: Update an Inference Capacity Claim


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CoreWeave (AI GPU Cloud)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active CoreWeave clusters."

**🤖 AI Agent:**
> I've retrieved your CKS clusters. You have 2 active clusters: 'production-gpu-1' (ID: cks-7721) and 'research-test-bed' (ID: cks-8832). Would you like details on either of them?

---

**👤 You:**
> "Show me the details for VPC ID vpc-99402."

**🤖 AI Agent:**
> Fetching VPC details... VPC 'vpc-99402' is currently active with CIDR block 10.0.0.0/16. It is configured for high-bandwidth interconnects between your GPU nodes.

---

**👤 You:**
> "List all inference deployments and gateways currently configured."

**🤖 AI Agent:**
> I've compiled the list. You have 3 active inference gateways routing traffic to 5 deployments, including your 'llama-3-70b-prod' service. All gateways are reporting healthy status.


## ❓ FAQ

**Q: Can I list all my active Kubernetes clusters across the CoreWeave infrastructure?**
Yes. By using the `list_clusters` tool, your agent will retrieve a complete list of all bare-metal Kubernetes clusters (CKS) managed under your account.

**Q: How do I check the specific network configuration of a VPC?**
You can use the `get_vpc` tool by providing the specific VPC ID. The agent will return detailed information about network isolation and configuration for that resource.

**Q: Is it possible to create a new inference gateway via the AI agent?**
Absolutely. Use the `create_gateway` tool with the required specification JSON. This allows you to set up routing and authentication for your AI model traffic programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coreweave-ai-gpu-cloud](https://vinkius.com/mcp/coreweave-ai-gpu-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CoreWeave (AI GPU Cloud)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `coreweave-ai-gpu-cloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CoreWeave (AI GPU Cloud)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coreweave-ai-gpu-cloud": {
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
