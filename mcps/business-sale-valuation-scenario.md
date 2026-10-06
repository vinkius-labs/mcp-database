# Business Sale Valuation Scenario MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/business-sale-valuation-scenario)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate business exit scenarios, from Enterprise Value to final Net Proceeds.

## Description
This MCP server provides a complete financial modeling suite for business owners planning an exit. It allows AI agents to calculate the total market value using `calculate_enterprise_value`, adjust for liabilities with `calculate_equity_value`, and determine final take-home cash using `calculate_net_proceeds`. For a complete financial waterfall, use `generate_valuation_summary` to see the full transition from revenue and profit to net proceeds after taxes and fees.


## Available Tools (4)
- **calculate_enterprise_value**: Calculate the total estimated market value of the business based on its earnings
- **calculate_equity_value**: Calculate the value attributable to shareholders after accounting for debt and cash
- **calculate_net_proceeds**: Calculate how much cash the seller will actually keep after taxes and fees
- **generate_valuation_summary**: Provide a full breakdown of the sale from Enterprise Value down to Net Proceeds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Business Sale Valuation Scenario** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the enterprise value of a company with $5,000,000 in revenue and a 3x multiplier?"

**🤖 AI Agent:**
> The enterprise value of the company is $15,000,000.

---

**👤 You:**
> "If my equity value is $1,000,000, my cost basis was $600,000, the tax rate is 20%, and fees are $50,000, how much will I keep?"

**🤖 AI Agent:**
> Your net proceeds will be $730,000.

---

**👤 You:**
> "Calculate a full summary for a business with $2M revenue, $400k profit, a 5x profit multiplier, $100k debt, $50k cash, 25% tax, and $20k fees. The original cost was $500k."

**🤖 AI Agent:**
> The valuation summary is: Enterprise Value: $2,000,000; Equity Value: $1,950,000; Total Tax: $362,500; Net Proceeds: $1,567,500.


## ❓ FAQ

**Q: How do I calculate the total market value of my company?**
You can use the `calculate_enterprise_value` tool by providing your annual revenue or profit and the appropriate industry multiplier.

**Q: What is the difference between Enterprise Value and Equity Value?**
Enterprise Value is the total market value of the business. Equity Value is what remains for the owners after subtracting debt and adding cash, which can be calculated using `calculate_equity_value`.

**Q: Can I get a full breakdown of my sale proceeds?**
Yes, the `generate_valuation_summary` tool provides a complete waterfall including Enterprise Value, Equity Value, taxes, and final Net Proceeds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/business-sale-valuation-scenario](https://vinkius.com/en/ai-agent-connect/business-sale-valuation-scenario)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Business Sale Valuation Scenario** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `business-sale-valuation-scenario` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Business Sale Valuation Scenario** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "business-sale-valuation-scenario": {
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
