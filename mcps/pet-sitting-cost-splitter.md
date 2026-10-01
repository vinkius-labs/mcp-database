# Pet-Sitting Cost Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-sitting-cost-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Splits pet-sitting, boarding, transport, and supply expenses between owners using responsibility dates and custom shares.

## Description
This MCP server acts as a financial reconciliation engine for pet owners. It allows AI agents to divide expenses like sitting, boarding, transport, and supplies among multiple participants. By using specific responsibility windows and custom cost-sharing ratios, the engine calculates precise itemized amounts owed. Users can use `get_expense_summary` to see total liabilities, `calculate_proportional_splits` to see individual breakdowns for specific costs, and `get_settlement_plan` to generate the most efficient list of transfers to settle all debts. It also includes `validate_ownership_window` to ensure responsibility periods are logically sound.


## Available Tools (4)
- **get_expense_summary**: Provides a high-level overview of all recorded expenses and the current total liability per owner
- **get_settlement_plan**: Generates the most efficient list of monetary transfers required to settle all outstanding debts
- **calculate_proportional_splits**: Calculates exactly how much each owner owes for each specific expense based on their dates of responsibility
- **validate_ownership_window**: Checks if a proposed period of responsibility is valid for a specific owner and expense


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet-Sitting Cost Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current balance for each owner?"

**🤖 AI Agent:**
> Owner A is owed $50.00, and Owner B owes $50.00.

---

**👤 You:**
> "Show me the settlement plan to clear all debts."

**🤖 AI Agent:**
> Owner B should transfer $50.00 to Owner A.

---

**👤 You:**
> "How much does Owner A owe for expense ID 123?"

**🤖 AI Agent:**
> Owner A owes $15.50 for that expense.


## ❓ FAQ

**Q: How are costs split between owners?**
Costs are split based on defined responsibility windows and custom cost shares. You can use `calculate_proportional_splits` to see the exact breakdown for any expense.

**Q: How can I see who owes what?**
You can use `get_expense_summary` to view the current total liability and balances for each owner, or `get_settlement_plan` to see the specific transfers needed to settle up.

**Q: Can I use custom ratios instead of 50/50?**
Yes, the engine supports custom cost shares, allowing owners to agree on any ratio (e.g., 60/40) during their period of responsibility.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-sitting-cost-splitter](https://vinkius.com/en/ai-agent-connect/pet-sitting-cost-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet-Sitting Cost Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-sitting-cost-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet-Sitting Cost Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-sitting-cost-splitter": {
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
