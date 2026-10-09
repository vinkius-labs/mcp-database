# Soap Batch Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/soap-batch-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Scales soap recipe ingredients by a batch multiplier for precise production.

## Description
This MCP server provides precise ingredient scaling for soap makers. Use `get_base_recipes` to browse available formulas, `scale_recipe` to calculate new quantities based on a multiplier, and `validate_scaling_safety` to ensure your batch size fits within standard equipment limits. It also includes `get_ingredient_catalog` to verify ingredient availability.


## Available Tools (4)
- **get_base_recipes**: Retrieves the list of available standard soap recipes
- **get_ingredient_catalog**: Provides a list of all ingredients used across all standard recipes
- **scale_recipe**: Calculates the new quantities for all ingredients when a recipe is scaled
- **validate_scaling_safety**: Checks if a scaled recipe remains within safe operational bounds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Soap Batch Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What soap recipes are available?"

**🤖 AI Agent:**
> The available recipes are Lavender Bliss and Citrus Surge.

---

**👤 You:**
> "Scale the Citrus Surge recipe by 1.5."

**🤖 AI Agent:**
> For Citrus Surge at 1.5x scale: Lye: 45g, Coconut Oil: 90g, Citrus Essential Oil: 4.5g.

---

**👤 You:**
> "Is it safe to scale Lavender Bliss by 10?"

**🤖 AI Agent:**
> No, a multiplier of 10 for Lavender Bliss exceeds the safe operational bounds for standard equipment.


## ❓ FAQ

**Q: How do I see which recipes are available?**
You can use the `get_base_recipes` tool to list all available standard soap recipes.

**Q: Can I check if a large batch is safe to make?**
Yes, use the `validate_scaling_safety` tool to check if your multiplier keeps the recipe within safe operational bounds for standard equipment.

**Q: How do I scale a recipe for a double batch?**
Use the `scale_recipe` tool with your desired `recipeId` and set the `multiplier` to 2.0.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/soap-batch-calculator](https://vinkius.com/en/ai-agent-connect/soap-batch-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Soap Batch Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `soap-batch-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Soap Batch Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "soap-batch-calculator": {
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
