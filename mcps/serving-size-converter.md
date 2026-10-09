# Serving Size Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/serving-size-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Precisely scale recipe ingredient quantities to match any desired serving size.

## Description
This MCP server provides precise mathematical tools for adjusting recipe ingredients when changing serving counts. It allows AI agents to calculate individual ingredient amounts using `scale_ingredient_quantity`, scale entire ingredient lists at once with `batch_scale_ingredients`, determine the necessary multiplier via `get_scaling_factor`, and verify if a requested change is practical for kitchen use with `validate_recipe_scale`.


## Available Tools (4)
- **batch_scale_ingredients**: Scales an entire list of ingredients at once for a new serving size
- **get_scaling_factor**: Provides the multiplier needed to convert any ingredient from the original serving size to the target size
- **scale_ingredient_quantity**: Calculates the new amount of a single ingredient needed for a different number of servings
- **validate_recipe_scale**: Checks if a requested scaling operation is within practical culinary limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Serving Size Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a recipe for 4 servings that uses 200g of flour. How much flour do I need for 6 servings?"

**🤖 AI Agent:**
> You will need 300g of flour for 6 servings.

---

**👤 You:**
> "Scale these ingredients from 2 servings to 10 servings: [{'name': 'sugar', 'quantity': 50}, {'name': 'butter', 'quantity': 100}]"

**🤖 AI Agent:**
> [{'name': 'sugar', 'scaledQuantity': 250}, {'name': 'butter', 'scaledQuantity': 500}]

---

**👤 You:**
> "What is the scaling factor if I want to go from 8 servings to 2 servings?"

**🤖 AI Agent:**
> The scaling factor is 0.25.


## ❓ FAQ

**Q: How do I scale a whole list of ingredients?**
You can use the `batch_scale_ingredients` tool by providing a list of ingredient names and their original quantities along with the original and target serving counts.

**Q: Can I check if a recipe scale is too extreme for cooking?**
Yes, the `validate_recipe_scale` tool checks if the requested scaling is within practical culinary limits to ensure measurements remain usable in a standard kitchen.

**Q: What happens if I try to scale for zero servings?**
The tools will return an error, as scaling for zero or negative servings is mathematically undefined and not supported.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/serving-size-converter](https://vinkius.com/en/ai-agent-connect/serving-size-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Serving Size Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `serving-size-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Serving Size Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "serving-size-converter": {
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
