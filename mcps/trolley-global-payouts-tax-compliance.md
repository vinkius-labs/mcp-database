# Trolley Global Payouts & Tax Compliance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/trolley-global-payouts-tax-compliance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Automate global payouts and tax compliance — manage recipients, payments, and tax forms via AI.

## Description
Equip your AI agent with the most powerful platform for global payouts and tax compliance through the **Trolley** MCP server. This integration provides real-time access to your Trolley dashboard, allowing your agent to manage recipients (payees), initiate and monitor payments, and ensure regulatory compliance with automated tax form tracking. Whether you are scaling a marketplace, managing a global workforce, or auditing financial distributions, your agent acts as a dedicated financial operations specialist through natural conversation.

### What you can do

- **Recipient Management** — List, retrieve, and create recipients for your payout workflows.
- **Payment Monitoring** — Track the status of global payments across various methods and currencies.
- **Tax Compliance** — Audit and retrieve tax forms (like W-8/W-9) for your recipients to ensure compliance.
- **Balance Inquiries** — Monitor your account balances across different funding sources and currencies.
- **Invoice Management** — Access and list invoices associated with your payees for better financial tracking.

### How it works

1. Subscribe to this server
2. Enter your Trolley API Key and API Secret
3. Start managing your global payouts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance Teams** — automate the manual overhead of managing global payees and tax compliance.
- **Marketplace Operators** — scale payout operations to thousands of providers worldwide.
- **Compliance Officers** — ensure all recipients have the necessary tax documentation before distribution.
- **Operations Managers** — maintain a clear view of balances and payment statuses in real-time.


## Available Tools
- **get_recipient**: Get a specific recipient
- **get_tax_forms**: ) associated with a specific recipient.

Get tax forms for a recipient
- **list_balances**: List account balances
- **list_invoices**: List invoices
- **list_payments**: List payments in Trolley
- **list_recipients**: List recipients in Trolley


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Trolley Global Payouts & Tax Compliance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my recipients in Trolley."

**🤖 AI Agent:**
> Retrieving your recipients... I found 25 payees including 'John Doe' and 'Jane Smith'. Would you like to see the details for a specific one?

---

**👤 You:**
> "What is the status of my latest payments?"

**🤖 AI Agent:**
> Checking payment history... Your 10 most recent payments are all in 'completed' status, except for one pending for 'Global Services Ltd'.

---

**👤 You:**
> "Check the tax form status for recipient 'R-123456'."

**🤖 AI Agent:**
> Retrieving tax documentation for R-123456... I found a W-8BEN form that was submitted and verified on January 10th. The recipient is currently compliant for payouts.


## ❓ FAQ

**Q: Can I check if a recipient has submitted their W-9 form?**
Yes! Use the `get_tax_forms` tool with the recipient ID. It will return the status and details of all tax forms associated with that person.

**Q: How do I see my current balance in EUR?**
Use the `list_balances` tool. It will return a list of all currency balances in your Trolley account, including EUR, USD, and others.

**Q: Can I track the status of a specific payment?**
Yes. Use the `get_payment` tool with the specific Payment ID to retrieve its real-time status (e.g., pending, completed, or failed) and other relevant details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/trolley-global-payouts-tax-compliance](https://vinkius.com/mcp/trolley-global-payouts-tax-compliance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Trolley Global Payouts & Tax Compliance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `trolley-global-payouts-tax-compliance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Trolley Global Payouts & Tax Compliance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "trolley-global-payouts-tax-compliance": {
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
