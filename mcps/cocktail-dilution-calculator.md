# Cocktail Dilution Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cocktail-dilution-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [food-and-drink](../categories/food-and-drink.md)

Calculate precise water and ice dilution for cocktail recipes.

## Description
This MCP server provides precision calculation tools for mixologists to manage cocktail dilution. It allows you to determine the exact amount of water or melted ice needed to reach specific dilution targets based on your base ingredients. Use `calculate_dilution_volume` to find the required water volume, `calculate_total_from_target` to work backward from a desired final drink size, `estimate_ice_melt_volume` to convert water volume into ice weight, or `validate_recipe_balance` to verify if your current volumes match your target percentage.


## Available Tools (4)
- **estimate_ice_melt_volume**: Converts a target dilution volume into a weight of ice, assuming standard ice melting properties
- **calculate_dilution_volume**: Determines how much water/ice is needed to hit a specific dilution target
- **calculate_total_from_target**: Determines the required base volume if the user knows their final desired cocktail volume and target dilution
- **validate_recipe_balance**: Checks if a proposed set of volumes (base and dilution) matches a specific target dilution percentage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cocktail Dilution Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 60ml of base ingredients. How much water do I need for a 25% dilution?"

**🤖 AI Agent:**
> You need 15ml of water, resulting in a total volume of 75ml.

---

**👤 You:**
> "I want a final cocktail volume of 120ml with a 20% dilution. What is my base volume?"

**🤖 AI Agent:**
> You need 100ml of base ingredients and 20ml of dilution volume.

---

**👤 You:**
> "How much ice weight do I need to get 30ml of water?"

**🤖 AI Agent:**
> You need approximately 31.2g of ice.


## ❓ FAQ

**Q: How do I calculate the water needed for a Negroni?**
You can use the `calculate_dilution_volume` tool by providing the total volume of your gin, vermouth, and bitters as the base volume, and your target dilution percentage.

**Q: Can I estimate how much ice I need to melt?**
Yes, use the `estimate_ice_melt_volume` tool to convert your required dilution volume into the estimated weight of ice needed.

**Q: How do I check if my cocktail is balanced?**
Use the `validate_recipe_balance` tool to input your base volume, dilution volume, and target percentage to see if they match.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cocktail-dilution-calculator](https://vinkius.com/en/ai-agent-connect/cocktail-dilution-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cocktail Dilution Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cocktail-dilution-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cocktail Dilution Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cocktail-dilution-calculator": {
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
