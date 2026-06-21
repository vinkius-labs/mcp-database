# Bold MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bold)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bold-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bold-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Automate payments via Bold Colombia — manage terminals, process transactions, generate payment links, and track settlements from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bold** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all the datáfono terminals connected to my Bold account."

**🤖 AI Agent:**
> I found 3 active terminals on your account: 'Smart Pro #BLD-4291' (online, last transaction 2 minutes ago), 'Smart Mini #BLD-7803' (online, idle), and 'Smart Pro #BLD-1156' (offline). Would you like to send a payment request to any of these terminals?

---

**👤 You:**
> "Create a payment link for 150,000 COP for the invoice #INV-2024-089."

**🤖 AI Agent:**
> Done! I've generated a payment link for $150,000 COP. The shareable URL is: https://checkout.bold.co/pay/abc123xyz. Share it with your client via WhatsApp, email, or SMS. The link expires in 24 hours.

---

**👤 You:**
> "List all transactions from the last 7 days and show me the total processed."

**🤖 AI Agent:**
> I queried your transactions from April 3 to April 10, 2026. You processed 47 transactions totaling $8,234,500 COP. 43 were approved (91.5%), 3 declined, and 1 refunded. The peak day was Friday with 12 transactions. Want me to break down by payment method?


## Installation & Usage

To install and use the **Bold** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bold](https://vinkius.com/mcp/bold)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
