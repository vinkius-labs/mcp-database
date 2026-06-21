# Mono MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mono)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Automate financial data retrieval and payment orchestration via Mono — access account balances, transaction history, and initiate bank transfers directly from any AI agent.

## Description
Connect your **Mono** account to any AI agent to access real-time financial data and payment capabilities across African financial institutions through natural conversation.

### What you can do

- **Account Insights** — Fetch real-time balances, account numbers, and institution details for any linked account using `get_account`.
- **Transaction Analysis** — Query historical transaction data with filters for dates and types (credit/debit) via `get_transactions`.
- **Statement Retrieval** — Generate and download bank statements in JSON or PDF formats for auditing and reconciliation using `get_statement`.
- **Identity Verification** — Retrieve verified identity information including Full Name, BVN, and contact details with `get_identity`.
- **Payment Initiation** — Orchestrate direct bank transfers with custom references and descriptions using `initiate_payment`.

### How it works

1. Subscribe to this server
2. Enter your Mono Secret Key
3. Start managing financial data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fintech Developers** — Test and integrate Mono features directly from your code editor to maintain development flow.
- **Financial Analysts** — Automate the collection of statements and transaction logs for faster reporting and auditing.
- **Operations Teams** — Verify user identities and initiate payouts through simple natural language commands.


## Available Tools
- **get_account**: Get Mono account details
- **get_identity**: Get identity information for a Mono account
- **initiate_payment**: Initiate a direct bank transfer
- **get_statement**: Get bank statement for a Mono account
- **get_transactions**: Get transactions for a Mono account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mono** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the account details and balance for account ID 642a1b2c3d4e5f6g7h8i9j0k."

**🤖 AI Agent:**
> I've retrieved the details for account 642a1b2c3d4e5f6g7h8i9j0k. The account is held at GTBank with a current balance of 250,000 NGN. The account number is 0123456789.

---

**👤 You:**
> "List all credit transactions for account 642a1b2c... from the last month."

**🤖 AI Agent:**
> I found 3 credit transactions for the requested period. The largest was a transfer of 50,000 NGN on 15-10-2023 labeled 'Salary Deposit'. Would you like to see the full list?

---

**👤 You:**
> "Initiate a payment of 5000 kobo with reference 'REF-998' and description 'Service Fee'."

**🤖 AI Agent:**
> Payment initiation request sent. Reference: REF-998. Amount: 5000 kobo. Description: Service Fee. Please follow the redirect URL provided to complete the authorization.


## ❓ FAQ

**Q: Can I check the balance and institution details of a specific linked account?**
Yes! Use the `get_account` tool with the specific Account ID. The agent will return the current balance, account number, and the name of the financial institution.

**Q: How do I download a bank statement in PDF format for a specific period?**
You can use the `get_statement` tool. Specify the `account_id`, set the `output` parameter to 'pdf', and define the `period` (e.g., 'last6months') to receive the statement data.

**Q: Is it possible to verify the identity of the account holder?**
Absolutely. The `get_identity` tool allows you to fetch verified information such as the holder's full name, BVN, phone number, and registered address directly from the linked bank account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mono](https://vinkius.com/mcp/mono)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mono** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mono` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mono** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mono": {
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
