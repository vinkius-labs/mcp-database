# ChargeOver MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chargeover-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Bill your customers with flexible recurring invoicing, automated dunning, and payment collection that keeps revenue flowing.

## Description
Connect your **ChargeOver** account to any AI agent and take full control of your recurring revenue and subscription billing workflows through natural conversation.

### What you can do

- **Billing Profile Orchestration** — List and manage customer billing profiles programmatically, retrieving detailed high-fidelity account metadata and payment history
- **Subscription Lifecycle Management** — Create and update recurring billing packages programmatically to maintain perfectly coordinated subscriber journeys
- **Invoice & Statement Architecture** — Monitor real-time invoice history and programmatically generate new billing statements to streamline your accounts receivable
- **Transaction Intelligence** — Track payment transactions, refunds, and credits in real-time to maintain a high-fidelity overview of your financial health
- **Operational Monitoring** — Access high-level billing summaries and manage account-level metadata directly through your agent for instant financial reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** (Username) and **API Secret** (Private Key) from ChargeOver (Settings > Developers > REST API)
3. Identify your **Subdomain** (e.g., 'acme' from acme.chargeover.com)
4. Start managing your recurring revenue from Claude, Cursor, or any MCP client

No more manual entry into billing tables or digging through subscription lists. Your AI acts as your dedicated billing coordinator and revenue analyst.

### Who is this for?

- **Finance & Billing Teams** — instantly retrieve payment statuses and update customer billing data using natural language commands
- **SaaS Founders** — monitor recurring revenue trends and manage subscription packages without leaving your workspace
- **Operations Leads** — automate invoice generation and track transaction histories through simple AI queries


## Available Tools
- **create_billing_customer**: Create a new customer
- **create_billing_invoice**: Create a new invoice
- **create_subscription**: Create a new subscription
- **list_billing_customers**: List all customers
- **list_billing_invoices**: List all invoices
- **list_subscriptions**: List all subscriptions (packages)
- **list_billing_transactions**: List all transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ChargeOver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active billing customers in ChargeOver."

**🤖 AI Agent:**
> I've retrieved your billing directory. You currently have 150 active customers, including 'Acme Corp' (ID: 1024) and 'Global Logistics'. Which one would you like to check for outstanding invoices?

---

**👤 You:**
> "Show the last 5 payment transactions and their status."

**🤖 AI Agent:**
> Accessing transaction logs... Out of the last 5, four were 'Successful' and one is 'Pending' ($250.00 from @user1). Shall I retrieve the detailed metadata for the pending payment?

---

**👤 You:**
> "Create a new subscription for 'Acme Corp' (ID: '1024') titled 'Pro Plan'."

**🤖 AI Agent:**
> Subscription created! I've successfully initialized the 'Pro Plan' for Acme Corp. The new billing package ID is 'pkg_789'. The customer will be automatically billed according to your account's default cycle.


## ❓ FAQ

**Q: How do I find my ChargeOver API credentials?**
Log in to your account, navigate to **Settings** > **Developers** > **REST API**, and copy your API Key (Username) and API Secret (Private Key).

**Q: Can I create a new subscription via AI?**
Yes! Use the `create_subscription` tool and provide the customer ID and a nickname for the billing package to initialize a new recurring plan.

**Q: How do I check a customer's payment history?**
The `list_billing_transactions` tool retrieves a detailed history of all payments, refunds, and credits associated with your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chargeover-alternative](https://vinkius.com/mcp/chargeover-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ChargeOver** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `chargeover-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ChargeOver** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chargeover-alternative": {
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
