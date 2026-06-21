# Rancher MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rancher)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI to manage Kubernetes environments directly through Rancher, overseeing clusters, namespaces, and active pods.

## Description
Connect your **Rancher** Kubernetes management platform to your AI agent, allowing seamless orchestration of your container infrastructure directly from a chat interface. By integrating this server, your AI can introspect and interact with multiple remote Kubernetes clusters managed governed by your Rancher deployment.

### What you can do

- **Cluster Oversight** — List and examine the status of all managed clusters connected to your Rancher control plane.
- **Namespace Discovery** — Explore specific logical partitions (namespaces) within those clusters without digging into complex kubectl configuration.
- **Workload Management** — Access deployments, daemonsets, and statefulsets to observe operational health across environments.
- **Pod Introspection** — Query individual pod states, find crashing containers, and pull context faster than running manual CLI queries.

### How it works

1. Enable the MCP server integration.
2. Configure it with your Rancher Server URL and the generated Bearer Token for API authentication.
3. Instruct your AI to inspect a cluster, query specific namespaces, or detail the status of a specific pod.

### Who is this for?

- **DevOps Engineers** — Debug and query live cluster statuses interactively, bypassing the need to constantly switch context between terminals and UI dashboards.
- **Kubernetes Administrators** — Run automated queries to verify policies, scaling sets, and general deployment topologies rapidly.
- **Backend Developers** — Ensure microservices are running smoothly on target clusters and verify namespace health without complex local setups.


## Available Tools
- **get_cluster**: Retrieves details for a specific Kubernetes cluster
- **get_project**: Retrieves details for a specific Rancher project
- **list_apps**: Lists Helm applications installed in a project
- **list_catalogs**: Lists available Helm chart repositories (Catalogs)
- **list_clusters**: Lists all Kubernetes clusters managed by Rancher
- **list_namespaces**: Lists Kubernetes namespaces associated with a project
- **list_nodes**: Lists all nodes within a specific cluster
- **list_projects**: Use this to find project IDs.

Lists logical projects within a cluster
- **list_users**: Lists all user accounts in the Rancher platform
- **list_workloads**: Lists all Kubernetes workloads (Deployments, StatefulSets) in a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rancher** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Kubernetes clusters managed by my Rancher instance."

**🤖 AI Agent:**
> Through `list_clusters`, I have enumerated your environment. You have 2 visible instances: 'production-us-east' (State: Active) and 'staging-development' (State: Provisioning).

---

**👤 You:**
> "Query the namespaces available inside cluster 'c-8xk9z'."

**🤖 AI Agent:**
> I requested `list_namespaces` for the cluster ID 'c-8xk9z'. It contains several namespaces, including: 'default', 'kube-system', 'monitoring-setup', and 'frontend-tier'.

---

**👤 You:**
> "Check the status of the 'auth-service' pod located in the 'backend-production' namespace on cluster 'c-lq4x2'."

**🤖 AI Agent:**
> Checking pod metrics... Using `list_pods`, the 'auth-service' pod is marked 'Running', executing in the requested namespace. No crash loops were detected in its recent container history.


## ❓ FAQ

**Q: How do I generate a Bearer Token in Rancher?**
Log into your Rancher UI. Go to your User Profile menu and select 'API & Keys'. Create a new API Key with appropriate scopes. Combine the generated Access Key and Secret Key using a colon (`AccessKey:SecretKey`), or use the final Bearer Token provided to authenticate the MCP server.

**Q: Does the integration require direct cluster network access?**
No, the MCP server acts exclusively by pinging the overarching main Rancher Server API URL rather than connecting locally to standard cluster API endpoints separately. Your network configuration remains secure as it relies completely on the Rancher gateway role.

**Q: Can I deploy new workloads to my cluster via the chat interface?**
Currently, the server allows listing and fetching comprehensive statuses for namespaces, workloads, endpoints, clusters, and pods natively to observe the infrastructure state interactively without allowing unmanaged destructive configurations to roll out purely based on prompt.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rancher](https://vinkius.com/mcp/rancher)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rancher** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `rancher` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rancher** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rancher": {
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
