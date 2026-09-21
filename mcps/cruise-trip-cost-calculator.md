# Cruise Trip Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cruise-trip-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate total cruise costs, per-person daily rates, and package value comparisons.

## Description
This MCP server provides a complete financial planning suite for cruise travelers. It allows AI agents to aggregate all trip expenses, including base fares, port fees, taxes, and gratuities. Users can use `calculate_trip_summary` to get a full breakdown of total, per-person, and per-day costs. The toolset also includes `analyze_package_value` to determine if beverage or internet packages are worth the cost, `calculate_excursion_budget` for activity planning, and `get_cabin_comparison` to evaluate different cabin tiers.


## Available Tools (4)
- **analyze_package_value**: Determines if a flat-rate package is more cost-effective than paying for individual items
- **calculate_excursion_budget**: Estimates the total cost of all planned activities and excursions
- **calculate_trip_summary**: Provides a complete breakdown of the total financial commitment for the entire trip
- **get_cabin_comparison**: Compares the cost-effectiveness of different cabin tiers for the same trip


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cruise Trip Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total cost for a 7-day cruise for 2 people with a $1200 base fare, $200 port fees, $150 taxes, and $15 daily gratuities per person."

**🤖 AI Agent:**
> The total trip cost is $1,710. This includes $1,200 for the cabin, $200 in port fees, $150 in taxes, and $210 in total gratuities.

---

**👤 You:**
> "Is a $250 beverage package worth it if a single drink costs $12 and I plan to have 20 drinks?"

**🤖 AI Agent:**
> Yes, the package is worth it. The package costs $250, while 20 individual drinks would cost $240. Wait, actually, the package is not worth it in this specific case as individual drinks are cheaper by $10.

---

**👤 You:**
> "Compare an Economy cabin at $800 and a Suite at $2500 for 2 travelers."

**🤖 AI Agent:**
> The Suite is the most expensive option. The price difference between the Economy and Suite tiers is $1,700, which is $850 per person.


## ❓ FAQ

**Q: How does the tool handle mandatory fees?**
The `calculate_trip_summary` tool automatically aggregates port fees, taxes, and daily gratuities based on the traveler count and trip duration.

**Q: Can I compare different cabin types?**
Yes, you can use `get_cabin_comparison` to compare the cost-effectiveness of different cabin tiers like Economy, Premium, or Suite.

**Q: How do I know if a beverage package is worth it?**
Use the `analyze_package_value` tool by providing the package price and your estimated usage to see if the flat rate is cheaper than paying a la carte.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cruise-trip-cost-calculator](https://vinkius.com/en/ai-agent-connect/cruise-trip-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cruise Trip Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cruise-trip-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cruise Trip Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cruise-trip-cost-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
