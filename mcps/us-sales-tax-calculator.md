# US Sales Tax Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-sales-tax-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise US sales and use tax liabilities based on jurisdiction, sourcing rules, and item exemptions.

## Description
This MCP server provides a high-precision engine for determining US sales and use tax obligations. It handles the complexities of multi-layered taxation (state, county, city, and special districts) and supports both destination-based and origin-based sourcing rules. Use `get_jurisdiction_rates` to retrieve full tax breakdowns for any ZIP code, `calculate_transaction_tax` to compute exact liabilities for specific transactions including tax-inclusive pricing, and `check_item_exemption` to verify if product categories like groceries or apparel are exempt in a particular state. It is designed to bridge AI agents with real-time US tax data.


## Available Tools (3)
- **calculate_transaction_tax**: Calculate the total tax liability for a transaction
- **check_item_exemption**: Check if an item category is exempt from tax
- **get_jurisdiction_rates**: Retrieve tax rates for a specific location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Sales Tax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the tax rates for ZIP code 90210 in California?"

**🤖 AI Agent:**
> For ZIP code 90210 (CA), the total combined rate is 9.5%. This includes a state rate of 7.25%, a county rate of 0.25%, and local district rates of 2.0%.

---

**👤 You:**
> "Calculate the tax for a $100 electronics purchase from 60601 to 90210."

**🤖 AI Agent:**
> The total tax amount is $9.50, making the final total $109.50. This calculation uses destination-based sourcing for California.

---

**👤 You:**
> "Is apparel exempt from sales tax in New York?"

**🤖 AI Agent:**
> In New York, certain clothing items are exempt from the state sales tax, though local district taxes may still apply.


## ❓ FAQ

**Q: How does the tool handle different sourcing rules?**
The `calculate_transaction_tax` tool automatically identifies whether a state uses destination-based or origin-based sourcing by comparing the provided origin and destination postal codes.

**Q: Can I check if specific items like groceries are exempt?**
Yes, you can use the `check_item_exemption` tool to determine if a product category is subject to tax or exempt in a specific state.

**Q: Does it support tax-inclusive pricing?**
Yes, when using `calculate_transaction_tax`, you can set the `isTaxInclusive` parameter to true to correctly calculate the taxable base amount from a price that already includes tax.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-sales-tax-calculator](https://vinkius.com/mcp/us-sales-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Sales Tax Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-sales-tax-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Sales Tax Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-sales-tax-calculator": {
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
