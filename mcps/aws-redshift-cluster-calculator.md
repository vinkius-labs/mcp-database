# AWS Redshift Cluster Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aws-redshift-cluster-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Deterministic sizing for AWS Redshift clusters, including node counts, concurrency scaling, and WLM configuration.

## Description
This MCP server provides precise sizing and configuration for AWS Redshift clusters. Use `calculate_cluster_size` to determine the required number of nodes based on data volume and hardware profiles like dc2, ds2, or ra3. Optimize your environment using `optimize_workload_performance` to manage concurrency scaling slots, distribution styles, and sort key strategies. Finally, use `configure_resource_management` to set up WLM queues and snapshot schedules. It acts as a bridge between your AI agent and AWS Redshift architecture planning.


## Available Tools (3)
- **calculate_cluster_size**: Determines the fundamental hardware requirements for the Redshift cluster
- **configure_resource_management**: Sets up the internal governance of the cluster, including memory allocation and data backups
- **optimize_workload_performance**: Provides configuration for query execution, scaling, and data organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWS Redshift Cluster Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many nodes do I need for 50TB of data using dc2 nodes?"

**🤖 AI Agent:**
> For 50TB of data on dc2 nodes, you will need a specific number of nodes based on the storage capacity of the dc2 tier. Please run `calculate_cluster_size` with 50 as the data volume to get the exact count.

---

**👤 You:**
> "Help me optimize a cluster with 5 nodes and 20 concurrent queries."

**🤖 AI Agent:**
> To optimize a 5-node cluster with 20 concurrent queries, use `optimize_workload_performance`. This will calculate available concurrency scaling slots and recommend a distribution style like 'even' or 'key' to maximize performance.

---

**👤 You:**
> "Set up a snapshot schedule for a 10-node cluster."

**🤖 AI Agent:**
> You can configure the snapshot schedule by calling `configure_resource_management` with 10 nodes and your preferred frequency (hourly, daily, or weekly).


## ❓ FAQ

**Q: How do I determine the number of nodes needed?**
You can use the `calculate_cluster_size` tool. Provide the total compressed data volume in TB and select your preferred node type (dc2, ds2, or ra3) to get the exact node count.

**Q: Can I configure WLM queues through this tool?**
Yes, the `configure_resource_management` tool allows you to define up to 8 WLM queues and allocate memory percentages to ensure efficient workload management.

**Q: What is the difference between compound and interleaved sort keys?**
When using `optimize_workload_performance`, you can choose between compound sort keys (prioritized sequence) or interleaved sort keys (multi-dimensional weight) depending on your query patterns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aws-redshift-cluster-calculator](https://vinkius.com/ai-agent-connect/aws-redshift-cluster-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AWS Redshift Cluster Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aws-redshift-cluster-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AWS Redshift Cluster Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aws-redshift-cluster-calculator": {
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
