# Durian Value-Yield Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/durian-value-yield-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate the true edible yield and cost-efficiency of durian varieties.

## Description
This MCP server provides deterministic tools to calculate the real value of durian purchases. By accounting for non-edible components like husk and seed weight, it reveals the true cost per kilogram of edible flesh. Use `calculate_yield_metrics` to find the exact edible weight and effective price, `get_variety_statistics` to check biological characteristics of specific varieties, or `recommend_best_value` to identify the most cost-effective durian for your budget.


## Available Tools (3)
- **calculate_yield_metrics**: Calculates the physical edible weight and the true cost per kilogram of the edible portion
- **get_variety_statistics**: Answers "What are the typical seed/husk characteristics for a specific variety?"
- **recommend_best_value**: Answers "Which variety should I buy to get the most value for my money?"


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Durian Value-Yield Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I bought 5kg of Musang King for 150 SGD. The quality is an 8/10. What is my yield and value?"

**🤖 AI Agent:**
> For 5kg of Musang King, the edible flesh weight is 3.25kg, the effective price is 46.15 SGD/kg, and your value score is 17.34.

---

**👤 You:**
> "Which durian should I buy if my budget is 30 SGD per kg?"

**🤖 AI Agent:**
> Based on a budget of 30 SGD/kg, the D24 variety offers the best value for your money.

---

**👤 You:**
> "What are the seed and husk percentages for D24 durian?"

**🤖 AI Agent:**
> For the D24 variety, the expected seed weight is 20% and the husk weight is 60%.


## ❓ FAQ

**Q: How is the edible weight calculated?**
The edible weight is calculated by subtracting the fixed husk weight (60%) and the variety-specific seed weight from the total weight.

**Q: What is the difference between sticker price and effective price?**
The sticker price is the cost per kg of the whole fruit, while the effective price is the actual cost per kg of the edible flesh you consume.

**Q: Can I use this to compare different durian varieties?**
Yes, you can use `recommend_best_value` to compare varieties based on your budget and quality preferences.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/durian-value-yield-calculator](https://vinkius.com/ai-agent-connect/durian-value-yield-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Durian Value-Yield Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `durian-value-yield-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Durian Value-Yield Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "durian-value-yield-calculator": {
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
