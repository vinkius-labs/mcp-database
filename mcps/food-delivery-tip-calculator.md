# Food Delivery Tip Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/food-delivery-tip-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise delivery tips and view industry standard recommendations.

## Description
This MCP server provides essential tools for managing food delivery gratuities. Use `calculate_tip_amount` to find the exact monetary value for any order total and percentage, or `get_tip_recommendations` to see standard tiers like Good or Excellent. You can also use `validate_tip_compliance` to ensure a tip meets minimum service standards and `format_currency_display` to present amounts in USA or Europe formats.


## Available Tools (4)
- **validate_tip_compliance**: 
- **calculate_tip_amount**: 
- **format_currency_display**: 50 or 12,50 €

Formats a numeric value into a human-readable string suitable for USA or Europe
- **get_tip_recommendations**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Food Delivery Tip Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much is a 20% tip on a $50.00 order?"

**🤖 AI Agent:**
> $10.00

---

**👤 You:**
> "What are the standard tip recommendations for a $30.00 order?"

**🤖 AI Agent:**
> Standard (15%): $4.50, Good (18%): $5.40, Excellent (20%): $6.00

---

**👤 You:**
> "Is a $2.00 tip compliant for a $40.00 order?"

**🤖 AI Agent:**
> No, the tip is not compliant as it falls below the minimum service threshold.


## ❓ FAQ

**Q: How do I calculate a specific tip amount?**
You can use the `calculate_tip_amount` tool by providing the total order cost and the percentage you wish to tip.

**Q: Can I see standard tip suggestions?**
Yes, the `get_tip_recommendations` tool provides standard tiers such as Standard, Good, and Excellent based on your order total.

**Q: How can I check if my tip is fair?**
Use the `validate_tip_compliance` tool to check if your proposed tip meets the minimum service standards for the driver.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/food-delivery-tip-calculator](https://vinkius.com/en/ai-agent-connect/food-delivery-tip-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Food Delivery Tip Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `food-delivery-tip-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Food Delivery Tip Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "food-delivery-tip-calculator": {
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
