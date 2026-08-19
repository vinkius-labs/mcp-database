# OpenSearch Shard Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/opensearch-shard-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Deterministic AWS OpenSearch shard distribution and resource allocation calculator.

## Description
This MCP server provides precise calculations for AWS OpenSearch cluster architecture. Use `calculate_shard_distribution` to determine primary and total shard counts based on your index size and target shard size. Use `calculate_cluster_limits_and_health` to evaluate shard density per node and overall cluster stability. Finally, use `recommend_resource_and_performance_settings` to obtain optimized JVM heap sizes, garbage collection recommendations, and refresh intervals for your specific workload. It helps prevent common issues like excessive shard density or undersized JVM heaps.


## Available Tools (3)
- **calculate_cluster_limits_and_health**: 
- **calculate_shard_distribution**: 
- **recommend_resource_and_performance_settings**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenSearch Shard Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 500 GB of data across 10 indices. I want each shard to be 30 GB. How many shards do I need and how many replicas should I consider?"

**🤖 AI Agent:**
> For 500 GB across 10 indices with a 30 GB target, you will need 17 primary shards in total (2 per index, rounded up). If you use 1 replica, your total shard count will be 34.

---

**👤 You:**
> "My OpenSearch node has 64 GB of RAM. I am running a write-heavy workload. What are my recommended settings?"

**🤖 AI Agent:**
> For a 64 GB instance with a write-heavy workload, the recommended JVM heap size is 32 GB. It is recommended to use the G1GC garbage collector, and you should increase the refresh interval to accommodate high indexing volume.

---

**👤 You:**
> "I have 5000 total shards across 5 data nodes. Is this a problem?"

**🤖 AI Agent:**
> With 5000 total shards across 5 nodes, you have 1000 shards per node. This is at the upper limit of the recommended density and may impact performance.


## ❓ FAQ

**Q: How do I know if my shard density is too high?**
You can use the `calculate_cluster_limits_and_health` tool. It will return a flag if the shards per node exceeds the recommended limit of 1000.

**Q: Can this tool recommend JVM settings?**
Yes, the `recommend_resource_and_performance_settings` tool provides optimized JVM heap size, recommended garbage collection algorithms like G1GC, and translog flush thresholds.

**Q: What is the recommended shard size for OpenSearch?**
A good rule of thumb is to target a shard size between 10 and 50 GB. You can use `calculate_shard_distribution` to see how your specific index size fits these targets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/opensearch-shard-calculator](https://vinkius.com/ai-agent-connect/opensearch-shard-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenSearch Shard Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `opensearch-shard-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenSearch Shard Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opensearch-shard-calculator": {
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
