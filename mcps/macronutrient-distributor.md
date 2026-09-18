# Macronutrient Distributor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/macronutrient-distributor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculates optimal daily and meal-based macronutrient targets.

## Description
This MCP server provides precise nutritional planning tools. Use `calculate_daily_macros` to determine protein, carbohydrate, and fat targets based on caloric goals and activity levels. You can also use `distribute_macros_per_meal` to split these totals across your eating windows, or `get_therapeutic_adjustments` to modify targets for specific health needs like muscle preservation.


## Available Tools (4)
- **distribute_macros_per_meal**: Breaks down the daily macronutrient totals into specific amounts for each meal
- **calculate_daily_macros**: Calculates the total daily grams of protein, carbohydrates, and fats
- **get_therapeutic_adjustments**: Provides specific macronutrient modifications for therapeutic dietary needs
- **validate_diet_compliance**: Checks if a set of eaten foods or a specific meal meets the target macronutrient ratios


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Macronutrient Distributor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my macros for a 2000 calorie maintenance diet with a balanced approach and moderate activity."

**🤖 AI Agent:**
> Your daily targets are 150g of protein, 225g of carbohydrates, and 67g of fats.

---

**👤 You:**
> "Split my daily macros (150g protein, 225g carbs, 67g fat) into 4 meals."

**🤖 AI Agent:**
> Each of your 4 meals will contain 37.5g of protein, 56.25g of carbohydrates, and 16.75g of fats.

---

**👤 You:**
> "I ate 30g protein, 40g carbs, and 10g fat. My target was 30g protein, 45g carbs, and 15g fat. Am I compliant?"

**🤖 AI Agent:**
> You are within the acceptable variance for protein, but you are slightly under your targets for carbohydrates and fats.


## ❓ FAQ

**Q: How do I calculate my daily targets?**
Use the `calculate_daily_macros` tool by providing your total calorie target, your goal (maintenance, loss, or gain), your diet type, and your activity level.

**Q: Can I adjust macros for specific medical needs?**
Yes, the `get_therapeutic_adjustments` tool allows you to modify your base macros for conditions such as muscle preservation or glucose control.

**Q: How can I check if I am following my diet?**
You can use `validate_diet_compliance` to compare your target macros against what you have actually consumed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/macronutrient-distributor](https://vinkius.com/en/ai-agent-connect/macronutrient-distributor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Macronutrient Distributor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `macronutrient-distributor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Macronutrient Distributor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "macronutrient-distributor": {
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
