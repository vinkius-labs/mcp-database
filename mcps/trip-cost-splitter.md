# Trip Cost Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/trip-cost-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate individual balances and determine the most efficient way to settle shared trip expenses.

## Description
Trip Cost Splitter helps groups of travelers manage shared expenses across multiple currencies. It calculates the net financial position of every participant and identifies the minimum number of transfers needed to settle all debts. Use `calculate_net_balances` to find out who owes what, `suggest_settlements` to get a clear list of transfers, `convert_currency` for quick conversions, and `validate_trip_data` to ensure all participants and currencies are correctly recorded.


## Available Tools (4)
- **calculate_net_balances**: Calculate the net financial position of every participant
- **convert_currency**: Translate a specific amount from one currency to another
- **suggest_settlements**: Provide a list of specific transfers required to settle debts
- **validate_trip_data**: Ensure all participants and currencies are present in the reference data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Trip Cost Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the net balances for Alice, Bob, and Charlie. Alice paid 100 USD for everyone. Bob and Charlie are beneficiaries. The exchange rate for USD is 1.0."

**🤖 AI Agent:**
> Alice: +66.67 USD, Bob: -33.33 USD, Charlie: -33.33 USD.

---

**👤 You:**
> "Suggest settlements for these balances: Alice: +50 USD, Bob: -20 USD, Charlie: -30 USD."

**🤖 AI Agent:**
> Bob pays Alice 20 USD and Charlie pays Alice 30 USD.

---

**👤 You:**
> "Convert 50 EUR to USD using an exchange rate where 1 EUR = 1.1 USD."

**🤖 AI Agent:**
> 55.0 USD


## ❓ FAQ

**Q: How does the tool handle different currencies?**
The tool uses provided exchange rates to normalize all expenses to a single base currency, ensuring accurate debt calculation regardless of the original currency used.

**Q: What is the most efficient way to settle debts?**
You can use the `suggest_settlements` tool, which matches the largest debtors with the largest creditors to minimize the total number of transactions required.

**Q: Can I verify if my trip data is complete?**
Yes, the `validate_trip_data` tool checks if all participants and currencies mentioned in your expenses are present in your reference data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/trip-cost-splitter](https://vinkius.com/en/ai-agent-connect/trip-cost-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Trip Cost Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `trip-cost-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Trip Cost Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "trip-cost-splitter": {
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
