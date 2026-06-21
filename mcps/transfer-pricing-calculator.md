# Transfer Pricing Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/transfer-pricing-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Verify arm's length compliance for related-party transactions using CUP, Cost Plus, and Resale Minus methods.

## Description
The Transfer Pricing Calculator ensures that transactions between related parties follow the Arm's Length Principle. By using tools like `get_industry_benchmarks`, `verify_cost_plus_compliance`, `verify_resale_minus_compliance`, and `verify_cup_equivalence`, businesses can determine if their pricing strategies align with industry-standard profit margins and market benchmarks, mitigating tax risks.


## Available Tools
- **get_industry_benchmarks**: Retrieves the acceptable arm's length profit margin bounds for a specific industry sector
- **verify_cup_equivalence**: Evaluates if a transaction price is sufficiently similar to a known market benchmark price
- **verify_resale_minus_compliance**: Determines if the gross margin from a resale transaction is within acceptable industry bounds
- **verify_cost_plus_compliance**: Determines if a transaction's markup on cost is within the allowed arm's length range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Transfer Pricing Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is a 15% markup on a $100 unit cost compliant in the Manufacturing sector?"

**🤖 AI Agent:**
> The applied markup is 15%. Based on the Manufacturing sector benchmarks, this falls within the acceptable arm's length range.

---

**👤 You:**
> "Check if a resale price of $500 with a purchase price of $450 is compliant for Retail."

**🤖 AI Agent:**
> The gross margin is 10%. For the Retail sector, this is within the allowed arm's length bounds.

---

**👤 You:**
> "Compare a transaction price of $95 to a market benchmark of $100 with a 2% tolerance."

**🤖 AI Agent:**
> The price variance is 5%. Since this exceeds the allowed tolerance of 2%, the transaction is not compliant.


## ❓ FAQ

**Q: What is the Arm's Length Principle?**
It is a standard that requires transactions between related parties to be priced as if they were between independent entities under similar circumstances.

**Q: How can I check if my markup is compliant?**
You can use the `verify_cost_plus_compliance` tool by providing your unit cost, transaction price, and the relevant industry sector.

**Q: Does this tool support different industries?**
Yes, you can use `get_industry_benchmarks` to retrieve specific margin bounds for sectors like Manufacturing, Services, Retail, and Logistics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/transfer-pricing-calculator](https://vinkius.com/mcp/transfer-pricing-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Transfer Pricing Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `transfer-pricing-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Transfer Pricing Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "transfer-pricing-calculator": {
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
