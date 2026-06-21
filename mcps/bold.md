# Bold MCP Server

Automate payments via Bold Colombia — manage terminals, process transactions, generate payment links, and track settlements from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/bold)

## Overview
**Category:** money-moves
**Tools Count:** 14

## Description
Connect your **Bold** merchant account to any AI agent and gain full control of your Colombian payment infrastructure through natural conversation.

### What you can do

- **Terminal Management** — List all bound datáfono devices (Smart Pro, Smart Mini) and trigger in-store payment flows remotely
- **Online Payments** — Process card-not-present payments, create shareable payment links, and manage the full transaction lifecycle
- **Transaction Intelligence** — Query historical transactions by date range, inspect individual payment details including card brand and settlement data
- **Refund Operations** — Issue full reversals on approved online payments back to the original payment method
- **Webhook Configuration** — Register and manage real-time HTTPS endpoints for transaction event notifications
- **Balance Monitoring** — Check your merchant account balance including available funds and pending disbursements

### How it works

1. Subscribe to this server
2. Enter your Bold API Key and Secret Key
3. Start managing payments from Claude, Cursor, or any MCP-compatible client

Your AI becomes a dedicated payment operations assistant, eliminating context switching between the Bold dashboard and your day-to-day workflow.

### Who is this for?

- **E-commerce Operators** — automate payment link creation and monitor transaction status without leaving your workspace
- **Retail Managers** — remotely trigger POS terminal payments and track daily sales from conversations
- **Finance Teams** — query settlement reports and refund histories programmatically for reconciliation


## Available Tools
- **create_online_payment**: Requires card tokenization details, the amount in COP, and payer information for Colombian anti-fraud compliance.

Process an online card payment
- **create_payment_link**: The link includes the specified amount in Colombian Pesos (COP) and a reference description.

Generate a shareable payment link
- **create_webhook**: ) in your Bold merchant account.

Register a new webhook endpoint
- **delete_webhook**: Remove a webhook endpoint
- **get_account_balance**: Get current merchant account balance
- **get_online_payment**: Get details of an online payment
- **get_payment_link**: Get details of a specific payment link
- **get_transaction**: Get details of a specific transaction
- **initiate_terminal_payment**: This requires the terminal serial number and the payment amount in COP.

Trigger a payment on a physical terminal
- **list_payment_methods**: List accepted payment methods
- **list_terminals**: ) currently linked to your Bold merchant account, including their serial numbers and connectivity status.

List all bound payment terminals
- **list_transactions**: List recent payment transactions
- **list_webhooks**: List configured webhooks
- **refund_payment**: The refund is processed back to the original payment method and may take 5-10 business days to reflect on the cardholder's statement.

Issue a refund for a processed payment


## Installation & Usage

To install and use the **Bold** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bold](https://vinkius.com/mcp/bold)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
