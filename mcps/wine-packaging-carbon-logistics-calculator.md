# Wine Packaging Carbon & Logistics Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-packaging-carbon-logistics-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Calculate carbon footprint and shipping logistics for wine packaging.

## Description
This MCP server provides specialized tools to analyze the environmental and economic impact of wine packaging. Use `calculate_per_bottle_impact` to determine the CO2e footprint of a single bottle based on its weight, closure type, and transport distance. Use `calculate_case_logistics` to find the total weight of a shipping case. You can also use `compare_packaging_options` to evaluate the trade-offs between lightweight and premium glass, or `estimate_freight_cost_impact` to see how weight changes affect shipping expenses.


## Available Tools (4)
- **calculate_case_logistics**: Calculates the physical weight and shipping profile for a standard shipping case
- **calculate_per_bottle_impact**: Determines the specific carbon footprint of a single bottle of wine
- **compare_packaging_options**: Evaluates the environmental and logistic trade-offs between two different bottle weight profiles
- **estimate_freight_cost_impact**: Estimates how changes in bottle weight affect the economic cost of shipping


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Packaging Carbon & Logistics Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the carbon footprint of a 0.5kg bottle with a cork closure shipped 500km by road?"

**🤖 AI Agent:**
> The total carbon footprint for this bottle is 0.85 kg CO2e.

---

**👤 You:**
> "How much does a case of 12 bottles weigh if each bottle is 0.6kg and contains 0.75kg of wine?"

**🤖 AI Agent:**
> The total case weight is 16.2 kg.

---

**👤 You:**
> "Compare a 0.4kg lightweight bottle to a 0.7kg premium bottle for a 12-bottle case over 1000km by sea."

**🤖 AI Agent:**
> Switching to the lightweight bottle results in 4.2 kg of weight savings and a 15% reduction in carbon footprint.


## ❓ FAQ

**Q: How is the carbon footprint calculated?**
The footprint is calculated by summing the production impact of the glass and closure with the transport impact based on weight and distance.

**Q: Can I compare different bottle weights?**
Yes, use the `compare_packaging_options` tool to see the carbon and weight savings when switching to lighter bottles.

**Q: Does this tool account for shipping costs?**
Yes, the `estimate_freight_cost_impact` tool calculates how changes in bottle weight influence total freight expenses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-packaging-carbon-logistics-calculator](https://vinkius.com/ai-agent-connect/wine-packaging-carbon-logistics-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Packaging Carbon & Logistics Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-packaging-carbon-logistics-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Packaging Carbon & Logistics Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-packaging-carbon-logistics-calculator": {
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
