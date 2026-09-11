# Lifting Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/lifting-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate production costs per barrel, analyze cost trends, and benchmark performance.

## Description
This MCP server provides essential tools for oil and gas production cost analysis. It allows AI agents to calculate the unit cost per barrel using `get_unit_cost`, track cost fluctuations over time with `get_cost_trend`, evaluate performance against industry standards via `compare_to_benchmark`, and examine the breakdown of fixed and variable expenses through `get_cost_composition`.


## Available Tools (4)
- **get_unit_cost**: Calculates the cost per barrel for a specific period and asset
- **compare_to_benchmark**: Evaluates the asset's unit cost against industry-standard performance levels
- **get_cost_composition**: Provides a granular breakdown of fixed vs. variable costs and specific cost categories
- **get_cost_trend**: Analyzes how the cost per barrel changes over a sequence of time periods


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lifting Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the unit cost for asset ASSET-123 in 2023-Q1?"

**🤖 AI Agent:**
> The unit cost for ASSET-123 in 2023-Q1 was $12.50 per barrel, with a total operating expense of $1,250,000 and a total volume of 100,000 barrels.

---

**👤 You:**
> "Is asset ASSET-456 performing well compared to the global standard for 2023-Q2?"

**🤖 AI Agent:**
> Yes, ASSET-456 is outperforming the global standard. Its unit cost is $10.00, which is $2.00 lower than the benchmark value of $12.00.

---

**👤 You:**
> "Show me the cost composition for ASSET-789 in 2023-Q3."

**🤖 AI Agent:**
> For ASSET-789 in 2023-Q3, the fixed costs totaled $500,000 and variable costs totaled $300,000, resulting in a fixed-to-variable cost ratio of 1.67.


## ❓ FAQ

**Q: How do I calculate the cost per barrel for a specific asset?**
You can use the `get_unit_cost` tool by providing the asset ID and the desired time period.

**Q: Can I compare my production costs to industry standards?**
Yes, the `compare_to_benchmark` tool allows you to compare your asset's unit cost against regional, global, or internal peer benchmarks.

**Q: How can I see if my costs are increasing or decreasing?**
Use the `get_cost_trend` tool to analyze how the cost per barrel changes over a sequence of time periods.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/lifting-cost-calculator](https://vinkius.com/en/ai-agent-connect/lifting-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lifting Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lifting-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lifting Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lifting-cost-calculator": {
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
