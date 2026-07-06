# OpenCost (K8s Cost) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opencost-k8s-cost)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Monitor and analyze Kubernetes infrastructure costs — query workload allocations, backing assets, and cloud billing directly from your AI agent.

## Description
Connect your **OpenCost** instance to any AI agent to gain real-time visibility into your Kubernetes spending and infrastructure efficiency through natural language.

### What you can do

- **Workload Allocation** — Query costs and resources allocated to clusters, nodes, namespaces, controllers, and pods using `get_allocation`.
- **Asset Inspection** — Retrieve backing cost data for physical infrastructure like Nodes, Disks, and Load Balancers via `get_assets`.
- **Cloud Billing Integration** — Access AWS CUR, Azure Export, and GCP Billing data directly with `get_cloud_cost` to reconcile K8s costs with provider bills.
- **Third-Party Costs** — Track external service expenses (e.g., Datadog, MongoDB Atlas) using custom cost timeseries and total summary tools.
- **Granular Filtering** — Aggregate data by labels, annotations, or service levels to understand exactly where your budget is going.

### How it works

1. Subscribe to this server
2. Enter your OpenCost API Base URL
3. Start auditing your cloud spend from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps & Platform Engineers** — Identify expensive namespaces or orphaned resources without manual dashboard diving.
- **FinOps Teams** — Reconcile internal Kubernetes allocations with external cloud provider billing reports instantly.
- **Engineering Managers** — Get quick summaries of project-based costs to stay within budget during development cycles.


## Available Tools (6)
- **get_allocation**: Query costs and resources allocated to Kubernetes workloads
- **get_cloud_cost**: Retrieve cloud cost data directly from cloud provider billing reports
- **get_custom_cost_timeseries**: g., Datadog, MongoDB Atlas).

Get samples of third-party service costs over time steps
- **get_custom_cost_total**: Get summary of third-party costs over a window
- **set_log_level**: Change OpenCost log level at runtime
- **get_assets**: Retrieve backing cost data broken down by individual assets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenCost (K8s Cost)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the cost allocation for all namespaces over the last 7 days."

**🤖 AI Agent:**
> I've retrieved the allocation data for the last 7 days. The 'production' namespace accounts for 65% of the spend ($420.50), followed by 'staging' at 20% ($130.00). Would you like to see the breakdown by controller kind?

---

**👤 You:**
> "What are the backing asset costs for our nodes today?"

**🤖 AI Agent:**
> Querying asset data... For today, your cluster nodes have incurred a cost of $45.20. This includes compute costs for 12 m5.large instances and associated EBS volumes. No load balancer costs were detected in this window.

---

**👤 You:**
> "Get the total summary for third-party service costs for the current month."

**🤖 AI Agent:**
> The total custom costs for this month sum up to $1,250.00. The largest contributors are Datadog ($800.00) and MongoDB Atlas ($450.00). Would you like to see the daily timeseries for these services?


## ❓ FAQ

**Q: Can I see costs grouped by a specific Kubernetes namespace?**
Yes. Use the `get_allocation` tool and set the `aggregate` parameter to 'namespace'. You can also specify a `window` like '7d' to see trends over the last week.

**Q: Does this server support viewing external cloud provider billing?**
Absolutely. The `get_cloud_cost` tool retrieves data directly from cloud provider billing reports (AWS CUR, Azure Export, GCP Billing) to give you a complete financial picture.

**Q: Can I track costs for non-Kubernetes services like Datadog?**
Yes, if configured in your OpenCost instance, you can use `get_custom_cost_total` or `get_custom_cost_timeseries` to query costs for third-party SaaS and infrastructure services.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opencost-k8s-cost](https://vinkius.com/mcp/opencost-k8s-cost)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenCost (K8s Cost)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `opencost-k8s-cost` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenCost (K8s Cost)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opencost-k8s-cost": {
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
