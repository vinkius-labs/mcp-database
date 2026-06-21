# Yodlee MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yodlee)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Access financial data via Yodlee — list accounts, fetch transactions, and verify banking details directly from any AI agent.

## Description
Connect your **Yodlee** developer account to any AI agent and gain programmatic access to financial data and account verification workflows through natural conversation.

### What you can do

- **Account Aggregation** — List all linked financial accounts and retrieve specific details for any account ID
- **Transaction History** — Fetch and filter transactions across all accounts by date, category, or keywords
- **Provider Discovery** — Search for supported financial institutions (providers) and inspect their login requirements
- **Account Linking** — Manage the process of linking new provider accounts or refreshing existing credentials
- **Verification Services** — Initiate and check the status of account verifications for secure onboarding

### How it works

1. Subscribe to this server
2. Enter your Yodlee Base URL, Client ID, and Secret
3. Start querying financial data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fintech Developers** — test API responses and verify account linking flows directly from the terminal or IDE
- **Financial Analysts** — aggregate transaction data and categorize expenses without manual CSV exports
- **Personal Finance Managers** — build custom dashboards or agents that track net worth and spending patterns across multiple institutions


## Available Tools
- **generate_token**: Generate a Yodlee access token
- **create_provider_account**: Link a new financial institution account
- **create_verification**: g., for ACH).

Initiate account verification
- **delete_account**: Remove an account from the user profile
- **get_account**: Get details for a specific account
- **get_provider_account**: Check the status of an account refresh or linking process
- **get_provider**: g., login requirements).

Get details about a specific provider
- **get_verification**: Retrieve verification results
- **list_accounts**: List all financial accounts for a user
- **list_providers**: Search for supported financial institutions
- **list_transaction_categories**: List available transaction categories
- **list_transactions**: Fetch transactions across all accounts
- **update_provider_account**: Update credentials or trigger a manual refresh


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Yodlee** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my linked financial accounts and their current balances."

**🤖 AI Agent:**
> I've retrieved your accounts. You have 3 linked accounts: a 'Premier Checking' (ID: 10123) with $4,250.00, a 'High Yield Savings' (ID: 10124) with $12,800.00, and a 'Travel Rewards Credit Card' (ID: 10125) with a balance of -$450.20.

---

**👤 You:**
> "Search for transactions containing 'Amazon' from the last 30 days."

**🤖 AI Agent:**
> Searching your history... I found 2 transactions: $45.99 at 'Amazon.com' on Oct 12th and $12.99 for 'Amazon Prime' on Oct 15th. Would you like more details on either of these?

---

**👤 You:**
> "Show me the details for the financial provider with ID 16441."

**🤖 AI Agent:**
> Fetching provider info... ID 16441 corresponds to 'Chase Bank'. It supports account aggregation and verification, requiring a username, password, and MFA for linking.


## ❓ FAQ

**Q: Can I filter transactions by a specific date range or category?**
Yes. Use the `list_transactions` tool with optional parameters like `fromDate`, `toDate`, and `categoryId` to narrow down your financial history.

**Q: How do I find if a specific bank is supported by Yodlee?**
You can use the `list_providers` tool to search for financial institutions and the `get_provider` tool to see specific details and requirements for that institution.

**Q: Is it possible to remove a linked account through the AI agent?**
Yes. The `delete_account` tool allows you to remove a specific account from the user profile by providing its unique Account ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yodlee](https://vinkius.com/mcp/yodlee)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Yodlee** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `yodlee` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Yodlee** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "yodlee": {
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
