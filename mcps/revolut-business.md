# Revolut Business MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/revolut-business)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Grant your AI access to Europe's powerhouse treasury. Automate multi-currency exchange, mass payouts and real-time vendor bulk-payments.

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


## Available Tools (34)
- **revolut_cancel_payout_link**: Funds are returned to the source account.

Cancel an unclaimed payout link
- **revolut_create_draft_payment**: The draft appears in the Revolut Business app where an authorized team member must approve it. This is the safest way to handle payments via the API.

Create a payment draft for human approval
- **revolut_create_payment**: For payments requiring human approval, use revolut_create_draft_payment instead.

Make a direct payment to a counterparty
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
- **revolut_get_account**: Get details of a specific Revolut account
- **revolut_get_account_bank_details**: Useful for sharing payment details with clients.

Get IBAN, BIC, and local bank details for a specific account
- **revolut_get_counterparty**: Get full details of a specific counterparty
- **revolut_get_draft_payment**: Get details of a specific payment draft
- **revolut_get_exchange_rate**: Optionally provide an amount to get the exact quoted conversion.

Get live FX exchange rates
- **revolut_get_expense**: Get details of a specific expense
- **revolut_get_payout_link**: Get details of a specific payout link
- **revolut_get_team_member**: Get details of a specific team member
- **revolut_get_transaction**: Get details of a specific transaction
- **revolut_get_transfer_reasons**: Use this to get the valid codes before creating a transfer.

Get the list of valid transfer reason codes
- **revolut_get_webhook**: Get details of a specific webhook
- **revolut_get_webhook_failed_events**: Useful for debugging connectivity issues or missed notifications.

Get failed delivery events for a webhook
- **revolut_list_accounts**: List all Revolut Business accounts and balances
- **revolut_list_counterparties**: List all saved payment recipients
- **revolut_list_draft_payments**: Drafts require human approval in the Revolut Business app before funds are released.

List all pending payment drafts
- **revolut_list_expenses**: Use for accounts payable reconciliation and expense auditing. Note: not available in sandbox mode.

List all submitted expenses
- **revolut_list_payout_links**: Available in UK, EEA, AU, and SG.

List all payout links
- **revolut_list_roles**: List all available roles in the organisation
- **revolut_list_team_members**: List all team members in the Revolut Business account
- **revolut_list_transactions**: Use for reconciliation, auditing, and financial reporting.

Retrieve historical transactions
- **revolut_list_webhooks**: List all configured webhooks
- **revolut_rotate_webhook_secret**: The old secret is invalidated immediately.

Rotate the signing secret for a webhook
- **revolut_update_webhook**: Update a webhook configuration
- **revolut_create_counterparty**: Required before making payments to a new recipient.

Add a new payment recipient (Counterparty)
- **revolut_create_exchange**: Settles immediately.

Execute an FX currency exchange between accounts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Revolut Business** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Review our Treasury balances. Scan all underlying operational wallets across Revolut right now."

**🤖 AI Agent:**
> Treasury check complete. Sweeping operational limits... We observed approximately 5 Active Wallet domains. Your USD pool registers at $14,000 liquid, while GBP rests at 50,000. No un-settled constraints present.

---

**👤 You:**
> "It looks like we are short on GBP for office supplies. Please buy 500 GBP using our primary Euro reserve wallet ID natively."

**🤖 AI Agent:**
> Foreign Exchange executed! We successfully transferred the structural value. Live rates computed perfectly moving out nominal assets towards GBP. You should observe balances refilled instantly.

---

**👤 You:**
> "Map a new Counterparty Profile under 'AWS Services'."

**🤖 AI Agent:**
> Completed profile injection! 'AWS Services' is now established within your internal directory and readily accepts mass payouts.


## ❓ FAQ

**Q: Will an AI mistake drain our corporate funds globally?**
Fortunately, the Revolut API restricts direct instantaneous payouts primarily via Drafts. If you trigger `revolut_create_draft_payment`, the LLM compiles and packages up perfectly formatted vendor-payments pushing them into your queue. A Human Finance Administrator generally just presses 'Approve' inside their Revolut Business app. Total isolation of power.

**Q: Can I convert currencies with the robot?**
Yes! Revolut Business is famous for inter-banking rates. Use the `revolut_exchange_currency` tool dictating you wish to move 5,000 USD to your GBP corporate holding account. Instantly, the system executes an institutional-tier forex buy sequence under the hood settling immediately.

**Q: How do I access full transaction histories?**
The tool `revolut_get_transactions` hooks straight into Revolut's raw global event log, feeding exactly dates, references, and amounts for AI auditing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/revolut-business](https://vinkius.com/mcp/revolut-business)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Revolut Business** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `revolut-business` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Revolut Business** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "revolut-business": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
