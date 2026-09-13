# Production Allocation Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/production-allocation-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Distribute commingled reservoir production volumes across specific geological zones or wells.

## Description
This MCP server provides specialized engineering tools for reservoir management. It allows AI agents to calculate production splits using methodologies like `get_allocation_by_method` (well test, production logging, or tracer), evaluate how physical properties influence distribution via `get_zone_contribution_analysis`, and monitor mass balance accuracy with `get_historical_reconciliation_report`. It also includes `get_tracer_efficiency_check` to validate tracer-based recovery rates.


## Available Tools (4)
- **get_allocation_by_method**: Calculates the production split for a set of zones using a specific measurement technique
- **get_historical_reconciliation_report**: 
- **get_tracer_efficiency_check**: Specifically assesses the validity of a tracer-based allocation based on tracer recovery rates
- **get_zone_contribution_analysis**: Evaluates how changes in zone physical properties impact the total production distribution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Production Allocation Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the production split for a total of 5000 barrels using the well_test method with two zones: Zone A with a metric value of 60 and Zone B with 40."

**🤖 AI Agent:**
> The allocated production is 3000 barrels for Zone A and 2000 barrels for Zone B.

---

**👤 You:**
> "Analyze the contribution of zones where the total production is 1000 and Zone 1 has a property weight of 7 and Zone 2 has a property weight of 3."

**🤖 AI Agent:**
> Zone 1 contributes 700 units and Zone 2 contributes 300 units.

---

**👤 You:**
> "Check tracer efficiency if 100 units were injected, 95 units were recovered, and Zone X has a concentration of 50."

**🤖 AI Agent:**
> The recovery rate is 95%, and the allocated volume for Zone X is 47.5 units.


## ❓ FAQ

**Q: What methodologies are supported for production splitting?**
The server supports well test, production logging, and tracer-based methodologies through the `get_allocation_by_method` tool.

**Q: How can I check if my tracer recovery is valid?**
You can use the `get_tracer_efficiency_check` tool to assess recovery rates and validate zone-specific allocations.

**Q: Can I analyze historical allocation accuracy?**
Yes, the `get_historical_reconciliation_report` tool analyzes the delta between estimated volumes and actual measured totals over time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/production-allocation-model](https://vinkius.com/en/ai-agent-connect/production-allocation-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Production Allocation Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `production-allocation-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Production Allocation Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "production-allocation-model": {
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
