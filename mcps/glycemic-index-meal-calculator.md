# Glycemic Index Meal Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/glycemic-index-meal-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate the weighted average Glycemic Index of a meal based on ingredient proportions.

## Description
This MCP server provides tools to assess the glycemic impact of meals. Use `calculate_weighted_gi` to compute the total weighted average GI from a list of ingredients and their weights, `categorize_impact_level` to classify an index as Low, Medium, or High, and `validate_ingredient_integrity` to ensure ingredient data is valid for calculation.


## Available Tools (3)
- **calculate_weighted_gi**: Calculate the weighted average glycemic index of a meal
- **categorize_impact_level**: Classify the glycemic impact level of a given GI value
- **validate_ingredient_integrity**: Validate the integrity of an individual ingredient entry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Glycemic Index Meal Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the weighted glycemic index for a meal with 100g of white bread (GI: 75) and 200g of Greek yogurt (GI: 35)?"

**🤖 AI Agent:**
> The calculated weighted average Glycemic Index for this meal is 48.33.

---

**👤 You:**
> "Is a glycemic index of 60 considered high impact?"

**🤖 AI Agent:**
> A Glycemic Index of 60 is classified as Medium Impact.

---

**👤 You:**
> "Check if an ingredient with a GI of -5 and weight of 10 is valid."

**🤖 AI Agent:**
> The ingredient entry is invalid because the Glycemic Index must be a positive number.


## ❓ FAQ

**Q: How do I calculate the GI of my meal?**
Use the `calculate_weighted_gi` tool by providing a JSON array of ingredients, where each entry includes its `glycemicIndex` and `portionWeight`.

**Q: What does the impact level classification mean?**
The `categorize_impact_level` tool classifies values into Low (below 55), Medium (56-69), or High (70+) based on standard nutritional guidelines.

**Q: Can I validate my ingredient data before calculating?**
Yes, use the `validate_ingredient_integrity` tool to check if an individual ingredient's GI and weight are valid positive numbers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/glycemic-index-meal-calculator](https://vinkius.com/mcp/glycemic-index-meal-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Glycemic Index Meal Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `glycemic-index-meal-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Glycemic Index Meal Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "glycemic-index-meal-calculator": {
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
