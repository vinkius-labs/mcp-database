# Beverage Batch Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/beverage-batch-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Scale drink recipes by guests, glass size, ice displacement, and garnish.

## Description
A professional tool for event planners to calculate precise ingredient lists, total batch volumes, and per-serving costs. Use `calculate_batch_requirements` to determine liquid volumes accounting for ice displacement and garnish, `estimate_inventory_needs` to find out how many bottles to buy, and `validate_recipe_safety` to check for dietary restrictions.


## Available Tools (4)
- **calculate_batch_requirements**: Calculates the total liquid volume, specific ingredient quantities, and total cost for a planned event
- **estimate_inventory_needs**: Determines how many full units of an ingredient must be purchased to cover the batch
- **get_recipe_by_name**: Retrieves the base recipe and unit costs for a specific beverage
- **validate_recipe_safety**: Checks if a recipe contains ingredients that might conflict with dietary or regional restrictions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beverage Batch Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to make 50 Margaritas. The glasses are 300ml, ice takes up 50ml, and lime garnish takes up 10ml. How much liquid do I need?"

**🤖 AI Agent:**
> To serve 50 guests, you will need a total batch volume of 12,000ml of liquid.

---

**👤 You:**
> "Is the Mojito recipe safe for someone who is vegan?"

**🤖 AI Agent:**
> Yes, the Mojito is safe for vegan dietary restrictions.

---

**👤 You:**
> "How many 750ml bottles of Gin do I need for 100 servings of a Gin Fizz?"

**🤖 AI Agent:**
> You will need to purchase 4 bottles of Gin.


## ❓ FAQ

**Q: How does the tool account for ice?**
The tool uses the `iceDisplacement` parameter to subtract the volume occupied by ice from the total glass capacity, ensuring you don't overfill.

**Q: Can I check if a drink is vegan?**
Yes, you can use `validate_recipe_safety` with the 'vegan' restriction to check for conflicting ingredients.

**Q: How many bottles of gin should I buy?**
You can use `estimate_inventory_needs` to get the exact number of purchase units required for your batch.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/beverage-batch-planner](https://vinkius.com/en/ai-agent-connect/beverage-batch-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Beverage Batch Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `beverage-batch-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Beverage Batch Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "beverage-batch-planner": {
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
