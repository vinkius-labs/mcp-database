# Orb MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/orb)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/orb-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/orb-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Automate usage-based billing via Orb — ingest events, manage subscriptions, and track invoices directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Orb** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 customers created in Orb."

**🤖 AI Agent:**
> I've retrieved the latest customers. The most recent entries include 'Acme Corp' (ID: cust_821), 'Global Tech' (ID: cust_932), and 'Starlight Inc' (ID: cust_104). Would you like to see the subscription details for any of them?

---

**👤 You:**
> "Ingest a usage event for customer cust_123: 50 units of 'api_requests'."

**🤖 AI Agent:**
> Usage event successfully ingested for 'cust_123'. I've used a unique idempotency key for this batch to ensure accurate tracking. The 50 units of 'api_requests' are now reflected in their usage metrics.

---

**👤 You:**
> "What is the upcoming invoice amount for subscription sub_987?"

**🤖 AI Agent:**
> The upcoming draft invoice for subscription `sub_987` is currently at $450.00. This includes the base plan fee plus $120.00 in metered usage accrued during the current period.


## Installation & Usage

To install and use the **Orb** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/orb](https://vinkius.com/mcp/orb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
