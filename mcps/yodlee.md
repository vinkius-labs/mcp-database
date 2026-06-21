# Yodlee MCP Server

Access financial data via Yodlee — list accounts, fetch transactions, and verify banking details directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/yodlee)

## Overview
**Category:** finance-accounting
**Tools Count:** 13

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


## Installation & Usage

To install and use the **Yodlee** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yodlee](https://vinkius.com/mcp/yodlee)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
