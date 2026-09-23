# Spice Mix Scaler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/spice-mix-scaler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Scales spice blend recipes for commercial batch production using precise multipliers.

## Description
A professional culinary utility for commercial spice blending. This MCP server allows AI agents to perform precise mass-based scaling of spice recipes. Use `list_available_recipes` to browse the catalog, `scale_recipe_batch` to calculate new ingredient quantities based on a multiplier, `get_recipe_ratios` to analyze the composition of a mix, and `validate_scaling_integrity` to ensure new batches maintain exact flavor profiles.


## Available Tools (4)
- **get_recipe_ratios**: Gets the proportional relationship between spices in a mix
- **list_available_recipes**: Lists all available spice mixes in the catalog
- **scale_recipe_batch**: Scales a spice recipe by a given multiplier
- **validate_scaling_integrity**: Validates if a set of scaled ingredients is mathematically consistent with the original recipe


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spice Mix Scaler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much of each ingredient do I need for a double batch of recipe 'savory-blend-01'?"

**🤖 AI Agent:**
> For a double batch of savory-blend-01, you will need: 20g of Salt, 10g of Black Pepper, and 5g of Garlic Powder.

---

**👤 You:**
> "What are the ingredient ratios for the 'spicy-kick-x' mix?"

**🤖 AI Agent:**
> The 'spicy-kick-x' mix consists of 50% Chili Powder, 30% Cumin, and 20% Paprika.

---

**👤 You:**
> "List all available recipes in the 'Savory' category."

**🤖 AI Agent:**
> The available recipes in the Savory category are: savory-blend-01, herb-mix-alpha, and umami-base-v2.


## ❓ FAQ

**Q: How do I see which spice mixes are available?**
You can use the `list_available_recipes` tool to view all available spice blends in the catalog, with optional filtering by category.

**Q: Can I scale a recipe down as well as up?**
Yes, by using a multiplier less than 1.0 in the `scale_recipe_batch` tool, you can scale a recipe down for smaller batches.

**Q: How does the tool ensure flavor consistency?**
The server uses mass-based calculations and the `validate_scaling_integrity` tool to verify that the ingredient ratios remain identical to the original recipe.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/spice-mix-scaler](https://vinkius.com/en/ai-agent-connect/spice-mix-scaler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spice Mix Scaler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spice-mix-scaler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spice Mix Scaler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spice-mix-scaler": {
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
