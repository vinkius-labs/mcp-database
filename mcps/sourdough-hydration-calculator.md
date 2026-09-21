# Sourdough Hydration Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sourdough-hydration-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculate precise baker's percentages, hydration, and batch scaling for sourdough recipes.

## Description
This MCP server provides precise mathematical tools for sourdough bakers. It calculates true hydration by accounting for the flour and water within the starter, determines baker's percentages, and allows for accurate batch scaling. Use `calculate_recipe_metrics` to find the hydration profile of your recipe, `scale_to_target_mass` to adjust a recipe for a specific dough weight, or `scale_to_loaf_count` to prepare exact quantities for a specific number of loaves. It ensures all ingredient weights are rounded to the nearest gram for practical baking.


## Available Tools (4)
- **calculate_recipe_metrics**: You can optionally provide the starter hydration.

Calculates fundamental baker's percentages and total hydration for a sourdough recipe
- **scale_to_loaf_count**: Determines required ingredient quantities for a specific number of loaves
- **scale_to_target_mass**: Re-calculates ingredient quantities to achieve a specific total dough mass
- **validate_hydration_profile**: Checks if a hydration level is within standard sourdough ranges


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sourdough Hydration Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the metrics for a recipe with 500g flour, 350g water, 100g starter, and 10g salt."

**🤖 AI Agent:**
> The total hydration is 72.7% and the total dough yield is 960g.

---

**👤 You:**
> "Scale my recipe to produce exactly 1500g of dough."

**🤖 AI Agent:**
> To achieve 1500g of dough, you will need 781g of flour, 547g of water, 156g of starter, and 16g of salt.

---

**👤 You:**
> "Is a hydration of 82% considered high?"

**🤖 AI Agent:**
> Yes, a hydration of 82% is classified as High.


## ❓ FAQ

**Q: How does this tool calculate hydration?**
The tool calculates total hydration by summing the water from the added water and the water contained within the starter, then dividing by the total flour (added flour plus flour from the starter).

**Q: Can I scale a recipe for a specific number of loaves?**
Yes, you can use the `scale_to_loaf_count` tool to determine the exact ingredient weights needed for a specific number of loaves of a chosen weight.

**Q: Does it handle starter hydration?**
Yes, when using `calculate_recipe_metrics`, you can specify the starter hydration (defaulting to 100%) to ensure the most accurate calculations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sourdough-hydration-calculator](https://vinkius.com/en/ai-agent-connect/sourdough-hydration-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sourdough Hydration Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sourdough-hydration-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sourdough Hydration Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sourdough-hydration-calculator": {
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
