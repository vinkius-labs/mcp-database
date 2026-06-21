# Stigg MCP Server

Automate billing and subscription management via Stigg — provision customers, manage plans, and report usage directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/stigg)

## Overview
**Category:** developer-tools
**Tools Count:** 12

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


## Installation & Usage

To install and use the **Stigg** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stigg](https://vinkius.com/mcp/stigg)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
