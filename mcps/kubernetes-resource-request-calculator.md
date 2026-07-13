# Kubernetes Resource Request Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kubernetes-resource-request-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Computes Kubernetes CPU/memory requests and limits from observed usage metrics (p50/p95/p99).

## Description
The Kubernetes Resource Request Calculator automates the derivation of optimized pod resource specifications. By analyzing historical usage percentiles (p50, p95, or p99), it calculates precise CPU and memory requests and limits using a configurable multiplier. The tool also validates scaling ratios against best practices and projects total cluster demand based on replica counts. Use `generate_resource_specification` to create configurations, `validate_scaling_ratio` to check burst boundaries, and `estimate_cluster_demand` for fleet-wide resource planning.


## Available Tools (3)
- **estimate_cluster_demand**: Projects the total resource requirements for a deployment based on pod specifications and replica count
- **generate_resource_specification**: Generates a complete resource configuration based on usage history
- **validate_scaling_ratio**: Verifies if a specific limit-to-request ratio stays within recommended operational boundaries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kubernetes Resource Request Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a resource spec using p95 CPU of 0.5, p95 memory of 512MB (536870912 bytes), and a multiplier of 1.5."

**🤖 AI Agent:**
> CPU Request: 0.5 cores, CPU Limit: 0.75 cores, Memory Request: 536870912 bytes, Memory Limit: 805306368 bytes, QoS Class: Burstable.

---

**👤 You:**
> "Is a scaling ratio of 2.0 considered safe?"

**🤖 AI Agent:**
> The ratio 2.0 is classified as being in the 'Aggressive' zone.

---

**👤 You:**
> "If I have 10 replicas, each needing 0.2 CPU and 256MB memory, what is the total demand?"

**🤖 AI Agent:**
> Total CPU Demand: 2.0 cores, Total Memory Demand: 2684354560 bytes.


## ❓ FAQ

**Q: How does the tool calculate CPU and memory requests?**
The `generate_resource_specification` tool looks up the value in your provided metrics (p50, p95, or p99) that matches your chosen strategy percentile and sets that as the request.

**Q: What is a 'Guaranteed' QoS class?**
A pod is in the Guaranteed class if both its CPU request equals its limit and its memory request equals its limit.

**Q: Can I use this to plan for large-scale deployments?**
Yes, you can use `estimate_cluster_demand` to project the total CPU and memory footprint required for any number of replicas.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kubernetes-resource-request-calculator](https://vinkius.com/mcp/kubernetes-resource-request-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kubernetes Resource Request Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kubernetes-resource-request-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kubernetes Resource Request Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kubernetes-resource-request-calculator": {
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
