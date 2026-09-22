# Restaurant Bill Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/restaurant-bill-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate complete restaurant bills including subtotal, taxes, and service fees.

## Description
This MCP server provides tools to manage and calculate restaurant bill totals. It handles individual food and drink line items, applies category-specific tax rates, and calculates service fees. Use `generate_final_bill` to get a complete breakdown of the subtotal, taxes, service fees, and the final amount due.


## Available Tools (4)
- **calculate_service_fee**: Calculates the service fee based on a percentage of the subtotal
- **calculate_taxes**: Calculates the total tax amount based on item categories
- **generate_final_bill**: Computes the complete breakdown of a restaurant bill
- **get_subtotal**: Calculates the sum of all line items before taxes and fees


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Restaurant Bill Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total bill for a meal with a $20 burger (food) and a $5 soda (drink), with 7% food tax, 10% drink tax, and a 15% service fee."

**🤖 AI Agent:**
> The total bill is $28.45.

---

**👤 You:**
> "What is the subtotal for items costing $15.50, $10.00, and $4.50?"

**🤖 AI Agent:**
> The subtotal is $30.00.

---

**👤 You:**
> "Calculate the tax for a $50 food item with a 5% tax rate."

**🤖 AI Agent:**
> The total tax is $2.50.


## ❓ FAQ

**Q: How do I calculate the total bill with all fees?**
You can use the `generate_final_bill` tool to compute the subtotal, taxes, and service fees in one single operation.

**Q: Can I apply different tax rates for food and drinks?**
Yes, the `calculate_taxes` tool allows you to specify separate decimal tax rates for food and drink categories.

**Q: How is the service fee calculated?**
The service fee is calculated by applying a percentage to the subtotal using the `calculate_service_fee` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/restaurant-bill-calculator](https://vinkius.com/en/ai-agent-connect/restaurant-bill-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Restaurant Bill Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `restaurant-bill-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Restaurant Bill Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "restaurant-bill-calculator": {
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
