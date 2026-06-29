# Markup Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/markup-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate markup divisor and suggested selling price based on costs, taxes, and profit margins.

## Description
The Markup Calculator is a specialized financial tool designed to help businesses determine the ideal selling price for their products. By using tools like `calculate_markup`, you can input your base product cost, tax rates, fixed expense rates, and desired profit margins to find the precise markup divisor needed to maintain profitability. Additionally, use `compare_regimes` to evaluate how different tax structures impact your final price, or `list_tax_degrees` to quickly access common industry-standard scenarios. This MCP server acts as a bridge between complex financial logic and your AI assistant, providing accurate, data-driven pricing decisions.


## Available Tools (3)
- **list_tax_scenarios**: g., VAT, US Sales Tax).

List predefined tax scenarios
- **compare_regimes**: Pass scenarios as a JSON string array of objects.

Compare different tax and expense configurations
- **calculate_markup**: Calculate suggested selling price based on costs and rates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Markup Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the suggested selling price for a product that costs $50, with a 20% tax rate, 15% expense rate, and a 10% target profit margin."

**🤖 AI Agent:**
> For a product cost of $50.00, the suggested selling price is $76.92. This calculation uses a markup divisor of 0.65, accounting for a total percentage burden of 45%.

---

**👤 You:**
> "Compare how a 10% tax rate vs a 25% tax rate affects the selling price of an item costing $100 with a 15% profit margin and 10% expenses."

**🤖 AI Agent:**
> With a 10% tax rate, the suggested price is $133.33. With a 25% tax rate, the suggested price increases to $166.67. Both scenarios maintain your 15% profit margin and 10% expense rate.

---

**👤 You:**
> "Show me some common tax and expense scenarios I can use."

**🤖 AI Agent:**
> Here are the available predefined scenarios: VAT_STANDARD (20% tax), VAT_REDUCED (5% tax), and US_SALES_TAX_ESTIMATE (8% tax).


## ❓ FAQ

**Q: How does the markup calculation work?**
The `calculate_markup` tool calculates a divisor by subtracting your tax rate, expense rate, and target profit margin from 100%. It then divides your product cost by this divisor to suggest a selling price that covers all obligations.

**Q: Can I compare different tax scenarios?**
Yes, the `compare_regimes` tool allows you to provide multiple tax and expense configurations in a single request to see how each one affects your suggested selling price.

**Q: What happens if my total rates exceed 100%?**
If the sum of your tax rate, expense rate, and profit margin is 100% or greater, the tool will return an error because a valid selling price cannot be mathematically determined.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/markup-calculator](https://vinkius.com/mcp/markup-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Markup Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `markup-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Markup Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "markup-calculator": {
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
