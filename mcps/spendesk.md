# Spendesk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/spendesk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Empower your AI with real-time spend management. Track budgets, audit invoices, and review expense claims directly from your IDE.

## Description
Bring your **Spendesk** financial operations natively into your AI workspace. Eliminate constant tab switching to check the finance dashboard. You can now use conversational prompts to audit real-time company expenses, verify specific payment IDs, and inspect active supplier invoices while writing your integration code or managing operational scripts.

### What you can do

- **Track Cash Flow** — Monitor organizational outflows by executing `list_payments`. Need deep details on a specific transaction? Pull exactly what happened using `get_payment_details`
- **Audit Invoices & Expenses** — Keep track of pending vendor bills via `list_invoices` and review employee out-of-pocket reimbursements triggering `list_expense_claims`
- **Supplier Management** — Check your registered vendor matrix using `list_suppliers` and pull contact or payment history directly calling `get_supplier_details`
- **Control Limits** — Actively supervise remaining budget allocations calling `list_budgets` and watch the assigned corporate limits on issued plastic/virtual via `list_cards`

### How it works

1. Subscribe to this AI integration server
2. Introduce your official Spendesk Access Token
3. Start using Claude, Cursor, or your terminal IDE to query financial states autonomously

Stop managing financial syncs blindly and asking accountants to pull limits. Let your local AI understand your company's real-time spending constraints directly before triggering automated actions.

### Who is this for?

- **Finance Engineers** — test accounting webhooks or integrations reading live Spendesk data intuitively through pure conversational chat formats
- **Operation Managers** — use an agent to build quick markdown summaries on active budgets or compile how much a specific team spent on software this month
- **Founders & Admins** — query team members (`list_members`) or verify immediately if a virtual card (`list_cards`) has enough cap for a high-value purchase without logging in


## Available Tools (9)
- **get_payment_details**: Get detailed information about a specific payment
- **get_supplier_details**: Get detailed information about a specific supplier
- **list_budgets**: List all budgets and their spending status
- **list_cards**: List all virtual and physical cards issued
- **list_expense_claims**: List all employee expense claims and reimbursement requests
- **list_invoices**: List all invoices pending or processed
- **list_members**: List all team members with Spendesk access
- **list_payments**: List all payments in the Spendesk account
- **list_suppliers**: List all registered suppliers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spendesk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Review Spendesk and show me all recent payments hitting our account."

**🤖 AI Agent:**
> Pulling via `list_payments` request...

**Recent Transaction Flow**:
1. 💳 **Payment #p_xyz9000** - Vendor: AWS Cloud Services - Amount: $421.50 (Completed)
2. 💸 **Payment #p_klm1458** - Vendor: GitHub Inc - Amount: $20.00 (Processing)
3. 💳 **Payment #p_rst1098** - Vendor: Delta Airlines - Amount: $310.00 (Pending Approval)

Type the ID to fetch extended metadata explicitly via `get_payment_details` if you want.

---

**👤 You:**
> "Bring a quick summary containing our currently monitored budgets to check for remaining allocated thresholds."

**🤖 AI Agent:**
> Executing an integration pull triggering `list_budgets` against the current instance.

**Budget Dashboard Overview**:
- 🎯 `Q3 Core Operating Budget` (ID: 1x0a)
  - **Total Configured Amount**: €80,000 
  - **Status Remaining**: Active (Pending Spend: €12,410 remaining)

- 🎯 `Q3 Executive Marketing Pool` (ID: 2y0b)
  - **Total Configured Amount**: €150,000 
  - **Status Remaining**: Warning (Nearly Exhausted: €890 remaining)

I can list cards linked under these frameworks natively if required.

---

**👤 You:**
> "Let's check our member list in Spendesk to see who holds what permission roles currently."

**🤖 AI Agent:**
> Running the team hierarchy via mapping `list_members`. Here's your staff matrix:

- **Alice Jenkins** (a.jenkins@com.co)
  - *Role Profile*: Administrator / Owner

- **Bob S.** (bob.s@com.co)
  - *Role Profile*: Team Member (Standard)

- **Charlie Dao** (c.dao@com.co)
  - *Role Profile*: Accounting Approver / Admin

There are 12 additional standard users onboard, let me know if you need specific names verified.


## ❓ FAQ

**Q: Can the AI perform destructive actions like making a real payment or deleting invoices?**
No. The integration focuses strongly on extraction via READ endpoints (e.g. `list_payments`, `list_budgets`, `list_expense_claims`). It is designed to act as an advanced analytical viewing lens allowing you to query, organize, and monitor financial positions without executing operational mutations like transferring money.

**Q: How can the AI help me understand a specific expense claim?**
You can provide the Expense ID from your `list_expense_claims` search and ask natural questions. The AI will pull the structured data and explain explicitly who submitted the reimbursement, the exact amount, the associated spending currency, and the current processing status, formatting it all into an easily digestible summary.

**Q: How deep is the Spendesk token scoped? Is it secure?**
The integration is secure. Your Vinkius Agent runs strictly client-side on your PC. It queries the API using the explicit Bearer Token you manage. Spendesk's token access capabilities can also be carefully constrained natively from your Organization's Integration Settings to further enforce least privilege.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spendesk](https://vinkius.com/mcp/spendesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spendesk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spendesk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spendesk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spendesk": {
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
