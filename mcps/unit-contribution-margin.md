# Unit Contribution Margin MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/unit-contribution-margin)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate unit profitability, break-even points, and profit scenarios.

## Description
This MCP server provides essential financial tools to analyze product profitability. Use `get_unit_contribution_margin` to find the margin per unit, `calculate_break_even_volume` to determine the sales needed to cover fixed costs, `simulate_profitability_scenario` to predict net profit at specific volumes, and `compare_product_margins` to rank products by profitability.


## Available Tools (4)
- **calculate_break_even_volume**: Determines how many units must be sold to cover all costs
- **compare_product_margins**: Evaluates and compares the profitability of multiple product types
- **get_unit_contribution_margin**: Calculates the basic profitability of a single unit
- **simulate_profitability_scenario**: Predicts total profit or loss based on a specific sales volume


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unit Contribution Margin** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the margin for a product that costs $50 to make and sells for $80?"

**🤖 AI Agent:**
> The unit contribution margin is $30.00, which represents a 37.5% margin percentage.

---

**👤 You:**
> "How many units do I need to sell to break even if my fixed costs are $10,000, unit price is $50, and unit cost is $30?"

**🤖 AI Agent:**
> You need to sell 500 units to reach the break-even point, resulting in $25,000 in total revenue.

---

**👤 You:**
> "Predict the profit for selling 1,000 units at $100 each, with a $40 cost and $10,000 fixed costs."

**🤖 AI Agent:**
> The total contribution margin is $60,000, and after subtracting the $10,000 fixed costs, the net profit is $50,000.


## ❓ FAQ

**Q: What is the unit contribution margin?**
It is the amount remaining from the unit price after subtracting the unit cost. You can calculate this using the `get_unit_contribution_margin` tool.

**Q: How do I find my break-even point?**
Use the `calculate_break_even_volume` tool by providing the unit price, unit cost, and total fixed costs.

**Q: Can I compare multiple products at once?**
Yes, the `compare_product_margins` tool allows you to input a list of products to rank them by their margin percentage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/unit-contribution-margin](https://vinkius.com/en/ai-agent-connect/unit-contribution-margin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Unit Contribution Margin** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `unit-contribution-margin` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Unit Contribution Margin** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "unit-contribution-margin": {
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
