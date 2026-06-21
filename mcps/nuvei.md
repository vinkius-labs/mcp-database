# Nuvei MCP Server

Connect your AI agent to Nuvei to track transactions, manage payments, and securely tokenize cards through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/nuvei)

## Overview
**Category:** money-moves
**Tools Count:** 10

## Description
Connect your **Nuvei** merchant account to your AI agent and manage your global payments platform effortlessly.

### What you can do

- **Payment Processing** — Programmatically invoke the `create_payment` endpoint to handle live orders directly from your chat or workflows.
- **Transaction Auditing** — Query specific payments using `get_payment` or list multiple transactions with `get_transactions` to track settlements and statuses.
- **Card Vaulting & Tokenization** — Securely invoke `create_card_token` without touching raw card data, pushing tokens directly to Nuvei's vault.
- **Token Retrieval** — Look up vaulted payment methods using `get_token` to analyze returning customers or manage subscriptions.

### How it works

1. Subscribe to this server
2. Enter your Nuvei API Credentials and Merchant details
3. Start fetching transaction summaries and creating payments directly from Claude, Cursor, or any AI client

### Who is this for?

- **Finance Teams** — seamlessly fetch daily transaction batches or audit failed payments to reconcile accounting without opening the Nuvei Control Panel.
- **Customer Support** — quickly locate single transactions and verify successful payments for complaining users directly in the CRM workflow.
- **E-commerce Engineers** — tokenize payments and simulate order testing securely without leaving the code editor.


## Available Tools
- **capture_payment**: If amount is omitted, captures the full authorized total.

Capture a previously authorized card payment
- **create_payment**: This initiates a real money authorization/charge network request. Returns the Nuvei transaction ID and status.

Initialize a new payment intent with Nuvei
- **create_card_token**: Tokenize plain card details into a vaulted payment token
- **delete_token**: Stops future recurring charges or 1-click purchases immediately.

Delete a vaulted payment token permanently
- **get_payment**: Essential for checking if an async payment cleared.

Retrieve the current status mapped to a Nuvei Payment ID
- **get_token**: View details of a previously vaulted Nuvei Card/Payment Token
- **get_transactions**: List or enumerate historical transaction records
- **refund_payment**: Supports partial amounts.

Refund a fully captured Nuvei payment
- **update_token**: g. updating an expiry date string) without needing full card details again.

Mutate specific fields inside a vaulted token
- **void_payment**: Note: Can only void pending auths.

Cancel a pending authorized payment preventing capture


## Installation & Usage

To install and use the **Nuvei** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nuvei](https://vinkius.com/mcp/nuvei)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
