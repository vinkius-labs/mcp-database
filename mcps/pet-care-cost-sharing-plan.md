# Pet Care Cost Sharing Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-care-cost-sharing-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage and reconcile shared pet expenses among co-owners using explicit contribution rules.

## Description
This MCP server provides a structured way for pet co-owners to manage shared finances. It allows AI agents to calculate individual responsibilities, identify reimbursement actions, and flag unsupported costs that fall outside agreed categories. Use `calculate_responsibility_plan` to determine how much each owner owes, `generate_reimbursement_actions` to settle balances, and `create_reconciliation_agenda` to prepare for monthly financial reviews.


## Available Tools (5)
- **create_reconciliation_agenda**: Prepares a structured list of topics for a monthly meeting to review finances
- **generate_exception_report**: Raises specific questions regarding costs that fall outside the agreed-upon framework
- **generate_reimbursement_actions**: Identifies specific financial actions needed to settle up after expenses are paid
- **verify_payment_status**: Confirms if recent payments have been successfully applied to the shared ledger
- **calculate_responsibility_plan**: Generates an itemized breakdown of how much each owner owes for a set of invoices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Care Cost Sharing Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate how much Alice and Bob owe for these invoices: [{'amount': 50, 'category': 'Food', 'date': '2023-10-01'}, {'amount': 30, 'category': 'Vet', 'date': '2023-10-05'}]. Alice pays 60% and Bob pays 40%."

**🤖 AI Agent:**
> { "itemizedCosts": { "Alice": 48, "Bob": 32 }, "unsupportedCosts": [] }

---

**👤 You:**
> "Who needs to pay whom to settle up? Invoices: [{'amount': 100, 'payerName': 'Alice', 'category': 'Food', 'date': '2023-10-01'}]. Responsibility: Alice 50, Bob 50."

**🤖 AI Agent:**
> { "actions": [{ "fromOwner": "Bob", "toOwner": "Alice", "amount": 50, "method": "direct transfer" }] }

---

**👤 You:**
> "Are there any expenses that don't match our approved categories: ['Food', 'Vet']? Invoices: [{'amount': 20, 'category': 'Toys', 'date': '2023-10-10'}]."

**🤖 AI Agent:**
> { "questions": [{ "category": "Toys", "amount": 20, "reasoning": "The category 'Toys' is not in the approved list." }] }


## ❓ FAQ

**Q: How does the system handle unexpected expenses?**
Unexpected expenses are identified using `generate_exception_report`, which flags any invoice with a category not found in the approved list.

**Q: Can I use this to settle debts between owners?**
Yes, `generate_reimbursement_actions` identifies exactly who needs to pay whom to reach the agreed financial equilibrium.

**Q: How do I prepare for our monthly pet expense meeting?**
You can use `create_reconciliation_agenda` to generate a structured list of topics, including total spent and pending balances.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-care-cost-sharing-plan](https://vinkius.com/en/ai-agent-connect/pet-care-cost-sharing-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Care Cost Sharing Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-care-cost-sharing-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Care Cost Sharing Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-care-cost-sharing-plan": {
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
