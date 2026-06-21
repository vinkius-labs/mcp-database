# ChargeDesk MCP Server

Manage billing and payments via ChargeDesk — track charges, refund payments, and manage customers across multiple gateways directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/chargedesk)

## Overview
**Category:** customer-support
**Tools Count:** 8

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


## Installation & Usage

To install and use the **ChargeDesk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chargedesk](https://vinkius.com/mcp/chargedesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
