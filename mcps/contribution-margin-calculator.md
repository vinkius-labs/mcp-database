# Contribution Margin Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/contribution-margin-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate unit profitability, margin indices, and weighted product mix margins.

## Description
This MCP server provides specialized financial tools to measure business profitability. Use `calculate_unit_margin_metrics` to find the currency value and percentage-based margin for a single product after taxes and variable costs. Use `calculate_portfolio_weighted_margin` to determine the aggregate margin index for a collection of products based on their revenue weight. Additionally, use `identify_underperforming_products` to flag specific items that fall below your required profitability threshold.


## Available Tools (3)
- **calculate_portfolio_weighted_margin**: Determines the aggregate margin index for a collection of products based on their impact on total revenue
- **identify_underperforming_products**: Flags specific products that fail to meet a defined profitability threshold
- **calculate_unit_margin_metrics**: Calculates both the currency value and the percentage-based margin for a single product


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Contribution Margin Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the unit margin for a product with a selling price of $100, variable costs of $60, and a 10% tax rate."

**🤖 AI Agent:**
> The contribution margin amount is $30.00 and the contribution margin index is 0.3 (or 30%).

---

**👤 You:**
> "What is the weighted portfolio margin if Product A has a 20% margin with a 0.7 weight and Product B has a 40% margin with a 0.3 weight?"

**🤖 AI Agent:**
> The weighted average margin for the portfolio is 26%.

---

**👤 You:**
> "Identify products underperforming against a 15% threshold from this list: Product X (10%), Product Y (20%), and Product Z (5%)."

**🤖 AI Agent:**
> The underperforming products are: Product X, Product Z.


## ❓ FAQ

**Q: How do I calculate the margin for a single product?**
Use the `calculate_unit_margin_metrics` tool by providing the selling price, variable cost per unit, and the tax rate percentage.

**Q: How does the portfolio margin calculation work?**
The `calculate_portfolio_weighted_margin` tool calculates a weighted average. You provide an array of products, each with its margin index and revenue weight (the sum of weights must equal 1).

**Q: Yes, use the `identify_underperforming_products` tool. Simply provide a list of your products and their margin indices along with a minimum threshold value.**
Yes, use the `identify_underperforming_products` tool. Simply provide a list of your products and their margin indices along with a minimum threshold value.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/contribution-margin-calculator](https://vinkius.com/mcp/contribution-margin-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Contribution Margin Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `contribution-margin-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Contribution Margin Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "contribution-margin-calculator": {
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
