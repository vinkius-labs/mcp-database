# Nubank MX MCP Server

Manage your Nubank Mexico banking from any AI agent — check balances, review transactions, send SPEI transfers, pay bills, and track spending analytics.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/nubank-mx)

## Overview
**Category:** industry-titans
**Tools Count:** 14

## Description
Connect your **Nubank Mexico** account to any AI agent and take control of your personal banking through natural conversation.

### What you can do

- **Account Overview** — Check your Cuenta balance, CLABE number, and annual yield (rendimiento) on deposits in real-time
- **Transaction History** — Browse and inspect debit card purchases, SPEI transfers, ATM withdrawals, and incoming deposits with full merchant details
- **Credit Card Management** — View your credit limit, current balance, monthly statements, meses sin intereses purchases, and minimum payment due dates
- **SPEI Transfers** — Send instant interbank transfers to any Mexican bank account using CLABE numbers, with concept descriptions and recipient tracking
- **Bill Payments** — Pay CFE, Telmex, water, internet, and other Mexican utility services directly from your Cuenta balance
- **Spending Intelligence** — Access AI-powered spending analytics by category, with monthly trends and top merchant insights

### How it works

1. Subscribe to this server
2. Enter your Nubank API Key and Client Secret
3. Start managing your finances from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Personal Finance Enthusiasts** — monitor spending patterns and optimize budgets through natural conversation
- **Freelancers** — track income deposits and outgoing payments without navigating the mobile app
- **Financial Advisors** — query client portfolio and spending data programmatically


## Available Tools
- **create_transfer**: Transfers are processed in real-time during banking hours.

Send a SPEI transfer
- **get_account_info**: Get your Nubank Mexico account profile
- **get_spending_analytics**: ), showing monthly trends, top merchants, and comparisons to previous periods. Use the period parameter for specific timeframes.

Get spending analytics and insights
- **get_account_balance**: Check your current account balance
- **get_credit_card_info**: Get your Nubank credit card details
- **get_investments**: View your Cajitas investment portfolio
- **get_credit_card_statement**: Defaults to the current open statement if no month is specified.

Get a credit card statement
- **get_transaction**: Get full details of a specific transaction
- **list_bills**: List pending bills and service payments
- **list_credit_card_transactions**: settled status.

List recent credit card transactions
- **list_rewards**: List your Nubank reward points and benefits
- **list_transactions**: Use limit and offset for pagination through large histories.

List recent account transactions
- **list_transfers**: List outgoing transfers
- **pay_bill**: If no amount is specified, the full outstanding amount is paid. Supports partial payments for eligible billers.

Pay a bill or service


## Installation & Usage

To install and use the **Nubank MX** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nubank-mx](https://vinkius.com/mcp/nubank-mx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
