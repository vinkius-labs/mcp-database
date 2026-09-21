# Coffee Brewing Ratio Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/coffee-brewing-ratio-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Calculate precise coffee doses, water volumes, and brew ratios for any method.

## Description
This MCP server provides precise calculation tools for coffee enthusiasts. Use `calculate_brewing_parameters` to determine the exact weight of coffee and water needed for your target yield. You can also use `evaluate_grind_adjustment` to correct flavor profiles, `calculate_recipe_cost` to track expenses, and `getMethodDefaults` to find standard ratios for espresso, pour-over, french-press, or cold-brew.


## Available Tools (4)
- **calculate_brewing_parameters**: Determines the exact weight of coffee and water required based on a target yield or a target dose
- **calculate_recipe_cost**: Calculates the monetary cost of a single brew based on bean price and recipe dose
- **evaluate_grind_adjustment**: Provides guidance on whether to adjust the grind size based on the perceived flavor of the brew
- **get_method_defaults**: Retrieves standard ratio ranges and grind characteristics for specific brewing methods


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coffee Brewing Ratio Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to make 300g of pour-over coffee using a 1:15 ratio. How much coffee and water do I need?"

**🤖 AI Agent:**
> You will need 20g of coffee and 300g of water.

---

**👤 You:**
> "My espresso tastes bitter. What should I do?"

**🤖 AI Agent:**
> You should use a coarser grind to reduce extraction.

---

**👤 You:**
> "How much does a cup cost if my beans are $20 per 500g and I use 18g for my dose?"

**🤖 AI Agent:**
> The cost per cup is $0.72.


## ❓ FAQ

**Q: How do I calculate the water needed for my pour-over?**
Use the `calculate_brewing_parameters` tool with the mode set to 'pour-over' and specify your target yield or dose.

**Q: What should I do if my coffee tastes sour?**
Use `evaluate_grind_adjustment` with the flavor 'sour'. It will recommend a finer grind to increase extraction.

**Q: Can I calculate the cost of my coffee?**
Yes, use `calculate_recipe_cost` by providing the price per unit and the dose used in grams.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/coffee-brewing-ratio-calculator](https://vinkius.com/en/ai-agent-connect/coffee-brewing-ratio-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coffee Brewing Ratio Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coffee-brewing-ratio-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coffee Brewing Ratio Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coffee-brewing-ratio-calculator": {
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
