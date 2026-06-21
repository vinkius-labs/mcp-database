# Chargebee MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chargebee-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/chargebee-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/chargebee-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage recurring subscriptions, automate billing cycles, and reduce churn with revenue operations built for SaaS growth.

## Description
Connect your **Chargebee** site to any AI agent and take full control of your billing workflows through natural conversation.

### What you can do

- **Subscription Lifecycle** — List active, trialing, or cancelled subscriptions and inspect their metadata
- **Customer Management** — Query profiles, billing info, and contact details for any customer in your database
- **Invoicing & Payments** — Track paid, pending, and overdue invoices to stay on top of your revenue
- **Product Catalog** — List available plans and addons to understand your current offerings
- **Actionable Workflows** — Create customers, start new subscriptions, or cancel existing ones programmatically

### How it works

1. Subscribe to this server
2. Enter your Chargebee Site name and API Key
3. Start managing your recurring revenue from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **cancel_subscription**: Cancel an existing subscription
- **create_customer**: Create a new customer profile
- **create_subscription**: Create a new subscription for a customer
- **get_customer**: Get details for a specific customer
- **get_subscription**: Get details for a specific subscription
- **list_addons**: List available product addons
- **list_customers**: List Chargebee customers
- **list_invoices**: Can be filtered by status or customer.

List Chargebee invoices
- **list_plans**: List available product plans
- **list_subscriptions**: Supports filtering via optional parameters.

List Chargebee subscriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chargebee** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active subscriptions in Chargebee."

**🤖 AI Agent:**
> I've fetched the subscriptions. You have 12 active subscriptions, including 'sub_123' (Premium Plan) and 'sub_456' (Standard Plan).

---

**👤 You:**
> "Show me details for customer 'cust_789'."

**🤖 AI Agent:**
> Customer 'cust_789' is John Doe (john@example.com), based in New York. They have an active payment source on file.

---

**👤 You:**
> "Find all overdue invoices."

**🤖 AI Agent:**
> I've analyzed your invoices. There are currently 3 overdue invoices totaling $450. Would you like the list of customer IDs for these invoices?


## Installation & Usage

To install and use the **Chargebee** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chargebee-alternative](https://vinkius.com/mcp/chargebee-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
