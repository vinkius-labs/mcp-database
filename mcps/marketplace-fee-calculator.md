# Marketplace Fee Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/marketplace-fee-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate net seller proceeds by accounting for commissions, payment fees, shipping, taxes, and promotions.

## Description
This MCP server provides precise financial modeling for marketplace sellers. It allows AI agents to calculate exact net proceeds by subtracting commissions, payment processing fees, shipping costs, taxes, and promotion expenses from the gross sale price. Use `get_seller_proceeds` for a quick net total, `get_fee_breakdown` to see an itemized list of all deductions, or `simulate_margin_impact` to perform what-if analysis on variables like shipping or promotion costs. It also includes `validate_fee_structure` to ensure a pricing model remains profitable.


## Available Tools (4)
- **get_fee_breakdown**: Provides a detailed itemized list of every deduction applied to the gross sale price
- **get_seller_proceeds**: Calculates the final net amount a seller will receive from a single transaction
- **simulate_margin_impact**: Determines how changing a single variable affects the final proceeds
- **validate_fee_structure**: Checks if a specific combination of fees and costs is mathematically viable for a given sale price


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Marketplace Fee Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are my net proceeds for a $100 sale with a 15% commission, $2 fixed payment fee, 3% payment percentage fee, $10 shipping, $8 tax, and $5 promotion cost?"

**🤖 AI Agent:**
> Your net proceeds for this transaction are $62.00.

---

**👤 You:**
> "Show me the detailed breakdown for a $50 sale with 10% commission, $1 fixed fee, 2% payment fee, $5 shipping, $4 tax, and $0 promotion."

**🤖 AI Agent:**
> The deductions are: Commission: $5.00, Payment Fee: $2.00, Shipping: $5.00, Tax: $4.00, Promotion: $0.00. Total deductions: $16.00.

---

**👤 You:**
> "If I increase my shipping cost from $10 to $15 on a $100 sale, how much will my proceeds change?"

**🤖 AI Agent:**
> Increasing the shipping cost by $5.00 will decrease your net proceeds by exactly $5.00.


## ❓ FAQ

**Q: How are the net proceeds calculated?**
Net proceeds are calculated by taking the gross sale price and subtracting the marketplace commission, payment fees (fixed and percentage), shipping costs, taxes, and any promotion costs.

**Q: Can I test how a discount affects my profit?**
Yes, you can use the `simulate_margin_impact` tool to adjust variables like promotion costs and see the resulting change in proceeds.

**Q: Does this tool include shipping costs in the deductions?**
Yes, shipping costs are treated as a deduction from the gross sale price to arrive at the final net proceeds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/marketplace-fee-calculator](https://vinkius.com/en/ai-agent-connect/marketplace-fee-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Marketplace Fee Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `marketplace-fee-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Marketplace Fee Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "marketplace-fee-calculator": {
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
