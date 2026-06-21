# Flip MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flip)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage disbursements, validate bank accounts, and receive payments via AI agents with Flip.

## Description
Connect your **Flip** (Flip.id) account to any AI agent and automate your financial operations through the Model Context Protocol (MCP). Flip for Business provides a powerful API for making bulk disbursements, accepting payments via links or virtual accounts, and validating bank details. Now, you can manage your Indonesian payouts and collection workflows directly through natural conversation.

### What you can do

- **Money Transfers (Disbursement)** — Initiate real-time money transfers to Indonesian bank accounts individually or in bulk.
- **Payment Collection (Bills)** — Create payment links (Bills) to receive funds from your customers effortlessly.
- **Bank Account Validation** — Instantly verify if a bank account exists and retrieve the holder's name before sending money.
- **Balance Monitoring** — Get a real-time view of your Flip business account balance to ensure sufficient liquidity.
- **Bank Discovery** — List all supported banks and cities to facilitate accurate transaction entry.
- **Transaction History** — Retrieve lists of recent payouts and received payments to keep your records synchronized.
- **Recurring Tasks** — Monitor configured recurring disbursement tasks directly through the agent.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Flip Secret Key (found in your Flip for Business dashboard)
3. Start managing your payouts and collections from Claude, Cursor, or any MCP client

### Who is this for?

- **Finance Operations** — quickly initiate or verify disbursements without navigating complex banking portals.
- **SaaS Platforms** — automate the creation of payment links for user subscriptions and track incoming funds.
- **Business Owners** — get a quick overview of account balances and recent transaction history via simple AI commands.


## Available Tools
- **create_bill**: Create payment link (Bill)
- **create_disbursement**: Send money (payout)
- **get_balance**: Check account balance
- **get_bill**: Get bill details
- **list_cities**: List supported cities
- **get_disbursement**: Get payout details
- **list_banks**: List supported banks
- **list_bills**: List payment links
- **list_disbursements**: List payouts
- **list_payments**: List received payments
- **list_recurring_payments**: List recurring payments
- **validate_bank_account**: Verify bank account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flip** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate bank account '12345678' at bank 'bca'."

**🤖 AI Agent:**
> Validating account... I've checked the details with Flip. The account is valid and belongs to 'BUDI SANTOSO'. Would you like to proceed with a disbursement to this account?

---

**👤 You:**
> "Create a payment link for 500,000 IDR titled 'Service Fee'."

**🤖 AI Agent:**
> Bill created! I've generated a payment link for 500,000 IDR with the title 'Service Fee'. The Bill ID is 'bill_987'. Your customer can pay using this link: https://flip.id/p/abc123xyz.

---

**👤 You:**
> "What is my current Flip account balance?"

**🤖 AI Agent:**
> Checking your balance... You currently have 15,250,000 IDR available in your Flip for Business account. You are ready to process your next batch of disbursements.


## ❓ FAQ

**Q: How do I validate an Indonesian bank account before sending money?**
You can use the 'validate_bank_account' tool. Provide the bank code and account number, and the agent will call the Flip Bank Account Inquiry API to confirm the account is valid and return the registered holder's name.

**Q: Can I check my current account balance using this server?**
Yes! The 'get_balance' tool retrieves the current available balance of your Flip for Business account, helping you ensure you have enough funds for your upcoming disbursements.

**Q: How do I create a payment link for a customer?**
Use the 'create_bill' tool. Provide a title and the amount in IDR. The agent will generate a payment link (Bill) that you can share with your customer to collect the funds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flip](https://vinkius.com/mcp/flip)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flip** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `flip` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flip** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flip": {
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
