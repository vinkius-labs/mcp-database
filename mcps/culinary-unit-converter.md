# Culinary Unit Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/culinary-unit-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Convert culinary measurements between units like cups, spoons, and ml, or estimate ingredient mass.

## Description
This MCP server provides precise tools for culinary conversions. Use `convert_volume` to switch between volumetric units like cup, tablespoon, teaspoon, ml, oz, liter, and pinch. Use `estimate_mass` to calculate the estimated weight in grams of an ingredient based on its type (liquid, granulated, or solid). Additionally, `get_unit_details` provides metadata for specific units.


## Available Tools (3)
- **get_unit_details**: Provides metadata and usage context for a specific culinary unit
- **convert_volume**: Converts a value from one volumetric unit to another
- **estimate_mass**: Calculates the estimated mass (in grams) of a specific volume


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Culinary Unit Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert 2 cups to tablespoons."

**🤖 AI Agent:**
> Using `convert_volume`, 2 cups is equal to 32 tablespoons.

---

**👤 You:**
> "How many grams is 100ml of liquid ingredient?"

**🤖 AI Agent:**
> By calling `estimate_mass` with volume 100, unit 'ml', and type 'liquid', the estimated mass is 100 grams.

---

**👤 You:**
> "What is the usage of a teaspoon?"

**🤖 AI Agent:**
> The `get_unit_details` tool for 'teaspoon' shows it has a standard volume of 5ml and is typically used for small amounts of spices or liquids.


## ❓ FAQ

**Q: How can I convert cups to milliliters?**
You can use the `convert_volume` tool by providing the value, setting 'fromUnit' to 'cup', and 'toUnit' to 'ml'.

**Q: How does mass estimation work?**
The `estimate_mass` tool uses the ingredient type (liquid, granulated, or solid) to apply a density multiplier to the volume provided.

**Q: What units are supported?**
Supported units include cup, tablespoon, teaspoon, ml, oz, liter, and pinch. You can inspect specific unit metadata using `get_unit_details`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/culinary-unit-converter](https://vinkius.com/mcp/culinary-unit-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Culinary Unit Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `culinary-unit-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Culinary Unit Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "culinary-unit-converter": {
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
