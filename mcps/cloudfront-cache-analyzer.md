# CloudFront Cache Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/cloudfront-cache-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

Calculate AWS CloudFront cache hit ratios, origin load reduction, and TTL optimization.

## Description
This MCP server provides deterministic calculations for AWS CloudFront cache performance. Use `calculate_cache_metrics` to determine hit ratios, origin load reduction, and bandwidth delivery. Optimize your caching strategy with `get_ttl_optimization_advice` to find the ideal TTL, or use `calculate_stale_windows` to define SWR and SIE headers. You can also use `analyze_path_patterns` to evaluate caching health across different URL paths.


## Available Tools (4)
- **analyze_path_patterns**: Answers how cache behavior differs across different URL paths
- **get_ttl_optimization_advice**: Answers what adjustments should be made to the TTL to improve cache performance
- **calculate_cache_metrics**: Answers how efficient the current cache configuration is in terms of hit ratio, origin load, and data transfer
- **calculate_stale_windows**: Answers what supplementary caching headers should be used to improve availability and latency during revalidation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CloudFront Cache Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my cache metrics for 100MB objects at 10 requests per second with a 3600s TTL and 50ms origin latency."

**🤖 AI Agent:**
> Your cache hit ratio is 0.90, resulting in an origin load reduction of 9 requests per second and 900MB/s bandwidth to viewers.

---

**👤 You:**
> "My cache hit ratio is 0.65. What should I do?"

**🤖 AI Agent:**
> You should increase your TTL to improve the cache hit ratio.

---

**👤 You:**
> "What are the recommended stale windows for a 3600s TTL?"

**🤖 AI Agent:**
> The recommended stale-while-revalidate window is 300 seconds and the stale-if-error window is 86400 seconds.


## ❓ FAQ

**Q: How can I reduce the load on my origin server?**
You can use `calculate_cache_metrics` to see how much load is being reduced. Increasing your TTL via `get_ttl_optimization_advice` can also help increase the cache hit ratio and further reduce origin requests.

**Q: What is the best way to handle stale content?**
Use `calculate_stale_windows` to determine the appropriate durations for stale-while-revalidate and stale-if-error headers to improve availability.

**Q: Can I analyze multiple paths at once?**
Yes, the `analyze_path_patterns` tool allows you to evaluate the caching health across multiple defined path patterns in a single report.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/cloudfront-cache-analyzer](https://vinkius.com/ai-agent-connect/cloudfront-cache-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CloudFront Cache Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cloudfront-cache-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CloudFront Cache Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cloudfront-cache-analyzer": {
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
