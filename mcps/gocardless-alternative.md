# GoCardless MCP Server

Collect recurring payments directly from bank accounts with automated direct debit that reduces failed payment rates.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gocardless-alternative)

## Overview
**Category:** money-moves
**Tools Count:** 12

## Description
Connect your **GoCardless** account to any AI agent and take full control of your Direct Debit collections and recurring billing workflows through natural conversation.

### What you can do

- **Customer Orchestration** — List and manage bank payers programmatically, including contact info and payment history retrieval
- **Mandate Management** — Monitor and retrieve detailed status for customer payment authorizations to ensure collection reliability
- **Payment Automation** — Trigger one-off bank debit collections or manage complex recurring subscription plans directly through your agent
- **Financial Visibility** — Access payout creditor details and monitor system events to maintain high-fidelity oversight of your cash flow
- **Operations Control** — Programmatically cancel pending payments and check individual transaction states (confirmed, failed) in real-time

### How it works

1. Subscribe to this server
2. Retrieve your **Access Token** from GoCardless (Developers > Create > Access Token)
3. Specify your environment (live or sandbox) in the configuration
4. Start managing your bank payments from Claude, Cursor, or any MCP client

No more manual payment tracking or digging through bank files. Your AI acts as your dedicated payment operations assistant.

### Who is this for?

- **Finance Teams** — instantly check payment statuses and reconcile payouts using natural language
- **Billing Managers** — automate customer creation and mandate verification without leaving your workspace
- **SaaS Founders** — monitor subscription health and manage failed payments through automated queries


## Available Tools
- **stop_pending_payment**: Cancel payment
- **create_new_customer**: Add payer to account
- **collect_payment**: Trigger new payment
- **get_customer_details**: Get payer info
- **get_mandate_details**: Get authorization info
- **get_payment_status**: Check transaction state
- **list_account_creditors**: List payout recipients
- **list_customers**: List bank payers
- **list_system_events**: Get activity log
- **list_active_mandates**: List payment authorizations
- **list_payment_history**: List all transactions
- **list_recurring_payments**: List all subscriptions


## Installation & Usage

To install and use the **GoCardless** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gocardless-alternative](https://vinkius.com/mcp/gocardless-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
