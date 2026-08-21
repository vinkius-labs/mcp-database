# Cocktail Dilution Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/cocktail-dilution-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate final volume, ABV, and water dilution for cocktails.

## Description
This MCP server provides deterministic calculations for cocktail chemistry. It determines the final volume, alcohol-by-volume (ABV), and total water added based on ingredients, preparation methods, and dilution physics. Use `calculate_cocktail_stats` to get precise results for stirred, shaken, or blended drinks, or `validate_recipe_integrity` to ensure your recipe follows standard cocktail logic. It also provides specific dilution guidelines via `get_dilution_guidelines`.


## Available Tools (3)
- **calculate_cocktail_stats**: Calculates the final volume, final ABV, and water added for a specific cocktail recipe
- **get_dilution_guidelines**: Provides the expected dilution percentages and temperature targets based on the chosen method
- **validate_recipe_integrity**: Ensures a recipe is physically possible and follows standard cocktail logic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cocktail Dilution Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the stats for a Negroni: 30ml Gin (40% ABV), 30ml Sweet Vermouth (18% ABV), and 30ml Campari (25% ABV), stirred."

**🤖 AI Agent:**
> The Negroni will have a final volume of 117.0ml, a final ABV of 23.5%, and 27.0ml of water added.

---

**👤 You:**
> "What are the dilution guidelines for a shaken cocktail?"

**🤖 AI Agent:**
> A shaken cocktail typically results in a 40% dilution and a cold target serving temperature.

---

**👤 You:**
> "Is a recipe with 1000ml of Gin valid?"

**🤖 AI Agent:**
> No, the recipe is invalid because the total volume exceeds the standard serving size limit.


## ❓ FAQ

**Q: How does the dilution calculation work?**
The tool applies empirical dilution rates: 30% for stirred, 40% for shaken, and 50% for blended drinks. For layered drinks, no dilution is applied.

**Q: Can I check if my recipe is valid?**
Yes, you can use the `validate_recipe_integrity` tool to check for negative volumes, invalid ABV values, or excessive total volumes.

**Q: What information do I need to provide?**
You need to provide a list of ingredients (name, volume, and ABV), the preparation method (stirred, shaken, blended, or layered), and whether the drink is layered.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/cocktail-dilution-calculator](https://vinkius.com/ai-agent-connect/cocktail-dilution-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cocktail Dilution Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cocktail-dilution-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cocktail Dilution Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cocktail-dilution-calculator": {
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
