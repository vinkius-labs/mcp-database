# Orb MCP Server

Automate usage-based billing via Orb — ingest events, manage subscriptions, and track invoices directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/orb)

## Overview
**Category:** data-management
**Tools Count:** 10

## Description
Connect your **Orb** account to any AI agent to streamline your revenue operations and usage-based billing workflows through natural language.

### What you can do

- **Usage Ingestion** — Send batches of usage events with idempotency keys to track consumption in real-time.
- **Subscription Lifecycle** — Create, update, and cancel subscriptions, tying customers to specific billing plans seamlessly.
- **Customer Management** — Provision new customers and list existing ones with full metadata and external ID mapping.
- **Invoicing & Revenue** — List historical invoices or fetch upcoming draft invoices to predict end-of-month billing.
- **Credit Ledgers** — Manage prepaid credits by creating ledger entries for increments, decrements, or expirations.

### How it works

1. Subscribe to this server
2. Enter your Orb API Key
3. Start managing your billing and usage data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance & RevOps** — Instantly check upcoming revenue and manage customer credits without manual dashboard exports.
- **Engineering Teams** — Debug usage ingestion and verify event delivery directly from the terminal or IDE.
- **Product Managers** — Monitor feature adoption and subscription statuses across the customer base.


## Available Tools
- **cancel_subscription**: Cancel a subscription
- **create_customer**: Requires name and email.

Create a new customer in Orb
- **create_ledger_entry**: Create a ledger entry for credits
- **create_subscription**: Create a subscription for a customer
- **fetch_ledger**: Fetch credit ledger for a customer
- **get_upcoming_invoice**: Fetch upcoming invoice for a subscription
- **ingest_events**: Events require customer_id, event_name, timestamp, idempotency_key, and properties.

Ingest usage events into Orb
- **list_customers**: List customers in Orb
- **list_invoices**: List invoices
- **update_subscription**: Update an existing subscription


## Installation & Usage

To install and use the **Orb** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/orb](https://vinkius.com/mcp/orb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
