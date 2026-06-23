# Treasury Return Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/treasury-return-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate fair price, YTM, and inflation-adjusted returns for US Treasuries, UK Gilts, and German Bunds.

## Description
This MCP server provides specialized financial tools to value sovereign debt instruments. Use `calculate_bond_valuation` to determine the fair market price and annualized total return (YTM) for bonds like US T-Bills, T-Notes, or German Bunds based on current market yields. The `calculate_inflation_adjusted_return` tool allows you to assess purchasing power preservation by adjusting nominal returns against expected inflation rates. Additionally, use `calculate_currency_equivalent_yield` to evaluate the yield of a foreign bond when converted into a target currency, accounting for exchange rate impacts.


## Available Tools (3)
- **calculate_bond_valuation**: Calculate fair market price and annualized total return (YTM) of a bond
- **calculate_currency_equivalent_yield**: Evaluate the yield of a foreign sovereign bond in a target currency
- **calculate_inflation_adjusted_return**: Assess purchasing power preservation by adjusting nominal return for inflation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Treasury Return Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the fair price of a US T-Note with a 3% coupon, 2 years to maturity, and a 4% market yield?"

**🤖 AI Agent:**
> The calculated fair price for the bond is 97.15.

---

**👤 You:**
> "If my bond has a 5% nominal return and inflation is expected to be 2%, what is my real return?"

**🤖 AI Agent:**
> Your inflation-adjusted real return is approximately 2.94%.

---

**👤 You:**
> "Calculate the yield of a GBP bond with 4% yield if the USD/GBP exchange rate is 1.25."

**🤖 AI Agent:**
> The converted yield in the target currency is 4.0%.


## ❓ FAQ

**Q: What types of bonds can I calculate?**
You can calculate valuations for US Treasuries (T-Bills, T-Notes, T-Bonds), UK Gilts, and German Bunds.

**Q: How do I calculate the real return of my investment?**
Use the `calculate_inflation_adjusted_return` tool by providing your nominal yield and the expected annual inflation rate.

**Q: Can I convert yields between different currencies?**
Yes, the `calculate_currency_equivalent_yield` tool allows you to evaluate a bond's yield in terms of a target currency using current exchange rates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/treasury-return-calculator](https://vinkius.com/mcp/treasury-return-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Treasury Return Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `treasury-return-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Treasury Return Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "treasury-return-calculator": {
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
