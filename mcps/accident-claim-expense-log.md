# Accident Claim Expense Log MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accident-claim-expense-log)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize and track insurance claim expenses, reimbursements, and financial totals.

## Description
This MCP server manages the financial lifecycle of an insurance claim. It allows AI agents to retrieve high-level financial snapshots using `get_claim_summary`, list all incident costs via `list_expenses`, and inspect specific line items with `get_expense_details`. Agents can also advance the claim through its lifecycle stages using `update_claim_status`. It provides clear visibility into reimbursed, unreimbursed, pending, and out-of-pocket totals.


## Available Tools (4)
- **get_claim_summary**: Provides a high-level financial snapshot of the entire claim
- **get_expense_details**: Provides deep-dive information on a specific cost, including its reimbursement status
- **list_expenses**: Retrieves a chronological list of all costs associated with the accident
- **update_claim_status**: g., to Settled or Closed.

Advances the claim through its lifecycle stages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accident Claim Expense Log** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current financial summary for claim ID 12345?"

**🤖 AI Agent:**
> The current status for claim 12345 is Under Review. The reimbursed total is $500.00, the unreimbursed total is $250.00, the pending total is $100.00, and your out-of-pocket total is $350.00.

---

**👤 You:**
> "Show me all expenses for claim 98765 that happened in January."

**🤖 AI Agent:**
> In January, there were two expenses for claim 98765: a $150.00 medical bill on Jan 5th and a $45.00 towing fee on Jan 12th.

---

**👤 You:**
> "Can you update the status of claim 5544 to Settled?"

**🤖 AI Agent:**
> The status for claim 5544 has been successfully updated to Settled.


## ❓ FAQ

**Q: How can I see the total amount I still need to be reimbursed?**
You can use the `get_claim_summary` tool to see the unreimbursed total, which represents approved expenses not yet paid.

**Q: Can I change the status of a claim once it is closed?**
No, once a claim is moved to a terminal status like 'Closed' using `update_claim_status`, further modifications are prevented.

**Q: How do I get a list of all medical and property expenses?**
Use the `list_expenses` tool to retrieve a chronological list of all costs associated with the accident.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accident-claim-expense-log](https://vinkius.com/en/ai-agent-connect/accident-claim-expense-log)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accident Claim Expense Log** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accident-claim-expense-log` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accident Claim Expense Log** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accident-claim-expense-log": {
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
