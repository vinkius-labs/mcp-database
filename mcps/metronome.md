# Metronome MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/metronome)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/metronome-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/metronome-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Automate usage-based billing via Metronome — ingest events, query usage data, and manage customer contracts directly from any AI agent.

## Description
Connect your **Metronome** account to any AI agent to streamline your usage-based billing and revenue operations through natural conversation.

### What you can do

- **Usage Ingestion & Querying** — Send usage events and retrieve aggregated usage data across customers and metrics using `ingest_events` and `get_usage`.
- **Customer Management** — Create, list, and archive customers, or manage their billing configurations via `list_customers` and `create_customer`.
- **Billing & Invoicing** — Fetch, void, or regenerate invoices and track net balances with `list_invoices` and `get_net_balance`.
- **Contract Lifecycle** — Create and edit contracts, manage rate cards, and track commits using `create_contract` and `list_contracts`.
- **Alerts & Monitoring** — Set up notifications, alerts, and access audit logs for billing transparency.

### How it works

1. Subscribe to this server
2. Enter your Metronome API Token
3. Start managing your billing operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance Teams** — reconcile usage data and manage invoices without manual exports.
- **Product Managers** — analyze feature usage and billing impact in real-time.
- **Engineering Teams** — verify event ingestion and monitor billing services directly from the terminal.


## Available Tools
- **add_custom_field_key**: Create a custom field key
- **add_rate**: Add a rate to a rate card
- **archive_customer**: Voids invoices and archives contracts.

Archive a customer
- **create_alert**: Create a threshold notification alert
- **create_billable_metric**: Create a billable metric
- **create_commit**: Create a commit
- **create_contract**: Create a contract
- **create_customer**: Create a new customer
- **create_notification**: Create an offset lifecycle event notification
- **create_product**: Products can be USAGE, FIXED, COMPOSITE, or SUBSCRIPTION.

Create a product
- **create_rate_card**: Defines base prices for products.

Create a rate card
- **edit_contract**: ).

Edit a contract
- **get_audit_logs**: Get audit logs
- **get_customer**: Get a specific customer
- **get_invoice**: Get an invoice
- **get_net_balance**: Get net balance
- **get_services**: Get services
- **get_usage_groups**: Get usage data with paginated groupings
- **get_usage**: Get batched usage data
- **ingest_events**: Supports up to 100,000 events per second.

Ingest usage events into Metronome
- **list_balances**: List balances
- **list_billable_metrics**: List all billable metrics
- **list_contracts**: List customer contracts
- **list_credit_types**: List pricing units
- **list_customers**: Supports filtering.

List all customers
- **list_invoices**: List invoices
- **list_products**: List products
- **regenerate_invoice**: Regenerate an invoice
- **search_events**: Designed for sampling-based testing.

Search events by transaction ID
- **set_custom_field_values**: Set custom field values
- **void_invoice**: Void an invoice


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Metronome** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all customers currently registered in Metronome."

**🤖 AI Agent:**
> I've retrieved the customer list. You have 15 active customers, including 'Acme Corp' (ID: cust_821) and 'GlobalTech' (ID: cust_442). Would you like more details on a specific one?

---

**👤 You:**
> "Show me the usage data for customer cust_821 for the last 30 days."

**🤖 AI Agent:**
> Fetching usage data... For 'Acme Corp', I see 1.2M events ingested across 3 billable metrics. The primary driver is 'API Requests' with 950k units. Would you like to see the breakdown by day?

---

**👤 You:**
> "Retrieve the details and status for invoice inv_556677."

**🤖 AI Agent:**
> Invoice inv_556677 for 'GlobalTech' is currently 'Finalized' with a total amount of $4,250.00. It covers the period from Oct 1 to Oct 31. Would you like me to list the line items?


## Installation & Usage

To install and use the **Metronome** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/metronome](https://vinkius.com/mcp/metronome)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
