# Petrochemical Utilities Balance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/petrochemical-utilities-balance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

Calculate steam, power, and utility equilibrium for petrochemical complexes.

## Description
This MCP server provides tools to manage utility equilibrium in petrochemical complexes. It allows for calculating steam balances, determining power import or export status, and retrieving specific unit demands. By using `evaluate_heat_integration_potential`, users can also estimate savings through pinch analysis and heat recovery optimization.


## Available Tools (4)
- **calculate_power_status**: Determines whether the complex needs to buy electricity or can sell it
- **calculate_steam_balance**: Determines if the complex has a surplus or deficit of steam
- **evaluate_heat_integration_potential**: Estimates the reduction in utility demand achievable through pinch analysis
- **get_unit_demands**: Retrieve the specific utility requirements for a given process unit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Petrochemical Utilities Balance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the utility requirements for unit U-101?"

**🤖 AI Agent:**
> Unit U-101 requires 500 kg/h of steam, 150 kW of power, 200 m3/h of cooling water, and 50 m3/h of instrument air.

---

**👤 You:**
> "Is there a steam surplus if we generate 5000 kg/h of steam for units A, B, and C?"

**🤖 AI Agent:**
> The total steam demand for units A, B, and C is 4200 kg/h, resulting in a net steam surplus of 800 kg/h.

---

**👤 You:**
> "What is the power status if cogeneration produces 1000 kW and demand is 1200 kW with a 500 kW import limit?"

**🤖 AI Agent:**
> The complex is currently importing 200 kW of power from the grid.


## ❓ FAQ

**Q: How do I check the steam surplus or deficit?**
You can use the `calculate_steam_balance` tool by providing the list of unit IDs and the total steam generation.

**Q: Can I estimate energy savings from heat recovery?**
Yes, the `evaluate_heat_integration_potential` tool estimates potential steam and cooling water savings using pinch analysis.

**Q: How is power status determined?**
The `calculate_power_status` tool compares cogeneration output against unit demand to determine if the complex is importing, exporting, or balanced.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/petrochemical-utilities-balance](https://vinkius.com/en/ai-agent-connect/petrochemical-utilities-balance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Petrochemical Utilities Balance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `petrochemical-utilities-balance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Petrochemical Utilities Balance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "petrochemical-utilities-balance": {
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
