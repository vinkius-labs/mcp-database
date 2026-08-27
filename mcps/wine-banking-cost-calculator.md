# Wine Banking Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-banking-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate barrel aging costs, evaporation losses, and break-even premiums for wine banking.

## Description
This MCP server provides specialized tools for wine banking professionals to model the economic impact of barrel aging. It calculates the annual cost per liter using `get_annual_liquid_cost`, tracks inventory depletion via `get_cumulative_evaporation_loss`, determines necessary price increases with `get_break_even_premium`, and evaluates the efficiency of new versus neutral barrels with `compare_barrel_economics`.


## Available Tools (4)
- **compare_barrel_economics**: Compares the efficiency of using a brand new barrel versus a neutral (reused) barrel
- **get_annual_liquid_cost**: Calculates the total cost of maintaining a single barrel for one year, accounting for the wine volume
- **get_break_even_premium**: Determines the minimum price increase required per liter to make the aging process profitable
- **get_cumulative_evaporation_loss**: Calculates the total volume of wine lost to the "angel's share" over the entire lifespan of the barrel


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Banking Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the annual cost per liter for a 225L barrel costing $500, with a 5-year lifespan, 90% fill, $50 annual storage, $20 annual labor, and 3% angel's share."

**🤖 AI Agent:**
> The annual barrel cost per liter is $12.45, with a total annual maintenance cost of $70.00.

---

**👤 You:**
> "How much wine will be lost from a 200L initial fill over 10 years with a 2% annual evaporation rate?"

**🤖 AI Agent:**
> The total volume lost is 36.42 liters, leaving a remaining volume of 163.58 liters.

---

**👤 You:**
> "What is the required premium per liter if I have $1000 in total costs, lost 20L of wine, started with 100L, and have 80L remaining?"

**🤖 AI Agent:**
> The required premium per liter to break even is $12.50.


## ❓ FAQ

**Q: How does the angel's share affect my costs?**
The angel's share represents the volume lost to evaporation. You can use `get_cumulative_evaporation_loss` to see how much liquid is lost over time, which directly increases the required premium to break even.

**Q: Can I compare new and reused barrels?**
Yes, the `compare_barrel_economics` tool allows you to compare the cost per liter of a brand new barrel against a neutral (reused) barrel to find efficiency gains.

**Q: What is the break-even premium?**
It is the minimum price increase per liter needed to cover all capital expenditures and evaporation losses. Use `get_break_even_premium` to calculate this value.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-banking-cost-calculator](https://vinkius.com/ai-agent-connect/wine-banking-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Banking Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-banking-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Banking Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-banking-cost-calculator": {
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
