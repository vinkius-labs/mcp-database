# Travel Cost Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/travel-cost-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate individual debts and optimize reimbursement transfers for shared travel expenses.

## Description
This MCP server provides a specialized engine for managing shared travel costs. It allows AI agents to process expense lists, determine the net financial standing of every traveler using `calculate_balances`, and identify the most efficient way to settle debts via `optimize_settlements`. You can also verify participant lists with `validate_trip_participants` and get a high-level overview of spending with `get_expense_summary`.


## Available Tools (4)
- **get_expense_summary**: Provides a high-level overview of total spending and individual contributions
- **validate_trip_participants**: Ensures that all individuals mentioned in expenses are recognized as valid participants
- **optimize_settlements**: Finds the most efficient way to move money between travelers to clear all debts
- **calculate_balances**: Determines the net financial standing of every participant in the trip


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Travel Cost Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the balances for these expenses: Alice paid 100 for Alice and Bob, and Bob paid 50 for Alice and Bob."

**🤖 AI Agent:**
> Alice has a balance of +25 and Bob has a balance of -25.

---

**👤 You:**
> "What is the most efficient way to settle these balances: Alice: +50, Bob: -20, Charlie: -30?"

**🤖 AI Agent:**
> Bob pays Alice 20 and Charlie pays Alice 30.

---

**👤 You:**
> "Give me a summary of these expenses: Alice paid 100 for Alice and Bob, and Bob paid 50 for Alice and Bob."

**🤖 AI Agent:**
> Total spent: 150. Unique payers: Alice, Bob. Transaction count: 2.


## ❓ FAQ

**Q: How do I calculate who owes what?**
You can use the `calculate_balances` tool by providing a list of expenses, including the payer and the beneficiaries for each.

**Q: How can I minimize the number of bank transfers?**
The `optimize_settlements` tool calculates the minimum number of transactions required to clear all debts among participants.

**Q: Can I check if all names in my expenses are valid?**
Yes, use the `validate_trip_participants` tool to ensure all names mentioned in expenses exist in your master participant list.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/travel-cost-splitter](https://vinkius.com/en/ai-agent-connect/travel-cost-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Travel Cost Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `travel-cost-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Travel Cost Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "travel-cost-splitter": {
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
