# Flystack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flystack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Manage cloud infrastructure — audit deployments, clusters, and metrics via AI.

## Description
Empower your AI agent to orchestrate your entire cloud infrastructure and deployment auditing workflow with **Flystack**, the comprehensive source for programmable infrastructure data. By connecting Flystack to your agent, you transform complex DevOps tasks into a natural conversation. Your agent can instantly retrieve active deployments, audit cluster health, and monitor performance metrics without you ever touching a cloud console. Whether you are conducting system audits or managing application scaling, your agent acts as a real-time infrastructure consultant, ensuring your data is always comprehensive and up-to-the-minute.

### What you can do

- **Deployment Auditing** — Retrieve high-resolution details for all active deployments, including status, region, and creation metadata.
- **Cluster Oversight** — Audit the health and configuration of your infrastructure clusters to maintain strict organizational control.
- **Performance Intelligence** — Query real-time metrics including CPU and memory usage to understand the operational scale of your applications instantly.
- **Resource Discovery** — Retrieve detailed metadata for specific deployment IDs to assist in deep-dive infrastructure classification.
- **Operational Monitoring** — Check API status to ensure your infrastructure research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your Flystack API Key
3. Start managing your infrastructure intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers & CISOs** — monitor infrastructure state and retrieve official metadata straight from your workflow.
- **Backend Developers** — verify deployment statuses and audit cluster performance without manual searching.
- **Site Reliability Engineers** — perform rapid audits of system metrics and identify relevant resource markers through natural language.
- **Operations Leads** — automate infrastructure data querying to orchestrate cross-functional technical teams smoothly.


## Available Tools
- **check_api_status**: Check if the Flystack service is operational
- **get_cluster_metrics**: Get real-time performance metrics for a specific cluster
- **get_deployment_details**: Get full details for a specific deployment by ID
- **list_flystack_clusters**: List all infrastructure clusters in your Flystack account
- **list_flystack_deployments**: List all active deployments in your Flystack account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flystack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active deployments using Flystack."

**🤖 AI Agent:**
> I've retrieved the list of deployments! You have 3 active services, including 'web-production' and 'api-gateway'. Would you like the full details or performance metrics for any of these?

---

**👤 You:**
> "What are the metrics for cluster ID 'cluster-123'?"

**🤖 AI Agent:**
> I've retrieved the real-time metrics for cluster-123! The CPU usage is currently 45% and memory is at 60%. I can assist you with an audit of specific deployment IDs within this cluster if you'd like.

---

**👤 You:**
> "Show details for deployment 'api-gateway'."

**🤖 AI Agent:**
> I've identified the deployment 'api-gateway'! It is running in the 'us-east-1' region and was last updated 2 days ago. I can provide the unique ID and cluster metadata to help you identify it in your workflow.


## ❓ FAQ

**Q: How do I find my Flystack API Key?**
Log in to your [**Flystack dashboard**](https://app.flystack.dev/), go to your account settings or API section, and generate a new token. Copy and paste it below.

**Q: Does it support real-time metrics?**
Yes. The `get_cluster_metrics` tool retrieves the latest available CPU and memory usage metadata for your specified infrastructure cluster.

**Q: Can the agent list multiple deployments?**
Yes. The `list_flystack_deployments` tool provides a comprehensive list of all active deployments in your account instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flystack](https://vinkius.com/mcp/flystack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flystack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `flystack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flystack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flystack": {
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
