# Stigg MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stigg)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/stigg-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/stigg-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate billing and subscription management via Stigg — provision customers, manage plans, and report usage directly from any AI agent.

## Description
Connect your **Stigg** account to any AI agent to take full control of your pricing and packaging workflows. Manage the entire customer lifecycle from provisioning to usage reporting through natural conversation.

### What you can do

- **Customer Lifecycle** — Create, update, and retrieve customer profiles using REST or GraphQL tools.
- **Subscription Management** — Provision new subscriptions, fetch active plan details, or cancel them when needed.
- **Usage Reporting** — Report metered feature usage in real-time to ensure accurate billing and entitlement enforcement.
- **Hybrid API Access** — Choose between REST and GraphQL actions for flexible integration with your billing data.

### How it works

1. Subscribe to this server
2. Enter your Stigg API Key
3. Start managing your SaaS billing from Claude, Cursor, or any MCP-compatible client

No more jumping between dashboards to check a customer's entitlement or manually reporting usage. Your AI acts as a billing operations assistant.

### Who is this for?

- **Product Managers** — instantly check customer plan statuses and feature entitlements without opening the Stigg console.
- **Customer Success** — provision trials or update customer details directly during support interactions.
- **Developers** — test billing flows and report usage for metered features straight from the terminal or IDE.


## Available Tools
- **rest_cancel_subscription**: Cancel a subscription via REST API
- **rest_create_customer**: Create a new customer via REST API
- **rest_create_subscription**: Create a subscription via REST API
- **rest_get_customer**: Retrieve a customer via REST API
- **rest_get_subscription**: Retrieve a subscription via REST API
- **gql_get_customer**: Get customer details via GraphQL
- **gql_get_entitlements_state**: Get entitlements state via GraphQL
- **gql_provision_customer**: Provision a customer and optional subscription via GraphQL
- **gql_provision_subscription**: Provision a subscription via GraphQL
- **gql_report_usage**: Report usage via GraphQL
- **rest_report_usage**: Report usage for metered features via REST API
- **rest_update_customer**: Update a customer via REST API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stigg** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a customer with ID 'cust_123', name 'Alice', and email 'alice@example.com' using REST."

**🤖 AI Agent:**
> I've successfully created the customer 'Alice' (ID: cust_123) in Stigg. Would you like to provision a subscription for them now?

---

**👤 You:**
> "Report 50 units of usage for feature 'api-calls' for customer 'cust_123'."

**🤖 AI Agent:**
> Usage reported. I've added 50 units to the 'api-calls' feature for customer 'cust_123' via the REST API.

---

**👤 You:**
> "Get the details for customer 'cust_123' using GraphQL."

**🤖 AI Agent:**
> Retrieving data... Customer 'Alice' (cust_123) is currently active with email 'alice@example.com'. I can also list their active subscriptions if you'd like.


## Installation & Usage

To install and use the **Stigg** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stigg](https://vinkius.com/mcp/stigg)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
