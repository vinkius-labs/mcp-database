# Nubank MX MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nubank-mx)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nubank-mx-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nubank-mx-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Nubank Mexico banking from any AI agent — check balances, review transactions, send SPEI transfers, pay bills, and track spending analytics.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nubank MX** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much do I have in my Nubank account right now?"

**🤖 AI Agent:**
> Your Nubank Cuenta balance is $47,832.50 MXN. You have $2,150 MXN in pending transactions. Your available balance is $45,682.50 MXN. Your deposits are currently earning 15.0% annual yield (rendimiento). Your CLABE for receiving transfers is: 638180000012345678.

---

**👤 You:**
> "Send $5,000 MXN via SPEI to CLABE 012180001234567890 with concept 'Renta abril'."

**🤖 AI Agent:**
> SPEI transfer sent successfully! $5,000.00 MXN transferred to CLABE 012180001234567890 (BBVA Mexico). Concept: 'Renta abril'. Tracking number (clave de rastreo): 2026041000000012345678. Your new available balance is $40,682.50 MXN.

---

**👤 You:**
> "Show me my spending breakdown for last month."

**🤖 AI Agent:**
> Your spending last month totaled $28,450 MXN across 67 transactions. Top categories: 🍔 Food & Dining: $8,200 (29%) — top merchant: Uber Eats. 🚗 Transportation: $4,500 (16%) — top: Uber rides. 🏠 Housing: $5,000 (18%) — rent payment. 🛒 Shopping: $3,850 (14%). 🎮 Entertainment: $2,100 (7%). Compared to the previous month, you spent 12% more on dining. Would you like detailed insights on any category?


## Installation & Usage

To install and use the **Nubank MX** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nubank-mx](https://vinkius.com/mcp/nubank-mx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
