# Functional Beverage Nutrition Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/functional-beverage-nutrition-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [nutrition](../categories/nutrition.md)

Calculate precise nutritional profiles, label rounding, and compliance for beverage formulations.

## Description
This MCP server provides a suite of tools for beverage formulators to manage nutritional data. Use `calculate_nutrition_profile` to aggregate calories, sugar, caffeine, and other nutrients for both single servings and full containers. Ensure regulatory compliance by using `apply_label_rounding` for USA and Europe standards, and `validate_against_limits` to check formulations against specific nutrient thresholds. You can also use `summarize_active_ingredients` to isolate functional components like vitamins or caffeine for claim verification.


## Available Tools (4)
- **calculate_nutrition_profile**: Computes total nutritional content for a single serving and the entire container
- **summarize_active_ingredients**: Extracts and aggregates functional active ingredients from a profile
- **validate_against_limits**: Checks if a nutrition profile exceeds user-defined thresholds
- **apply_label_rounding**: Adjusts raw nutritional values to comply with USA or Europe labeling rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Functional Beverage Nutrition Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the nutrition for a 500ml bottle with a 250ml serving size using these ingredients: [{"name": "water", "volume": 500}, {"name": "sugar", "mass": 20}]"

**🤖 AI Agent:**
> The 250ml serving contains 20 calories and 5g of sugar. The full 500ml container contains 40 calories and 10g of sugar.

---

**👤 You:**
> "Check if this profile is compliant with a sugar limit of 5g per serving: {"sugar": 6}"

**🤖 AI Agent:**
> The profile is non-compliant. The sugar content (6g) exceeds the limit of 5g.

---

**👤 You:**
> "Summarize the active ingredients from this profile: {"active_ingredients": [{"name": "caffeine", "amount": 50}]}"

**🤖 AI Agent:**
> The active ingredients are: caffeine (50mg).


## ❓ FAQ

**Q: How do I calculate the nutrition for a whole bottle?**
You can use the `calculate_nutrition_profile` tool by providing both the `servingSize` and the `containerSize`. The tool will return both serving-level and container-level nutritional data.

**Q: Can I check if my drink meets sugar limits?**
Yes, use the `validate_against_limits` tool. You provide the nutrition profile and a map of your maximum allowed nutrient values to receive a compliance report.

**Q: Does this support European labeling standards?**
Yes, the `apply_label_rounding` tool supports both USA and Europe regulatory rounding rules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/functional-beverage-nutrition-calculator](https://vinkius.com/en/ai-agent-connect/functional-beverage-nutrition-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Functional Beverage Nutrition Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `functional-beverage-nutrition-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Functional Beverage Nutrition Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "functional-beverage-nutrition-calculator": {
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
