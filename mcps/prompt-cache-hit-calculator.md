# Prompt Cache Hit Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/prompt-cache-hit-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Analyze prompt prefix caching performance, efficiency, and cost savings.

## Description
This MCP server provides deterministic analysis of prompt prefix caching strategies. It allows AI agents to evaluate how effectively cached prefixes are being utilized to reduce latency and costs. Use `analyze_cache_performance` to calculate hit rates and monetary savings, `evaluate_cache_optimization` to determine the ideal cache size based on prefix sharing, and `inspect_cache_dynamics` to monitor eviction rates and specific prefix match lengths.


## Available Tools (3)
- **analyze_cache_performance**: Provides a high-level overview of how well the cache is performing regarding hits, efficiency, and cost savings
- **evaluate_cache_optimization**: Identifies the ideal cache capacity and the degree of prefix overlap to guide infrastructure scaling
- **inspect_cache_dynamics**: Investigates the frequency of cache turnover and the specific overlap between individual requests


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Prompt Cache Hit Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze my cache performance with a cache size of 1000 tokens and a cost of 0.00002 per token."

**🤖 AI Agent:**
> The cache hit rate is 0.45, with a cache efficiency of 0.25. The total cache hit value saved is $0.12.

---

**👤 You:**
> "What is the optimal cache size for these request logs?"

**🤖 AI Agent:**
> The optimal cache size is 1540 tokens, with a prefix sharing ratio of 0.65.

---

**👤 You:**
> "Check the cache eviction rate for a 5000 token cache."

**🤖 AI Agent:**
> The cache eviction rate is 0.02, indicating a stable cache with low turnover.


## ❓ FAQ

**Q: How do I calculate the monetary value of my cache hits?**
You can use the `analyze_cache_performance` tool. By providing the `costPerToken` parameter, the tool calculates the total `cacheHitValue` based on the tokens saved during successful hits.

**Q: What determines the optimal cache size?**
The `evaluate_cache_optimization` tool determines the optimal cache size by calculating the 95th percentile of prefix lengths from your request logs.

**Q: How can I see if my cache is evicting too many items?**
Use the `inspect_cache_dynamics` tool. It provides the `cacheEvictionRate`, which is the number of evictions divided by the total cache capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/prompt-cache-hit-calculator](https://vinkius.com/ai-agent-connect/prompt-cache-hit-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Prompt Cache Hit Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `prompt-cache-hit-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Prompt Cache Hit Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "prompt-cache-hit-calculator": {
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
