# Mocktail Recipe Scaler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mocktail-recipe-scaler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Precision scaling for non-alcoholic cocktail recipes, accounting for ice displacement and flavor balance.

## Description
This MCP server provides precision tools for scaling mocktail recipes. It accounts for physical variables like ice displacement and dilution, and chemical variables like sweetness and acidity targets. Use `scale_recipe_by_servings` to expand a recipe for a crowd, `scale_recipe_by_glass_volume` to fit specific glassware, `adjust_flavor_profile` to fine-tune taste, or `calculate_batch_logistics` to plan purchasing and preparation.


## Available Tools (4)
- **adjust_flavor_profile**: Rescales a recipe to meet specific sweetness or acidity targets
- **calculate_batch_logistics**: Provides a summary of total requirements for a large batch
- **scale_recipe_by_glass_volume**: Calculates how to adjust a recipe to perfectly fit a specific glassware type
- **scale_recipe_by_servings**: Scales an existing single-serving recipe to a specific number of servings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mocktail Recipe Scaler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scale this Mojito recipe for 15 people."

**🤖 AI Agent:**
> To serve 15 people, you will need 450ml of lime juice, 300ml of mint syrup, and 450ml of club soda. Total batch volume is 1200ml, and you will need 15 mint sprigs.

---

**👤 You:**
> "How much liquid fits in a 350ml glass if the ice displaces 50ml?"

**🤖 AI Agent:**
> The recipe will be scaled to provide 300ml of liquid per serving to accommodate the 50ml of ice displacement.

---

**👤 You:**
> "Make this recipe 20% sweeter."

**🤖 AI Agent:**
> The recipe has been adjusted with a sweetness factor of 1.2, increasing the syrup quantity to meet your target.


## ❓ FAQ

**Q: How does this tool handle ice?**
The tool uses `scale_recipe_by_glass_volume` to account for the volume of liquid displaced by ice, ensuring the drink fits perfectly in your glassware.

**Q: Can I change the sweetness of a recipe?**
Yes, you can use `adjust_flavor_profile` to apply a sweetness or acidity multiplier to any recipe.

**Q: How do I prepare for a large event?**
Use `calculate_batch_logistics` to get a full breakdown of total liquid volume, ingredient costs, and garnish counts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mocktail-recipe-scaler](https://vinkius.com/en/ai-agent-connect/mocktail-recipe-scaler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mocktail Recipe Scaler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mocktail-recipe-scaler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mocktail Recipe Scaler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mocktail-recipe-scaler": {
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
