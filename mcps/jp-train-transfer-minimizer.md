# jp-train-transfer-minimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/jp-train-transfer-minimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Calculate precise Japanese train route metrics including transfer penalties.

## Description
This MCP server provides deterministic tools to evaluate Japanese train routes. It calculates total travel time, the number of transfers, and a specific transfer penalty to determine the effective travel time. Use `calculate_route_metrics` to get a full breakdown of a journey, `compare_route_efficiency` to decide between two different paths, or `validate_segment_integrity` to verify individual route segments.


## Available Tools (3)
- **calculate_route_metrics**: 
- **compare_route_efficiency**: 
- **validate_segment_integrity**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **jp-train-transfer-minimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the metrics for a route with two segments: Yamanote Line for 15 minutes (no transfer) and Chuo Line for 20 minutes (requires transfer)."

**🤖 AI Agent:**
> Total travel time is 35 minutes, total transfers is 1, transfer penalty is 5 minutes, and effective travel time is 40 minutes.

---

**👤 You:**
> "Which route is better: Route A (30 mins, 0 transfers) or Route B (20 mins, 2 transfers)?"

**🤖 AI Agent:**
> Route A is better. Route A has an effective travel time of 30 minutes, while Route B has an effective travel time of 30 minutes. Since effective times are equal, Route A is better because it has fewer transfers.

---

**👤 You:**
> "Check if this segment is valid: { "lineName": "Shinkansen", "travelTimeMin": 120, "transferRequired": false }"

**🤖 AI Agent:**
> The segment is valid.


## ❓ FAQ

**Q: How is the transfer penalty calculated?**
The transfer penalty is calculated by multiplying the total number of transfers by 5 minutes, representing the average time spent walking and waiting.

**Q: Can I compare two different routes?**
Yes, you can use the `compare_route_efficiency` tool to determine which route is better based on effective travel time.

**Q: What is effective travel time?**
Effective travel time is the sum of the actual time spent on trains and the calculated transfer penalty.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/jp-train-transfer-minimizer](https://vinkius.com/ai-agent-connect/jp-train-transfer-minimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **jp-train-transfer-minimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jp-train-transfer-minimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **jp-train-transfer-minimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jp-train-transfer-minimizer": {
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
