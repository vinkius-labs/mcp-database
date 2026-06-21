# Fig Finance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fig-finance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Connect Fig Finance to automate embedded lending — manage customers, query loan offers, and handle disbursements directly from your AI agent.

## Description
Fig Finance is an AI-powered embedded finance platform for emerging markets. This MCP server allows your AI agent to interact with your Fig Finance account flawlessly.

### Key Features
- **Customer Orchestration** — Register and manage customer profiles for real-time credit assessment natively.
- **Loan Intelligence** — Query tailored loan offers and track application statuses flawlessly through the agent.
- **Disbursement Flow** — Trigger and monitor fund disbursements for approved loans synchronously.
- **Repayment Tracking** — Access detailed repayment schedules and status for active loans flawlessly.
- **Financial Overview** — Monitor your account balance and transaction history flawlessly natively.
- **Identity Verification** — Verify the authorized application and profile details through the agent flawlessly.

### How it works
1. Subscribe to this server
2. Enter your Fig Finance API Key (found in your partner dashboard)
3. Start managing your embedded lending from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Fintech Partners** — integrate credit products into your existing platform without manual portal navigation
- **B2B Marketplaces** — manage merchant financing and vendor credit directly from your chat workflow
- **Operations Teams** — automate loan tracking and customer assessment through simple natural language queries


## Available Tools
- **apply_for_loan**: Apply for a loan on behalf of a customer
- **create_customer**: Register a new customer for lending
- **disburse_funds**: Trigger fund disbursement for an approved loan
- **get_balance**: Get current wallet balance in Fig Finance
- **get_customer**: Get details for a specific customer
- **get_loan_offers**: Get available loan offers for a customer
- **get_loan_status**: Get the current status of a loan
- **get_me**: Get details for the authorized application account
- **get_repayments**: Get the repayment schedule and status for a loan
- **list_customers**: List all customers in your Fig Finance account
- **list_loans**: List all loans in the account
- **list_transactions**: List all financial transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fig Finance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all customers in my Fig Finance account."

**🤖 AI Agent:**
> I've retrieved your customer list. You have 25 registered customers, including 'Samuel Okoro' (ID: cust_101) and 'Adaeze Nwosu' (ID: cust_102). Which customer would you like to check for loan offers?

---

**👤 You:**
> "Show me the available loan offers for customer cust_101."

**🤖 AI Agent:**
> Inspecting offers... For Samuel Okoro, I found 2 available offers: a 'Nano Loan' of 50,000 NGN (3 months) and a 'Growth Capital' offer of 250,000 NGN (6 months). Would you like to apply for either?

---

**👤 You:**
> "What is my current account balance?"

**🤖 AI Agent:**
> Retrieving balance... Your current Fig Finance wallet balance is 1,250,000.00 NGN. Shall I list the recent transactions for this month?


## ❓ FAQ

**Q: How do I obtain my Fig Finance API Key?**
You can generate your API Key within your Fig Finance Partner Dashboard under the **Developer** or **API Keys** section.

**Q: Does Fig Finance support real-time disbursement?**
Yes, Fig Finance focuses on automated and near-instant disbursements once a loan application is approved through its AI algorithms.

**Q: Can I check the wallet balance of my account?**
Yes! The `get_balance` tool allows you to retrieve the current available balance in your Fig Finance account flawlessly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fig-finance](https://vinkius.com/mcp/fig-finance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fig Finance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fig-finance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fig Finance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fig-finance": {
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
