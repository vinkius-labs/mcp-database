# Baking Recipe Scaler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/baking-recipe-scaler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Scale baking recipes using baker's percentages and pan volume geometry.

## Description
This MCP server provides precision tools for professional and home bakers to recalibrate recipes. Use `calculate_scaled_recipe` to determine exact ingredient masses for new pan sizes and hydration levels, or `adjust_yeast_quantity` to maintain fermentation timing. It also includes `get_ingredient_density` to handle mass-to-volume conversions accurately.


## Available Tools (3)
- **adjust_yeast_quantity**: Modifies the yeast amount based on the change in dough volume and hydration
- **calculate_scaled_recipe**: Calculates the exact mass of every ingredient required for a new pan size while adjusting for a specific hydration level
- **get_ingredient_density**: Retrieves the standard density constant for a specific ingredient


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Baking Recipe Scaler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scale my recipe for a larger pan. Original: 500g flour, 350g water, 10g salt. Original pan is round, 15cm diameter, 5cm height. Target pan is round, 20cm diameter, 6cm height. Target hydration is 72%."

**🤖 AI Agent:**
> To scale your recipe for the 20cm pan at 72% hydration, you will need 768.5g of flour, 553.3g of water, and 15.4g of salt.

---

**👤 You:**
> "What is the density of all-purpose flour?"

**🤖 AI Agent:**
> The density of all-purpose flour is 0.59 g/ml.

---

**👤 You:**
> "I'm increasing my dough volume by 1.5x and increasing hydration by 5%. How much yeast should I use if I originally used 7g?"

**🤖 AI Agent:**
> Your adjusted yeast quantity is 10.2g.


## ❓ FAQ

**Q: How does the scaling work?**
The server uses pan volume geometry and baker's percentages to calculate the exact mass of ingredients needed for a target container.

**Q: Can I adjust the hydration level?**
Yes, the `calculate_scaled_recipe` tool allows you to specify a target hydration percentage for the new recipe.

**Q: How is yeast adjusted?**
The `adjust_yeast_quantity` tool scales yeast based on volume changes and hydration differences to ensure consistent fermentation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/baking-recipe-scaler](https://vinkius.com/mcp/baking-recipe-scaler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Baking Recipe Scaler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `baking-recipe-scaler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Baking Recipe Scaler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "baking-recipe-scaler": {
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
