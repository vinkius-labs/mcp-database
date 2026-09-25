# Care Expense Reimbursement Workflow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-expense-reimbursement-workflow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Manage care-related expenses with receipt validation, share calculation, and automated reimbursement requests.

## Description
This MCP server provides a complete management system for processing care-related expenses. It connects AI agents to a structured workflow for validating receipt evidence, calculating participant shares based on agreed rules, and generating formal payment requests. Use `analyze_expense_compliance` to verify receipts, `calculate_reimbursement_shares` to split costs, and `generate_payment_request` to initiate transfers. The system also provides full auditability through `fetch_reimbursement_ledger` and real-time status updates via `get_reimbursement_status`.


## Available Tools (5)
- **analyze_expense_compliance**: Verify if a receipt meets evidence standards and approval rules
- **fetch_reimbursement_ledger**: Retrieve a transparent, chronological history of all transactions
- **get_reimbursement_status**: Provide a summary of actions, pending payments, and outstanding items
- **calculate_reimbursement_shares**: Determine how much each participant owes based on agreed rules
- **generate_payment_request**: Create a formal request for funds to be transferred to the claimant


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Expense Reimbursement Workflow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this receipt is compliant: vendor is 'CarePharmacy', date is '2023-10-01', and amount is 50.00. The approval contact is 'manager_01'."

**🤖 AI Agent:**
> The receipt is compliant. The vendor, date, and amount are all present and verified by manager_01.

---

**👤 You:**
> "Calculate how to split a 120.00 expense equally among Alice, Bob, and Charlie."

**🤖 AI Agent:**
> Each participant (Alice, Bob, and Charlie) owes 40.00.

---

**👤 You:**
> "Create a payment request for 40.00 to be sent to Alice by 2023-12-31 via Bank Transfer."

**🤖 AI Agent:**
> The payment request has been generated with ID REQ-123 for 40.00, due on 2023-12-31 via Bank Transfer.


## ❓ FAQ

**Q: How do I verify if a receipt is valid?**
You can use the `analyze_expense_compliance` tool to check if the receipt contains the necessary vendor, date, and amount information.

**Q: Can I split expenses between multiple people?**
Yes, the `calculate_reimbursement_shares` tool allows you to distribute costs using equal, percentage, or fixed rules among participants.

**Q: How can I see the history of all payments?**
Use the `fetch_reimbursement_ledger` tool to retrieve a transparent, chronological history of all expenses and reimbursements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-expense-reimbursement-workflow](https://vinkius.com/en/ai-agent-connect/care-expense-reimbursement-workflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Expense Reimbursement Workflow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-expense-reimbursement-workflow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Expense Reimbursement Workflow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-expense-reimbursement-workflow": {
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
