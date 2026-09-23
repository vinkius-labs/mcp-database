# Recipe Pan Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/recipe-pan-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Accurately scale ingredient quantities when switching between different pan sizes or shapes.

## Description
This MCP server provides precise tools for culinary professionals and home cooks to scale recipes based on pan surface area. By calculating the ratio between the original pan and a new pan, you can ensure consistent cooking results. Use `calculate_scaling_factor` to find the multiplier, `scale_ingredient_quantity` to adjust amounts, and `convert_to_culinary_units` to get human-readable measurements like '1 cup 2 tbsp'.


## Available Tools (4)
- **calculate_scaling_factor**: Determines the exact multiplier needed to scale a recipe based on the change in pan surface area
- **convert_to_culinary_units**: Transforms raw numerical quantities into human-readable culinary measurements
- **get_recipe_scaling_summary**: Provides a high-level overview of the conversion task
- **scale_ingredient_quantity**: Applies a scaling factor to a specific ingredient amount to find the new required amount


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recipe Pan Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am switching from a circular pan with a 4-inch radius to a rectangular pan that is 10 inches long and 5 inches wide. What is my scaling factor?"

**🤖 AI Agent:**
> The scaling factor is 1.989.

---

**👤 You:**
> "If my scaling factor is 1.5 and I need 2 cups of flour, how much flour do I need now?"

**🤖 AI Agent:**
> You need 3 cups of flour.

---

**👤 You:**
> "Convert 0.75 cups into a more readable format."

**🤖 AI Agent:**
> 3/4 cup


## ❓ FAQ

**Q: How does this tool calculate the scaling factor?**
It calculates the ratio of the new pan's surface area to the original pan's surface area using `calculate_scaling_factor`.

**Q: Can I convert measurements to cups or grams?**
Yes, use `convert_to_culinary_units` to transform raw numbers into readable measurements like grams, cups, or tablespoons.

**Q: What pan shapes are supported?**
The server supports CIRCULAR and RECTANGULAR pan geometries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/recipe-pan-converter](https://vinkius.com/en/ai-agent-connect/recipe-pan-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Recipe Pan Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recipe-pan-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Recipe Pan Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recipe-pan-converter": {
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
