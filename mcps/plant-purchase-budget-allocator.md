# Plant Purchase Budget Allocator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/plant-purchase-budget-allocator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [shopping](../categories/shopping.md)

Optimizes plant selection by maximizing priority scores within a strict budget.

## Description
This MCP server provides an optimization engine to help users select the best collection of plants for their budget. It handles complex constraints including mandatory 'must-have' plants, seasonal discounts, and sales tax. Use `get_plant_catalog` to see available species, `get_seasonal_promotions` to find active discounts, and `calculate_budget_allocation` to generate the optimal purchase list based on your priority scores. You can also use `validate_purchase_plan` to verify if a specific selection is financially viable.


## Available Tools (4)
- **get_plant_catalog**: Retrieves the full list of available plants and their base pricing
- **calculate_budget_allocation**: Performs the core optimization to select plants based on priority and budget
- **validate_purchase_plan**: Verifies if a proposed selection of plants is financially viable and respects all constraints
- **get_seasonal_promotions**: Identifies which plants or categories are currently eligible for discounts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plant Purchase Budget Allocator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a budget of $100 and a tax rate of 0.05. Here are my priorities: {'fern_01': 10, 'cactus_02': 5}. What should I buy?"

**🤖 AI Agent:**
> Based on your $100 budget and priorities, you should purchase the Fern (fern_01) and the Cactus (cactus_02). The total cost including 5% tax is $94.50.

---

**👤 You:**
> "What plants are available in the catalog?"

**🤖 AI Agent:**
> The current catalog includes Ferns, Cacti, Succulents, and Tropical plants with varying base prices.

---

**👤 You:**
> "Is my plan to buy 'fern_01' and 'cactus_02' valid for a $50 budget with 7% tax?"

**🤖 AI Agent:**
> Yes, the plan is valid. The total cost including 7% tax is $42.80, which is within your $50 budget.


## ❓ FAQ

**Q: How does the budget allocation work?**
The system first ensures all 'must-have' plants are included. Then, it uses the remaining budget to select plants with the highest user-assigned priority scores.

**Q: Does the budget include sales tax?**
Yes, the `calculate_budget_allocation` tool incorporates the provided tax rate into the final cost of each plant to ensure the total stays within your limit.

**Q: Can I use seasonal discounts?**
Yes. You can use `get_seasonal_promotions` to identify active discounts and then pass those multipliers to the allocation tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/plant-purchase-budget-allocator](https://vinkius.com/en/ai-agent-connect/plant-purchase-budget-allocator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plant Purchase Budget Allocator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `plant-purchase-budget-allocator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plant Purchase Budget Allocator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plant-purchase-budget-allocator": {
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
