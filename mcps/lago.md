# Lago MCP Server

Manage your metering and usage-based billing with Lago — handle customers, subscriptions, plans, and events directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/lago)

## Overview
**Category:** money-moves
**Tools Count:** 12

## Description
Connect **Lago** to your AI agent to automate your metering and billing infrastructure. Lago is the open-source alternative to Stripe Billing, designed for complex usage-based pricing models.

### What you can do

- **Customer Management** — Create and update customer profiles with `upsert_customer` and retrieve details with `get_customer`.
- **Subscription Lifecycle** — Assign plans to customers using `create_subscription` and monitor them with `get_subscription`.
- **Billing Infrastructure** — Define billing plans with `create_plan` and set up `create_billable_metric` to track consumption.
- **Usage Tracking** — Send real-time usage data with `send_event` or `batch_events` to trigger accurate billing.
- **Financial Operations** — Manage wallets, apply coupons, and list invoices to keep your revenue operations running smoothly.

### How it works

1. Subscribe to this server
2. Enter your Lago API Key
3. Start managing your billing logic from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SaaS Founders** — quickly check customer subscription status or update plans without leaving the chat.
- **Growth Engineers** — automate the creation of coupons and wallets for promotional campaigns.
- **Finance Teams** — list invoices and verify billable metrics through natural language queries.


## Available Tools
- **apply_coupon**: Apply a coupon to a customer
- **batch_events**: Send a batch of usage events
- **create_billable_metric**: Create a billable metric
- **create_coupon**: Create a coupon
- **create_plan**: Create a new billing plan
- **create_subscription**: Assign a plan to a customer (create subscription)
- **create_wallet**: Create a wallet for prepaid credits
- **get_customer**: Retrieve a customer by external ID
- **get_subscription**: Retrieve a subscription by external ID
- **list_invoices**: List all invoices
- **send_event**: Send a usage event
- **upsert_customer**: Requires an external_id.

Create or update a customer in Lago


## Installation & Usage

To install and use the **Lago** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lago](https://vinkius.com/mcp/lago)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
