# Resting Metabolic Rate Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/resting-metabolic-rate-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate your RMR, TDEE, and macronutrient needs using the Mifflin-St Jeor equation.

## Description
This MCP server provides a complete metabolic engine. Use `calculate_rmr` to find your base metabolic rate using the Mifflin-St Jeor equation. Once you have your RMR, use `calculate_tdee` to estimate your total daily energy expenditure based on your activity level. Finally, use `recommend_macronutrients` to get a specific breakdown of proteins, fats, and carbohydrates tailored to your nutritional goals like weight loss or muscle gain.


## Available Tools (4)
- **get_activity_multipliers**: Retrieves the standardized multipliers used for TDEE calculations
- **calculate_rmr**: Calculates the base Resting Metabolic Rate (RMR) using the Mifflin-St Jeor equation
- **calculate_tdee**: Estimates the Total Daily Energy Expenditure (TDEE) by applying an activity multiplier to the RMR
- **recommend_macronutrients**: Provides a caloric distribution strategy for proteins, fats, and carbohydrates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Resting Metabolic Rate Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the RMR for a 30-year-old male weighing 80kg and 180cm tall?"

**🤖 AI Agent:**
> Your Resting Metabolic Rate (RMR) is 1812.0 calories per day.

---

**👤 You:**
> "Calculate TDEE for an RMR of 1500 with a sedentary activity level."

**🤖 AI Agent:**
> Your Total Daily Energy Expenditure (TDEE) is 1800.0 calories per day.

---

**👤 You:**
> "Give me macronutrient recommendations for 2000 calories with a weight loss goal."

**🤖 AI Agent:**
> For a weight loss goal at 2000 calories, you should consume 200.0g of protein, 55.6g of fat, and 175.0g of carbohydrates.


## ❓ FAQ

**Q: What is RMR?**
Resting Metabolic Rate (RMR) is the number of calories your body burns while at rest to maintain vital functions.

**Q: How do I calculate my total daily calories?**
You can use the `calculate_tdee` tool. It takes your RMR and applies an activity multiplier to estimate your total daily energy expenditure.

**Q: Can I get macronutrient recommendations?**
Yes, the `recommend_macronutrients` tool provides a breakdown of protein, fat, and carbohydrate grams based on your target calories and goal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/resting-metabolic-rate-calculator](https://vinkius.com/en/ai-agent-connect/resting-metabolic-rate-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Resting Metabolic Rate Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `resting-metabolic-rate-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Resting Metabolic Rate Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "resting-metabolic-rate-calculator": {
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
