# Grocery Discount Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/grocery-discount-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate grocery savings and final totals with precision.

## Description
This MCP server provides tools to manage grocery promotions. Use `get_savings_summary` to see a full breakdown of costs, or `calculate_final_total` to find the exact amount a customer owes. You can also use `validate_discount_eligibility` to check if a purchase meets specific promotional thresholds.


## Available Tools (4)
- **calculate_discount_amount**: Determines the specific monetary value that will be deducted from the subtotal
- **calculate_final_total**: Calculates the final amount the customer must pay
- **get_savings_summary**: Provides a complete breakdown of the original cost, the amount saved, and the final cost
- **validate_discount_eligibility**: Checks if a specific subtotal meets the minimum threshold required for a discount to be applied


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grocery Discount Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I spent $50.00 and have a 10% discount. How much is my final total?"

**🤖 AI Agent:**
> Your final total is $45.00.

---

**👤 You:**
> "Give me a summary for a $100.00 subtotal with a 15% discount."

**🤖 AI Agent:**
> Original Subtotal: $100.00, Amount Saved: $15.00, Final Total: $85.00.

---

**👤 You:**
> "Is a $35.00 purchase eligible for a $40.00 minimum discount threshold?"

**🤖 AI Agent:**
> No, the subtotal does not meet the minimum threshold.


## ❓ FAQ

**Q: How do I check if my order qualifies for a discount?**
You can use the `validate_discount_eligibility` tool by providing your subtotal and the required minimum threshold.

**Q: Can I get a full breakdown of my savings?**
Yes, the `get_savings_summary` tool provides the original subtotal, the amount saved, and the final total.

**Q: Does this tool handle rounding?**
Yes, all financial calculations are rounded to two decimal places for accuracy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/grocery-discount-calculator](https://vinkius.com/en/ai-agent-connect/grocery-discount-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grocery Discount Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `grocery-discount-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grocery Discount Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grocery-discount-calculator": {
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
