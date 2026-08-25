# Maple Syrup Production Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/maple-syrup-production-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predict syrup yields, boiling times, and production costs.

## Description
This MCP server provides professional-grade calculation tools for maple syrup producers. It uses the Jones Rule of 86 to predict syrup yields from raw sap and calculates the energy requirements for evaporation. Producers can determine boiling times and fuel consumption based on fuel type, and even account for energy savings from reverse osmosis pre-concentration. Use `predict_syrup_yield` to estimate volume, `calculate_boiling_requirements` for evaporation logistics, and `analyze_production_economics` for detailed cost breakdowns.


## Available Tools (3)
- **analyze_production_economics**: Provides a detailed breakdown of the cost to produce a specific volume of syrup
- **calculate_boiling_requirements**: Calculates the duration of the boiling process and the energy/fuel needed to reach target density
- **predict_syrup_yield**: Predicts the total volume of finished syrup that can be produced from a given amount of sap


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Maple Syrup Production Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much syrup can I get from 500 gallons of sap with 2% Brix if I want 66.9% Brix syrup?"

**🤖 AI Agent:**
> From 500 gallons of sap at 2% Brix, you can produce approximately 15.15 gallons of finished syrup at 66.9% Brix.

---

**👤 You:**
> "Calculate the boiling requirements for 1000 gallons of sap at 2.5 Brix targeting 67 Brix using Propane."

**🤖 AI Agent:**
> To process 1000 gallons of sap at 2.5 Brix to a target of 67 Brix using Propane, you will need approximately 450 minutes of boiling time and will consume 120 units of fuel.

---

**👤 You:**
> "What is the production cost for 50 gallons of syrup if I have 1000 gallons of sap at 2% Brix and fuel costs $2.50 per unit?"

**🤖 AI Agent:**
> The total production cost for this batch is $187.50, resulting in a cost of $3.75 per gallon of finished syrup.


## ❓ FAQ

**Q: How accurate are the yield predictions?**
Yields are calculated using the Jones Rule of 86, a standard industry method for estimating syrup volume from sap sugar concentration.

**Q: Can I account for reverse osmosis?**
Yes, the `calculate_boiling_requirements` tool allows you to input a reverse osmosis concentration factor to reduce estimated boiling time and fuel needs.

**Q: What fuel types are supported?**
The engine supports standard fuels including Wood, Propane, Natural Gas, and Diesel.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/maple-syrup-production-engine](https://vinkius.com/ai-agent-connect/maple-syrup-production-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Maple Syrup Production Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `maple-syrup-production-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Maple Syrup Production Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "maple-syrup-production-engine": {
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
