# Household Bill Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-bill-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Equitably divide household expenses among all residents.

## Description
This MCP server manages shared household expenses by dividing bills equally among residents. Use `get_resident_list` to identify household members, `calculate_equal_split` to determine individual shares, and `record_bill_payment` to log expenses and assign debts. You can also use `get_resident_balances` to track who owes money or has credits within the household.


## Available Tools (4)
- **get_resident_list**: Retrieves the current list of residents registered in the household
- **calculate_equal_split**: Calculates how much each resident owes for a specific bill
- **get_resident_balances**: Provides a summary of the current financial standing for every resident in a household
- **record_bill_payment**: Records that a bill has been processed and assigns the debt to all residents


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Bill Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who are the residents in household ID 123?"

**🤖 AI Agent:**
> The residents in household 123 are Alice and Bob.

---

**👤 You:**
> "How much should each person pay for a $150.50 electricity bill in household 123?"

**🤖 AI Agent:**
> Each resident owes $75.25.

---

**👤 You:**
> "Record a rent payment of $2000 for household 123."

**🤖 AI Agent:**
> The rent payment of $2000 has been successfully recorded for household 123.


## ❓ FAQ

**Q: How are the bills divided?**
The total bill amount is divided equally among all registered residents in the household.

**Q: How can I see who owes money?**
You can use the `get_resident_balances` tool to see the current financial standing and outstanding debts for every resident.

**Q: Can I record different types of bills?**
Yes, you can use `record_bill_payment` to log any expense, such as rent, electricity, or one-time repairs, by providing a description.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-bill-splitter](https://vinkius.com/en/ai-agent-connect/household-bill-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Bill Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-bill-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Bill Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-bill-splitter": {
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
