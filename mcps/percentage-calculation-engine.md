# Percentage Calculation Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/percentage-calculation-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Stop LLMs from miscalculating discounts and interest. Deterministically calculate exact percentages and relative increases.

## Description
LLMs frequently fail when applying layered financial math, such as calculating a 15% discount followed by a 20% tax. They guess the answer based on training data. This MCP brings pure, native Javascript logic to percentage math.

### The Superpowers

- **Flawless Financials:** Ensure your AI calculates invoice discounts, VAT taxes, and interest correctly every single time.
- **Absolute Determinism:** No stochastics. Just native mathematical evaluation executed at the edge.


## Available Tools (2)
- **calculate_increase_by**: Increases or decreases a value by X percent deterministically (use negative percent for discount)
- **calculate_percent_of**: Pass the base value and the percentage to compute. Essential for discount calculations, tax rates, and financial reports.

Calculates X percent of a total value deterministically


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Percentage Calculation Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is exactly 15.5% of $2,500.00?"

**🤖 AI Agent:**
> ✅ **Percentage Extracted:** `$387.50`

---

**👤 You:**
> "Add a 20% VAT tax rate to the baseline price of $500."

**🤖 AI Agent:**
> ✅ **Increased Value:** The final price with VAT is `$600.00`.

---

**👤 You:**
> "Apply a 10% coupon discount to the shopping cart total of $1000."

**🤖 AI Agent:**
> ✅ **Decreased Value:** The new cart total is `$900.00`.


## ❓ FAQ

**Q: Can it calculate discounts?**
Yes, by passing a negative percentage.

**Q: Is it deterministic?**
Absolutely. Pure math evaluation local.

**Q: Does it support tax addition?**
Yes, simply use the increase_by function.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/percentage-calculation-engine](https://vinkius.com/mcp/percentage-calculation-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Percentage Calculation Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `percentage-calculation-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Percentage Calculation Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "percentage-calculation-engine": {
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
