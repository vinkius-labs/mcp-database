# CO2 Savings Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/co2-savings-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sustainability](../categories/sustainability.md)

Calculate the mass of CO2 emissions avoided by using recycled materials instead of primary production.

## Description
This MCP server provides tools to quantify environmental benefits through carbon avoidance. By comparing the energy-intensive primary production process with more efficient recycled production, users can determine the exact kilograms of CO2 prevented from entering the atmosphere. Use `get_material_registry` to see supported materials, `calculate_single_material_savings` for individual calculations, and `calculate_batch_recycling_impact` to assess entire product lists at once.


## Available Tools (4)
- **calculate_batch_recycling_impact**: Calculate cumulative CO2 savings for a list of materials
- **get_impact_tier**: Categorize the magnitude of carbon savings
- **get_material_registry**: Retrieve the registry of supported materials and their emission factors
- **calculate_single_material_savings**: Calculate CO2 savings for one material at a specific mass


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CO2 Savings Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much CO2 can I save by recycling 500kg of aluminum?"

**🤖 AI Agent:**
> By recycling 500kg of aluminum, you would avoid approximately 8750kg of CO2 emissions.

---

**👤 You:**
> "What materials are available in the registry?"

**🤖 AI Agent:**
> The registry currently supports materials such as aluminum, glass, and steel.

---

**👤 You:**
> "Calculate the impact of recycling 10kg of glass and 20kg of plastic."

**🤖 AI Agent:**
> The total avoided CO2 for this batch is 45.5kg.


## ❓ FAQ

**Q: How do I know which materials are supported?**
You can use the `get_material_registry` tool to retrieve a complete list of all materials currently in the system along with their specific emission factors.

**Q: Can I calculate savings for multiple materials at once?**
Yes, the `calculate_batch_recycling_impact` tool allows you to provide a JSON array of items to calculate cumulative CO2 savings for an entire batch.

**Q: How is the environmental impact tier determined?**
The `get_impact_tier` tool compares your calculated avoided CO2 against pre-defined thresholds to categorize the savings as low, medium, or high impact.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/co2-savings-calculator](https://vinkius.com/mcp/co2-savings-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CO2 Savings Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `co2-savings-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CO2 Savings Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "co2-savings-calculator": {
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
