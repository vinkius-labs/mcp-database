# Electrical Panel Load Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/electrical-panel-load-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate residential electrical load requirements based on NEC Article 220 standards to determine panel capacity and conductor sizing.

## Description
This MCP server provides specialized tools for calculating residential electrical service requirements following the National Electrical Code (NEC) Article 220. It allows users to compute lighting loads based on square footage, calculate branch circuit demands, sum fixed appliance power requirements, and determine final panel specifications including amperage, recommended panel size, and main conductor gauge using `calculate_lighting_load`, `calculate_branch_circuit_load`, `calculate_appliance_load`, and `compute_panel_specification`.


## Available Tools (4)
- **calculate_appliance_load**: Calculate cumulative wattage for fixed appliances
- **calculate_branch_circuit_load**: Calculate total demand for small appliance and laundry circuits
- **calculate_lighting_load**: Calculate total lighting load based on square footage
- **compute_panel_specification**: Compute final electrical service requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Electrical Panel Load Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the lighting load for a 2500 square foot house."

**🤖 AI Agent:**
> The calculated lighting load for 2,500 sqft is 7,500 VA.

---

**👤 You:**
> "What is the total wattage for an electric range and a dishwasher?"

**🤖 AI Agent:**
> The cumulative appliance load for the electric range and dishwasher is 10,500 VA.

---

**👤 You:**
> "If my total demand is 24,000 VA, what panel size do I need?"

**🤖 AI Agent:**
> For a total demand of 24,000 VA, the required service is 200A, using a 200A panel and 3/0 AWG conductors.


## ❓ FAQ

**Q: How is the lighting load calculated?**
The `calculate_lighting_load` tool applies a fixed density of 3 VA per square foot to the total livable area provided.

**Q: What appliances are supported?**
The `calculate_appliance_load` tool supports common residential appliances such as electric ranges, clothes dryers, water heaters, dishwashers, and EV chargers.

**Q: How do I determine the required wire gauge?**
Use the `compute_panel_specification` tool. After providing the total VA demand, it will return the recommended American Wire Gauge (AWG) based on the selected panel size.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/electrical-panel-load-calculator](https://vinkius.com/mcp/electrical-panel-load-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Electrical Panel Load Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `electrical-panel-load-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Electrical Panel Load Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "electrical-panel-load-calculator": {
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
