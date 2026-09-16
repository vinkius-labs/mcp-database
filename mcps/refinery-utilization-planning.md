# Refinery Utilization Planning MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/refinery-utilization-planning)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Optimize refinery throughput, maintenance timing, and inventory levels.

## Description
This MCP server provides advanced optimization tools for refinery operations. It connects AI agents to critical planning functions including `calculate_optimal_run_rates` for throughput efficiency, `evaluate_turnaround_impact` for maintenance risk assessment, `analyze_seasonal_variations` for demand pattern analysis, and `optimize_inventory_strategy` for stock level management. It helps maintain operational stability by respecting turndown limits and managing inventory buffers against market demand.


## Available Tools (4)
- **calculate_optimal_run_rates**: Determines the most efficient throughput levels for a refinery over a specific timeframe
- **evaluate_turnaround_impact**: Assesses how scheduled maintenance affects the ability to meet market demand and inventory targets
- **optimize_inventory_strategy**: Calculates the ideal product stock levels required to mitigate risks from maintenance and demand spikes
- **analyze_seasonal_variations**: Identifies how shifts in product demand throughout the year should influence refinery operating modes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Refinery Utilization Planning** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the optimal run rate given a demand of 500 units and a maintenance window next week?"

**🤖 AI Agent:**
> The optimal run rate is 450 units to ensure sufficient inventory is built up before the scheduled maintenance window.

---

**👤 You:**
> "Will my current inventory cover the upcoming unit turnaround?"

**🤖 AI Agent:**
> No, the current inventory levels are insufficient to meet the projected demand during the turnaround; a buffer increase is recommended.

---

**👤 You:**
> "How should I adjust operations for the summer peak demand?"

**🤖 AI Agent:**
> Based on seasonal analysis, you should increase throughput by 15% to prepare for the summer driving season demand spike.


## ❓ FAQ

**Q: How can I determine the best throughput for my facility?**
You can use the `calculate_optimal_run_rates` tool to determine the most efficient throughput levels based on your demand forecast and maintenance schedule.

**Q: How does the server handle maintenance downtime?**
The `evaluate_turnaround_impact` tool assesses how scheduled maintenance affects your ability to meet market demand and identifies potential inventory risks.

**Q: Can I optimize my safety stock levels?**
Yes, the `optimize_inventory_strategy` tool calculates ideal product stock levels and safety stock requirements to mitigate risks from demand spikes or maintenance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/refinery-utilization-planning](https://vinkius.com/en/ai-agent-connect/refinery-utilization-planning)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Refinery Utilization Planning** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `refinery-utilization-planning` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Refinery Utilization Planning** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "refinery-utilization-planning": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
