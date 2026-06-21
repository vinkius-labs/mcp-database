# Togai (Usage Metering & Pricing) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/togai-usage-metering-pricing)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/togai-usage-metering-pricing-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/togai-usage-metering-pricing-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate usage-based billing and metering — ingest events, manage customers, and track entitlements directly from your AI agent.

## Description
Connect **Togai** to any AI agent to orchestrate complex usage-based pricing models and real-time metering through natural conversation.

### What you can do

- **Event Ingestion** — Push raw usage data using `ingest_event` or `ingest_batch_events` to track product consumption in real-time.
- **Customer & Account Management** — Create and update legal entities and billing accounts with `create_customer` and `create_account`.
- **Usage Metering** — Define how raw events transform into billable units using `create_usage_meter`.
- **Billing & Credits** — Monitor financial health with `list_invoices`, `get_wallet_balance`, and `grant_credit`.
- **Entitlements** — Check feature access and limits instantly using `check_entitlement` or `get_entitlements`.

### How it works

1. Subscribe to this server
2. Enter your Togai API Key
3. Start managing your revenue operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **FinOps & RevOps** — Monitor usage patterns, check invoice statuses, and manage credits without leaving your workflow.
- **Product Managers** — Verify customer entitlements and usage metrics to make data-driven pricing decisions.
- **Developers** — Test event ingestion and verify metering logic directly from the code editor.


## Available Tools
- **check_entitlement**: Check entitlement for a specific feature
- **create_account**: Create a new account
- **create_customer**: Create a new customer
- **create_price_plan**: Create a price plan (V2)
- **create_usage_meter**: Requires type, aggregation, and computations.

Create a usage meter
- **get_account**: Get details for a specific account
- **get_customer**: Get details for a specific customer
- **get_entitlements**: Get entitlements for an account
- **get_metrics**: Get aggregated metrics
- **get_wallet_balance**: Get wallet balance for an account
- **grant_credit**: Grant credits to an account
- **ingest_batch_events**: Ingest a batch of usage events
- **ingest_event**: Requires an event object with schemaName, timestamp, accountId, id, attributes, and dimensions.

Ingest a single usage event
- **list_accounts**: List all accounts
- **list_customers**: List all customers
- **list_invoices**: List invoices with optional filters
- **list_rate_cards**: List rate cards for a price plan
- **update_account**: Update an existing account
- **update_customer**: Update an existing customer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Togai (Usage Metering & Pricing)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first 10 customers in my Togai account."

**🤖 AI Agent:**
> I've retrieved your customer list. You have customers like 'Acme Corp' (ID: cust_123) and 'Globex' (ID: cust_456). Would you like to see details for any of them?

---

**👤 You:**
> "Ingest a usage event for account 'acc_vink_01' with 50 units of 'api_requests'."

**🤖 AI Agent:**
> Successfully ingested the event to Togai. The usage has been recorded for account 'acc_vink_01' under the 'api_requests' schema.

---

**👤 You:**
> "What is the current wallet balance for account 'acc_987'?"

**🤖 AI Agent:**
> The account 'acc_987' currently has a balance of $150.00 available in their wallet.


## Installation & Usage

To install and use the **Togai (Usage Metering & Pricing)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/togai-usage-metering-pricing](https://vinkius.com/mcp/togai-usage-metering-pricing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
