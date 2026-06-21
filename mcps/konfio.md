# Konfío MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/konfio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Automate your Konfío SMB banking and lending. Manage loans, pay invoices, track credit cards, and emit SAT-compliant CFDIs directly from any AI agent.

## Description
Connect your **Konfío** business account to any AI agent and manage Mexico's leading SMB financial suite through natural conversation. Whether you need to pay a loan, check credit limits, or emit electronic invoices (CFDIs), the AI handles the heavy lifting.

### What you can do

- **Loan Management** — Track active business loans, get amortization schedules, and make direct loan payments from your connected accounts
- **Credit Cards** — Review corporate credit card spending, check available limits, and fetch monthly statements for reconciliation
- **Electronic Invoicing (CFDI 4.0)** — List emitted and received SAT invoices, and generate new legally compliant invoices with automatic stamp generation
- **B2B Transfers** — Create SPEI transfers to suppliers and employees directly from your Konfío account
- **Credit Line Monitoring** — Check your business credit score status and apply for new working capital credit lines

### How it works

1. Subscribe to this server
2. Enter your Konfío Business API credentials
3. Start managing your PYME finances from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SMB Owners (PYMEs)** — monitor cash flow and loan balances without opening multiple banking apps
- **Accountants** — programmatically pull CFDI invoices and credit card transactions for end-of-month reconciliation
- **Finance Teams** — automate supplier SPEI transfers and invoice generation


## Available Tools
- **check_credit_status**: Check business credit rating and eligibility status
- **create_invoice**: 0 invoice for a client. Requires client RFC, tax regime, items, and CFDI usage code.

Create and emit a new electronic invoice (CFDI)
- **create_transfer**: Create a supplier B2B transfer (SPEI)
- **get_business_profile**: Get Konfío business profile
- **get_cc_statement**: Get a credit card monthly statement
- **get_credit_card**: Get business credit card details
- **get_loan_details**: Get details of a specific business loan
- **get_payment_schedule**: Get the amortization schedule for a loan
- **list_cc_transactions**: List credit card transactions
- **list_invoices**: You can filter by issued (emitted) or received invoices.

List electronic invoices (CFDIs)
- **list_loans**: List active and past business loans
- **list_transfers**: List B2B outgoing wire transfers
- **make_loan_payment**: Make a payment towards a business loan
- **request_credit_line**: Submit a new credit line request


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Konfío** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my latest business credit card transactions."

**🤖 AI Agent:**
> Here are your 3 most recent Konfío corporate card charges: 1. Amazon Web Services — $2,150.00 MXN (Cloud Hosting). 2. Home Depot — $4,300.00 MXN (Office supplies). 3. Uber — $350.00 MXN (Travel). Your current available credit is $145,000 MXN.

---

**👤 You:**
> "List the last 5 invoices we emitted to clients."

**🤖 AI Agent:**
> Your 5 most recent emitted CFDIs: 1. CFDI-8821: To 'TechCorp SA' for $11,600 MXN (Active). 2. CFDI-8820: To 'Logistics MX' for $5,800 MXN (Active). 3. CFDI-8819: To 'Juan Perez' for $1,160 MXN (Paid). Total emitted this period is $18,560 MXN.

---

**👤 You:**
> "Make a loan payment of $12,000 for loan LOAN-442."

**🤖 AI Agent:**
> Payment initiated! A direct debit of $12,000.00 MXN is being pulled from your primary connected bank account to pay towards LOAN-442. This covers your minimum installment of $10,500 with $1,500 going directly to the principal balance.


## ❓ FAQ

**Q: Can I emit legal Mexican electronic invoices (CFDIs) with this tool?**
Yes! Use the `create_invoice` tool. You just need to provide the client's RFC, the SAT usage code (e.g., G03), and the item details. Konfío will automatically stamp (timbrar) the XML document with the SAT network to make it fully legally binding in Mexico.

**Q: How do I check when my next loan payment is due?**
First use `list_loans` to find your active loan ID, then use `get_payment_schedule` with that ID to view all upcoming installments, breaking down principal, interest, and IVA taxes for each payment.

**Q: Can I pay suppliers via SPEI using my Konfío balance?**
Yes, use the `create_transfer` tool with the supplier's 18-digit CLABE number and the transfer amount. Konfío processes these as standard domestic SPEI wires.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/konfio](https://vinkius.com/mcp/konfio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Konfío** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `konfio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Konfío** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "konfio": {
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
