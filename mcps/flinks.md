# Flinks MCP Server

Connect to financial institutions to aggregate banking data, verify income, and perform deep transaction analysis via Flinks.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/flinks)

## Overview
**Category:** data-analytics
**Tools Count:** 15

## Description
Connect your **Flinks** instance to any AI agent to access real-time banking data, verify financial health, and automate KYC workflows through natural conversation.

### What you can do

- **Account Aggregation** — Retrieve full account details, balances, and transaction history from thousands of supported financial institutions.
- **Income Verification** — Use `get_income_attributes` to analyze income stability, sources, and verification patterns automatically.
- **Credit & Risk Analysis** — Fetch consumer or business analysis attributes to understand credit risk and financial behavior.
- **Transaction Categorization** — Automatically categorize bank transactions to understand spending patterns and merchant data.
- **Document Retrieval** — Fetch original bank-issued PDF statements (Canada only) for auditing and compliance.

### How it works

1. Subscribe to this server
2. Enter your Flinks Instance, Customer ID, API Key, and Secret Key
3. Start querying financial data directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Fintech Developers** — Test and integrate banking data flows without leaving the code editor.
- **Lending & Credit Teams** — Instantly analyze income and risk attributes for loan applications.
- **Accounting Professionals** — Automate the retrieval of transaction summaries and categorized data for reconciliation.


## Available Tools
- **authorize_session**: Authenticate a session and fetch cached banking data
- **create_transaction**: Requires FLINKS_CLIENT_ID credential.

Create an EFT transaction (debit or credit)
- **delete_card**: Delete all data associated with a specific user account
- **field_match**: Verify customer identity by comparing details against bank data
- **generate_authorize_token**: Valid for 30 minutes.

Generate a one-time authorize token
- **get_accounts_detail_async**: Poll for asynchronous account details processing
- **get_accounts_detail**: If 202 is returned, data is processing and you should poll the async endpoint.

Retrieve full account details including transactions and KYC
- **get_accounts_summary**: Retrieve general account details and balances
- **get_business_analysis_attributes**: Get insights for business underwriting and creditworthiness
- **get_categorization**: Get categorized transaction data
- **get_income_attributes**: Get income verification and stability insights
- **get_statements**: Retrieve original bank-issued PDF statements (Canada Only)
- **get_user_analysis_attributes**: Get credit-risk use-case attributes for a consumer
- **list_institutions**: List all available financial institutions supported by Flinks
- **set_scheduled_refresh**: Enable or disable nightly refreshes for a specific account


## Installation & Usage

To install and use the **Flinks** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flinks](https://vinkius.com/mcp/flinks)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
