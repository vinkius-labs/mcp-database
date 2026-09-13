# Water Coning Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/water-coning-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [oil-and-gas](../categories/oil-and-gas.md)

Predict water coning behavior and breakthrough timing in oil reservoirs.

## Description
This MCP server provides specialized tools for petroleum engineers to predict water coning in oil reservoirs with bottom water. It allows for calculating the `get_critical_coning_rate` to maintain stable production, estimating the `predict_breakthrough_time` to anticipate water arrival, and modeling the `calculate_water_cut_evolution` to understand fluid composition changes. Additionally, users can `analyze_well_geometry_impact` to evaluate how horizontal well configurations affect coning risks.


## Available Tools (4)
- **analyze_well_geometry_impact**: Evaluates impact of horizontal vs vertical well configuration
- **calculate_water_cut_evolution**: Predicts volume of water relative to oil over time
- **get_critical_coning_rate**: Determines the maximum safe production rate
- **predict_breakthrough_time**: Estimates time until water reaches wellbore


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Water Coning Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the maximum safe production rate for an oil zone with 50m thickness and a mobility ratio of 2.5, assuming no impermeable barrier?"

**🤖 AI Agent:**
> The maximum safe production rate is 450 barrels per day, which is classified as Stable.

---

**👤 You:**
> "If I produce at 600 barrels per day with a critical rate of 450, how long until water breakthrough?"

**🤖 AI Agent:**
> Water breakthrough is predicted to be Immediate.

---

**👤 You:**
> "How much will the water cut be 500 hours after a breakthrough that occurred at 200 hours, given a production rate of 500?"

**🤖 AI Agent:**
> The water cut fraction is 0.65, with a total fluid volume of 250,000 barrels.


## ❓ FAQ

**Q: How do I prevent water coning?**
You can use the `get_critical_coning_rate` tool to determine the maximum safe production rate that keeps the water-oil interface stable.

**Q: Can I model horizontal wells?**
Yes, the `analyze_well_geometry_impact` tool evaluates how horizontal well configurations reduce coning risks compared to vertical wells.

**Q: How is water breakthrough predicted?**
The `predict_breakthrough_time` tool estimates the duration until water reaches the wellbore based on production rates and critical coning thresholds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/water-coning-model](https://vinkius.com/en/ai-agent-connect/water-coning-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Water Coning Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `water-coning-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Water Coning Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "water-coning-model": {
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
