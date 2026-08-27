# Angel's Share: Wine Evaporation Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/angels-share-wine-evaporation-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate wine evaporation loss and topping requirements during barrel aging.

## Description
This MCP server provides precise calculations for the 'Angel's Share'--the volume of wine lost to evaporation during barrel aging. By modeling diffusion through wood staves, it allows winemakers to predict monthly evaporation rates, cumulative losses over time, and the exact volume of wine needed for topping. Use `calculate_monthly_evaporation_rate` to assess current cellar impact, `calculate_cumulative_loss` for long-term planning, or `compare_barrel_profiles` to see how different wood types like French or American oak behave in your specific cellar environment.


## Available Tools (4)
- **calculate_cumulative_loss**: Predicts the total percentage of wine lost over a specific duration of aging
- **calculate_monthly_evaporation_rate**: Determines the expected percentage of volume lost per month under current cellar conditions
- **calculate_topping_requirement**: Determines the specific volume of wine needed to refill a barrel to its original level
- **compare_barrel_profiles**: Compares how different wood types would perform under the exact same cellar conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Angel's Share: Wine Evaporation Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected monthly evaporation rate for a 5-year-old French oak barrel in a cellar at 14°C and 75% humidity?"

**🤖 AI Agent:**
> The expected monthly evaporation rate for your French oak barrel is 0.12%.

---

**👤 You:**
> "How much wine will I lose in total if I age wine in American oak for 24 months at 15°C and 70% humidity?"

**🤖 AI Agent:**
> The total cumulative loss over 24 months in American oak will be 2.85%.

---

**👤 You:**
> "I have 200 liters of wine in a Hungarian oak barrel. How much wine do I need to top it up after 6 months at 13°C and 80% humidity?"

**🤖 AI Agent:**
> You will need 0.74 liters of wine to refill the barrel to its original level.


## ❓ FAQ

**Q: How does wood type affect evaporation?**
Different woods have different porosities. You can use `compare_barrel_profiles` to see how French, American, and Hungarian oak differ under your specific cellar conditions.

**Q: What is 'topping' in winemaking?**
Topping is the process of adding wine to a barrel to replace the volume lost to evaporation. The `calculate_topping_requirement` tool tells you exactly how much is needed.

**Q: Does cellar temperature impact the loss?**
Yes, higher temperatures increase the vapor pressure deficit, accelerating evaporation. The tools account for temperature and humidity to provide accurate models.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/angels-share-wine-evaporation-calculator](https://vinkius.com/ai-agent-connect/angels-share-wine-evaporation-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Angel's Share: Wine Evaporation Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `angels-share-wine-evaporation-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Angel's Share: Wine Evaporation Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "angels-share-wine-evaporation-calculator": {
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
