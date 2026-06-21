# BILL (Bill.com) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bill-billcom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage financial operations via BILL — list vendors, customers, bills, and invoices directly from any AI agent.

## Description
Connect your **BILL (formerly Bill.com)** account to any AI agent and orchestrate your accounts payable and receivable workflows through natural conversation.

### What you can do

- **Accounts Payable Oversight** — List and inspect all incoming bills and vendor details to manage your payables effectively.
- **Accounts Receivable Management** — Query and retrieve details for outgoing invoices and customer profiles.
- **Vendor & Customer Directory** — Access your complete directory of business contacts with detailed metadata.
- **Financial Auditing** — List your chart of accounts and verify financial records directly from your workspace.
- **Profile Insights** — Retrieve authenticated user profile information for account verification.

### How it works

1. Subscribe to this server
2. Enter your BILL Dev Key, User Name, Password, and Org ID
3. Start managing your financial operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance Managers & CFOs** — quickly check pending bills and customer aging without opening the full portal.
- **Accountants** — retrieve vendor details and invoice statuses straight from their workflow tools.
- **Operations Teams** — verify business contact information and account structures using natural language.


## Available Tools
- **get_bill**: Get specific bill details
- **get_customer**: Get specific customer details
- **get_invoice**: Get specific invoice details
- **get_user_profile**: Get authenticated user profile
- **get_vendor**: Get specific vendor details
- **list_accounts**: List all chart of accounts
- **list_bills**: List all bills (accounts payable)
- **list_customers**: List all customers
- **list_invoices**: List all invoices (accounts receivable)
- **list_vendors**: List all vendors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BILL (Bill.com)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all unpaid bills in my account."

**🤖 AI Agent:**
> I've retrieved your unpaid bills. You have 4 pending payments, including 'Office Rent' (ID: bill_1) and 'Cloud Services' (ID: bill_2). Would you like the due dates for these?

---

**👤 You:**
> "Find the vendor details for 'Global Logistics'."

**🤖 AI Agent:**
> I found a vendor matching 'Global Logistics' (ID: vend_992). Their primary contact is Mark Johnson, and they are currently set up for electronic payments.

---

**👤 You:**
> "Show my last 5 customer invoices."

**🤖 AI Agent:**
> Retrieving invoices... Your 5 most recent customer invoices include 'INV-1001' (Status: Paid) and 'INV-1005' (Status: Unpaid). Would you like to see the amount for the unpaid invoice?


## ❓ FAQ

**Q: Can I check the status of a specific bill using the agent?**
Yes! Use the `get_bill` tool with the Bill ID. Your agent will fetch the latest status, including whether it is unpaid, partially paid, or fully paid.

**Q: How do I list all my active vendors in BILL?**
Simply ask the agent to `list_vendors`. It will retrieve the directory of all business vendors registered in your BILL account.

**Q: Does the integration support paying bills directly through the agent?**
No. For security and to comply with MFA requirements for financial transactions, the current toolset is focused on querying and auditing (listing bills, checking statuses). Initiating payments must be done through the official BILL platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bill-billcom](https://vinkius.com/mcp/bill-billcom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BILL (Bill.com)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bill-billcom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BILL (Bill.com)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bill-billcom": {
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
