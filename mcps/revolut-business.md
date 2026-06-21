# Revolut Business MCP Server

Grant your AI access to Europe's powerhouse treasury. Automate multi-currency exchange, mass payouts and real-time vendor bulk-payments.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/revolut-business)

## Overview
**Category:** money-moves
**Tools Count:** 34

## Description
The **Revolut Business MCP Server** effectively bridges large-scale pan-European treasuries directly to Vinkius LLMs.

### What you can do

- **Automated Treasury Sweeps** — Ensure you're never short on balance. Query your global ledgers using `revolut_list_accounts` across EUR, GBP, USD layers simultaneously.
- **Algorithmic FX Execution** — Don't depend on manual banking schedules. Programmatically execute foreign-exchange limit orders utilizing `revolut_exchange_currency` swapping EUR/GBP dynamically.
- **Orchestrated Corporate Payouts** — Create target profiles (`revolut_add_counterparty`) and trigger payment queues securely using `revolut_create_draft_payment` directly across inter-banking networks.

### How it works

1. Login to your Revolut Business Web interface (B2B tier).
2. Generate standard API integration tokens.
3. Embed the raw key payload exclusively into your Vinkius parameter map to synchronize routing boundaries.

### Who is this for?

- **Global Talent Agencies** — Easily map contractor IDs to counterparties and fire cross-border payroll seamlessly.


## Available Tools
- **revolut_create_counterparty**: Required before making payments to a new recipient.

Add a new payment recipient (Counterparty)
- **revolut_create_exchange**: Settles immediately.

Execute an FX currency exchange between accounts
- **revolut_create_payment**: For payments requiring human approval, use revolut_create_draft_payment instead.

Make a direct payment to a counterparty
- **revolut_get_account**: Get details of a specific Revolut account
- **revolut_get_exchange_rate**: Optionally provide an amount to get the exact quoted conversion.

Get live FX exchange rates
- **revolut_get_transaction**: Get details of a specific transaction
- **revolut_list_accounts**: List all Revolut Business accounts and balances
- **revolut_list_counterparties**: List all saved payment recipients
- **revolut_list_team_members**: List all team members in the Revolut Business account
- **revolut_list_transactions**: Use for reconciliation, auditing, and financial reporting.

Retrieve historical transactions
- **revolut_cancel_payout_link**: Funds are returned to the source account.

Cancel an unclaimed payout link
- **revolut_create_draft_payment**: The draft appears in the Revolut Business app where an authorized team member must approve it. This is the safest way to handle payments via the API.

Create a payment draft for human approval
- **revolut_create_payout_link**: The recipient receives a URL to claim the funds without sharing their banking details. The link expires after a set period.

Create a payout link to send money
- **revolut_create_transfer**: Different from payments which go to external counterparties. Useful for moving money between currency pockets.

Transfer money between your own Revolut accounts
- **revolut_create_webhook**: Create a new webhook subscription
- **revolut_delete_counterparty**: Cannot be undone.

Remove a counterparty from the account
- **revolut_delete_draft_payment**: Cannot delete drafts already sent for approval.

Delete a payment draft
- **revolut_delete_webhook**: Events will no longer be delivered to this endpoint.

Delete a webhook subscription
- **revolut_get_account_bank_details**: Useful for sharing payment details with clients.

Get IBAN, BIC, and local bank details for a specific account
- **revolut_get_counterparty**: Get full details of a specific counterparty
- **revolut_get_draft_payment**: Get details of a specific payment draft
- **revolut_get_expense**: Get details of a specific expense
- **revolut_get_payout_link**: Get details of a specific payout link
- **revolut_get_team_member**: Get details of a specific team member
- **revolut_get_transfer_reasons**: Use this to get the valid codes before creating a transfer.

Get the list of valid transfer reason codes
- **revolut_get_webhook**: Get details of a specific webhook
- **revolut_get_webhook_failed_events**: Useful for debugging connectivity issues or missed notifications.

Get failed delivery events for a webhook
- **revolut_list_draft_payments**: Drafts require human approval in the Revolut Business app before funds are released.

List all pending payment drafts
- **revolut_list_expenses**: Use for accounts payable reconciliation and expense auditing. Note: not available in sandbox mode.

List all submitted expenses
- **revolut_list_payout_links**: Available in UK, EEA, AU, and SG.

List all payout links
- **revolut_list_roles**: List all available roles in the organisation
- **revolut_list_webhooks**: List all configured webhooks
- **revolut_rotate_webhook_secret**: The old secret is invalidated immediately.

Rotate the signing secret for a webhook
- **revolut_update_webhook**: Update a webhook configuration


## Installation & Usage

To install and use the **Revolut Business** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/revolut-business](https://vinkius.com/mcp/revolut-business)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
