# OpenCost (K8s Cost) MCP Server

Monitor and analyze Kubernetes infrastructure costs — query workload allocations, backing assets, and cloud billing directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/opencost-k8s-cost)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 6

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


## Available Tools
- **get_allocation**: Query costs and resources allocated to Kubernetes workloads
- **get_assets**: Retrieve backing cost data broken down by individual assets
- **get_cloud_cost**: Retrieve cloud cost data directly from cloud provider billing reports
- **get_custom_cost_timeseries**: g., Datadog, MongoDB Atlas).

Get samples of third-party service costs over time steps
- **get_custom_cost_total**: Get summary of third-party costs over a window
- **set_log_level**: Change OpenCost log level at runtime


## Installation & Usage

To install and use the **OpenCost (K8s Cost)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opencost-k8s-cost](https://vinkius.com/mcp/opencost-k8s-cost)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
