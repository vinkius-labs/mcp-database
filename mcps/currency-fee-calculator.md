# Currency Fee Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/currency-fee-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise conversion fees and total transaction values.

## Description
This MCP server provides tools to calculate conversion costs for currency transactions. Use `get_conversion_fee` to find the specific service fee, `get_total_transaction_value` to determine the total capital required, `validate_fee_structure` to check if a fee is within business limits, or `summarize_transaction_costs` for a complete breakdown of principal, fee, and total.


## Available Tools (4)
- **get_total_transaction_value**: Calculates the total amount required to cover both the principal and the service fee
- **summarize_transaction_costs**: Provides a full breakdown of a conversion, including the principal, the fee, and the total
- **validate_fee_structure**: Checks if a proposed fee configuration meets specific business safety thresholds
- **get_conversion_fee**: Calculates only the specific service fee amount for a given transaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Currency Fee Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the fee for converting 1000 USD with a 2.5% fee?"

**🤖 AI Agent:**
> The conversion fee for 1000 USD at a 2.5% rate is 25 USD.

---

**👤 You:**
> "How much total will I need for a 500 EUR transaction with a 3% fee?"

**🤖 AI Agent:**
> The total transaction value is 515 EUR.

---

**👤 You:**
> "Give me a summary for 2000 GBP with a 1.5% fee."

**🤖 AI Agent:**
> The principal is 2000 GBP, the fee is 30 GBP, and the total value is 2030 GBP.


## ❓ FAQ

**Q: How do I calculate just the fee amount?**
You can use the `get_conversion_fee` tool by providing the principal amount and the fee percentage.

**Q: Can I see a full breakdown of the costs?**
Yes, the `summarize_transaction_costs` tool provides the principal, the fee amount, and the total value.

**Q: How do I check if a fee is too high?**
Use the `validate_fee_structure` tool to compare a proposed fee against a maximum allowed threshold.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/currency-fee-calculator](https://vinkius.com/en/ai-agent-connect/currency-fee-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Currency Fee Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `currency-fee-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Currency Fee Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "currency-fee-calculator": {
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
