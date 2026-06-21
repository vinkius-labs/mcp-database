# GoCardless MCP Server

Manage direct debit payments, track mandates, and oversee customers via AI agents with GoCardless.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gocardless)

## Overview
**Category:** money-moves
**Tools Count:** 12

## Description
Connect your **GoCardless** merchant account to any AI agent to automate your direct debit payments and customer mandates through the Model Context Protocol (MCP). GoCardless is the global leader in bank-to-bank payments, simplifying the collection of recurring and one-off payments. This MCP server enables you to retrieve customer records, track mandate authorizations, manage payment collections, and monitor bank payouts directly through natural conversation.

### Key Features

- **Customer & Bank Oversight** — List all customers registered in your system and fetch detailed profile and bank account metadata instantly.
- **Mandate Management** — Access and track customer authorizations (mandates) to ensure you have the legal right to collect payments.
- **Payment Orchestration** — List all direct debit collections, track their status (confirmed, failed), and programmatically initiate new payments against active mandates.
- **Subscription Insights** — Retrieve active and inactive recurring payment plans to understand your predictable revenue health.
- **Payout Tracking** — Access a complete list of funds being sent from GoCardless to your own bank account for easy reconciliation.
- **Refund Visibility** — Monitor processed refunds and reversed payments to maintain an accurate financial audit trail.
- **Real-time Synchronization** — Keep your bank-to-bank payment data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your GoCardless Access Token (found in Developers > Access Tokens)
3. Start managing your direct debits from Claude, Cursor, or any MCP client

### Who is this for?

- **Finance & Billing Ops** — quickly check if a mandate is active or verify if a payout has been initiated without manual portal navigation.
- **Account Managers** — get a real-time overview of a customer's payment history and subscription status via simple AI commands.
- **Operations Leads** — automate the retrieval of failed payment logs and mandate status reports seamlessly.


## Available Tools
- **verify_api_connection**: Check connection
- **create_new_payment**: Initiate a collection
- **get_account_details**: Get account identity
- **get_customer_details**: Get customer metadata
- **get_mandate_status**: Check mandate details
- **get_payment_details**: Get payment metadata
- **list_payment_customers**: List all customers
- **list_payment_mandates**: List active mandates
- **list_direct_debit_payments**: List all payments
- **list_merchant_payouts**: List bank payouts
- **list_payment_refunds**: List reversed payments
- **list_recurring_subscriptions**: List recurring plans


## Installation & Usage

To install and use the **GoCardless** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gocardless](https://vinkius.com/mcp/gocardless)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
