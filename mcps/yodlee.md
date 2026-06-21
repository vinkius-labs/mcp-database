# Yodlee MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yodlee)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/yodlee-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/yodlee-mcp)
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


## Installation & Usage

To install and use the **Yodlee** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yodlee](https://vinkius.com/mcp/yodlee)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
