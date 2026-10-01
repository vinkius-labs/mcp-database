# Handmade Item Price Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/handmade-item-price-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate sustainable selling prices for handmade goods by accounting for materials, labor, overhead, and fees.

## Description
This MCP server provides a suite of tools for artisans to ensure their handmade businesses remain profitable. It bridges the gap between raw production costs and final customer pricing. Use `calculate_unit_cost` to determine the base production cost including labor and overhead. Use `calculate_selling_price` to find the ideal price that covers platform fees while maintaining your target profit margin. You can also use `calculate_price_with_tax` to find the final out-the-door price for customers, or `compare_pricing_scenarios` to see how changing your margins or platform fees will impact your bottom line.


## Available Tools (4)
- **calculate_price_with_tax**: Calculate the final price including sales tax
- **calculate_unit_cost**: Calculate the base production cost and total unit cost
- **calculate_selling_price**: Calculate the final selling price to achieve a target margin
- **compare_pricing_scenarios**: Compare two different pricing scenarios


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Handmade Item Price Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I spent $15 on materials and 3 hours of work at $20/hour. My overhead is 10% and packaging is $2. What is my total unit cost?"

**🤖 AI Agent:**
> Your total unit cost is $78.50.

---

**👤 You:**
> "My total unit cost is $50. I want a 25% profit margin and the platform fee is 10%. What should my selling price be?"

**🤖 AI Agent:**
> Your suggested selling price is $76.92.

---

**👤 You:**
> "If my suggested price is $100 and the tax rate is 8%, what is the final price for the customer?"

**🤖 AI Agent:**
> The final customer price is $108.00.


## ❓ FAQ

**Q: How does this tool help me stay profitable?**
It ensures you account for all hidden costs like overhead and platform fees, so your target margin is actually what you keep in your pocket.

**Q: Can I compare different pricing strategies?**
Yes, you can use `compare_pricing_scenarios` to see how adjusting your target margin or platform fees changes your final price and profit.

**Q: Does this include sales tax in the price?**
The `calculate_price_with_tax` tool allows you to add a specific tax rate to your suggested selling price to find the total amount a customer pays.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/handmade-item-price-calculator](https://vinkius.com/en/ai-agent-connect/handmade-item-price-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Handmade Item Price Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `handmade-item-price-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Handmade Item Price Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "handmade-item-price-calculator": {
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
