# ChargeDesk MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chargedesk)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/chargedesk-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/chargedesk-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage billing and payments via ChargeDesk — track charges, refund payments, and manage customers across multiple gateways directly from any AI agent.

## Description
Connect your **ChargeDesk** account to any AI agent and take full control of your billing and payment operations across Stripe, PayPal, Braintree, and more through natural conversation. Streamline customer support and financial management.

### What you can do

- **Unified Payment Oversight** — List and retrieve details for charges across all connected payment gateways natively
- **Refund Management** — Process full or partial refunds for specific charges securely
- **Customer Intelligence** — Access and monitor customer profiles and their complete billing history flawlessly
- **Subscription Tracking** — List and retrieve details for active and inactive customer subscriptions securely
- **Gateway Auditing** — List all connected gateways and verify their operational status flawlessly
- **Notification Management** — Access and review configured webhooks and account alerts directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your ChargeDesk Secret Key (obtained from Account Settings -> API)
3. Start managing your billing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Customer Support Teams** — quickly look up payment history and process refunds using natural language
- **Finance Managers** — monitor revenue and transaction health without opening multiple gateway dashboards
- **Billing Administrators** — verify subscription statuses and customer details straight from their chat interface
- **Business Owners** — audit total charges and refund volumes across the entire business


## Available Tools
- **get_charge_details**: Get detailed information for a specific charge
- **get_customer_details**: Get detailed information for a specific customer
- **list_chargedesk_charges**: List recent charges from all gateways
- **list_chargedesk_customers**: List all customers in your account
- **list_connected_gateways**: List all connected payment gateways
- **list_chargedesk_subscriptions**: List active and inactive subscriptions
- **list_chargedesk_webhooks**: List configured webhooks
- **refund_chargedesk_payment**: Refund a specific charge


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ChargeDesk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the last 10 charges in ChargeDesk."

**🤖 AI Agent:**
> Retrieving recent charges... I found 10 items totaling $1,450.00. Most were via Stripe and PayPal. Would you like to see the customer details for any of these?

---

**👤 You:**
> "Refund $25.00 for charge ID 'ch_123456'."

**🤖 AI Agent:**
> Processing partial refund of $25.00 for ch_123456... The refund has been successfully initiated on the original gateway. The status in ChargeDesk is now 'Partially Refunded'.

---

**👤 You:**
> "List all my connected payment gateways."

**🤖 AI Agent:**
> Checking connected gateways... You have 3 active gateways: Stripe (Live), PayPal (Live), and Braintree (Sandbox). All are reporting a healthy connection.


## Installation & Usage

To install and use the **ChargeDesk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chargedesk](https://vinkius.com/mcp/chargedesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
