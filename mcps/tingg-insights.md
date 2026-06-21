# Tingg Insights MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tingg-insights)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tingg-insights-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tingg-insights-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze mobile payment and fintech data across African markets with insights that reveal transaction trends and user behavior.

## Description
Connect your **Tingg (Cellulant)** payments account to any AI agent and simplify how you collect payments, manage disbursements, and track financial settlements across Africa through natural conversation.

### What you can do

- **Transaction Oversight** — List and search all payment transactions and retrieve real-time status for specific checkout requests.
- **Disbursement Control** — Initiate and monitor payouts (B2C/B2B) to recipients across supported mobile money and bank channels.
- **Settlement Tracking** — List bank settlements to monitor when funds are moved from your Tingg account to your local bank.
- **Payment Initiation** — Programmatically create new checkout requests to collect payments via mobile money, card, or bank.
- **Engagement Automation** — Send transactional SMS or Email notifications to users via the Tingg Engage service.
- **Performance Metrics** — Retrieve high-level account metrics and payment success rates to monitor your business health.

### How it works

1. Subscribe to this server
2. Enter your Tingg Client ID and Client Secret (found in your merchant portal)
3. Start managing your African payment ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **Finance & Operations Managers** — quickly check transaction statuses and verify bank settlements via simple AI commands.
- **E-commerce & Business Owners** — monitor payout progress and retrieve account performance metrics directly from the workspace.
- **Product Teams** — automate payment requests and trigger user notifications via the AI assistant.


## Available Tools
- **check_api_health**: Verify Tingg API connectivity
- **create_checkout_request**: Initiate a new payment request
- **get_account_performance_metrics**: Retrieve performance stats
- **get_payout_status**: Check status of a payout
- **get_transaction_status**: Check status of a specific transaction
- **initiate_payout_request**: Send money to a recipient
- **list_disbursement_payouts**: List all payouts/disbursements
- **list_account_settlements**: List bank settlements
- **list_payment_transactions**: List recent payment transactions
- **list_configured_webhooks**: List active webhooks
- **send_engagement_notification**: Send SMS or Email alert
- **initiate_payment_refund**: Request a refund


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tingg Insights** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 payment transactions in my Tingg account."

**🤖 AI Agent:**
> I've retrieved your recent transactions. You have 5 checkout requests including #TX-8823 (Success), #TX-8824 (Pending), and #TX-8825 (Failed). Would you like real-time status for the pending request?

---

**👤 You:**
> "Show me my account performance metrics."

**🤖 AI Agent:**
> Fetching performance stats... Your account shows a 94% payment success rate over the last 30 days. Total volume processed is $12,500 across mobile money and card channels. Shall I break this down by country?

---

**👤 You:**
> "Check the status of payout 'payout_10293'."

**🤖 AI Agent:**
> Retrieving payout info... Payout payout_10293 is currently 'Processed Successfully'. The funds have been sent to the recipient's mobile money wallet. Is there anything else you'd like to track?


## Installation & Usage

To install and use the **Tingg Insights** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tingg-insights](https://vinkius.com/mcp/tingg-insights)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
