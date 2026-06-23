# Ingredient Weight Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ingredient-weight-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Convert volumetric culinary measurements into mass in grams based on specific ingredient densities.

## Description
This MCP server provides precise conversions between volume and weight for over 200 ingredients. By using tools like `search_ingredients`, `get_ingredient_density`, and `convert_volume_to_weight`, AI agents can accurately calculate the mass of ingredients like flour, sugar, or honey when given a volume measurement (e.g., cups, tablespoons, teaspoons). This is essential for digital recipe scaling and automated culinary tasks.


## Available Tools (3)
- **convert_volume_to_weight**: Convert a volume measurement to weight in grams
- **get_ingredient_density**: Retrieve the weight of one cup for a specific ingredient
- **search_ingredients**: Search for ingredients in the pantry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ingredient Weight Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many grams is 2 tablespoons of honey?"

**🤖 AI Agent:**
> Using `convert_volume_to_weight`, 2 tablespoons of honey weighs approximately 42.00g.

---

**👤 You:**
> "Search for ingredients related to 'flour'."

**🤖 AI Agent:**
> The `search_ingredients` tool found: All-purpose flour, Whole wheat flour, and Bread flour.

---

**👤 You:**
> "What is the density of sugar?"

**🤖 AI Agent:**
> The `get_ingredient_density` tool shows that 1 cup of sugar weighs 200.0g.


## ❓ FAQ

**Q: How can I find the correct ingredient name?**
Use the `search_ingredients` tool with a partial name to browse the available catalog.

**Q: Does it support units other than cups?**
Yes. The `convert_volume_to_weight` tool supports common culinary units like tablespoons and teaspoons.

**Q: What happens if I provide an unknown ingredient?**
The tool will return an error message indicating that the ingredient was not found in the catalog.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ingredient-weight-converter](https://vinkius.com/mcp/ingredient-weight-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ingredient Weight Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ingredient-weight-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ingredient Weight Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ingredient-weight-converter": {
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
