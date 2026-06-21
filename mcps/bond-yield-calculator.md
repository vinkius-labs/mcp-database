# Bond Yield Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bond-yield-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate YTM, Current Yield, and interest rate sensitivity for fixed-income bonds.

## Description
This MCP server provides advanced financial engineering tools to value fixed-income instruments. Using the `get_bond_yield_metrics` tool, you can determine the Yield to Maturity (YTM) and Current Yield based on market price, face value, and coupon rates. It also calculates risk metrics like Modified Duration and Convexity, and estimates price volatility for various interest rate shifts (1bp, 25bp, and 100bp). Perfect for bond traders and analysts needing precise sensitivity analysis.


## Available Tools (1)
- **get_bond_yield_metrics**: Calculate Yield to Maturity (YTM), Current Yield, and interest rate sensitivity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bond Yield Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected annual return profile of a bond with a market price of 950, face value of 1000, coupon rate of 5%, semi-annual payments, and 5 years to maturity?"

**🤖 AI Agent:**
> The Yield to Maturity (YTM) is approximately 6.17% and the Current Yield is 5.26%.

---

**👤 You:**
> "How much risk does a bond with market price 980, face value 1000, coupon rate 4%, annual payments, and 10 years to maturity carry regarding interest rate movements?"

**🤖 AI Agent:**
> The bond has a Modified Duration of approximately 8.25 and a Convexity of 75.4.

---

**👤 You:**
> "How will the bond's price change if interest rates shift by 100 basis points? (Price: 950, Face: 1000, Coupon: 6%, Frequency: 2, Maturity: 3)"

**🤖 AI Agent:**
> A 100 basis point increase in rates is estimated to cause a price decrease of approximately 4.5%.


## ❓ FAQ

**Q: What can I calculate with this server?**
You can calculate Yield to Maturity (YTM), Current Yield, Modified Duration, Convexity, and price sensitivity scenarios for bonds.

**Q: How do I use the `get_bond_yield_metrics` tool?**
Provide the market price, face value, annual coupon rate, payment frequency, and years to maturity as numerical inputs.

**Q: Does it support different payment frequencies?**
Yes, you can specify any number of payments per year (e.g., 1 for annual, 2 for semi-annual, 4 for quarterly).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bond-yield-calculator](https://vinkius.com/mcp/bond-yield-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bond Yield Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bond-yield-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bond Yield Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bond-yield-calculator": {
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
