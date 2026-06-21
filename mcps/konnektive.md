# Konnektive MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/konnektive)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/konnektive-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/konnektive-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage CRM and billing — list orders, query customers, and audit transactions.

## Description
Connect your AI agent to **Konnektive CRM** to automate and streamline your e-commerce operations.

### Core Capabilities

- **Order Management** — Query and retrieve detailed information about customer orders including shipping and billing data
- **Customer CRM Access** — Search and audit customer profiles directly from your chat client
- **Transaction Auditing** — Track and verify payment transactions across your integrated gateways
- **Product & Campaign Insights** — List available products and active marketing campaigns to inform your strategy
- **Administrative Actions** — Update order shipping addresses and monitor system audit logs

### Setup Requirements

1. Subscribe to this server
2. Obtain your **API Login ID** and **API Password** from the Konnektive dashboard (API settings)
3. Start managing your e-commerce data via natural language


## Available Tools
- **query_konnektive_orders**: Provide filters as a JSON string.

Search for orders in Konnektive
- **get_order_details**: Get details for a specific order
- **query_konnektive_customers**: Provide filters as a JSON string.

Search for customers
- **get_customer_details**: Get details for a specific customer
- **query_konnektive_transactions**: Provide filters as a JSON string.

Search for payment transactions
- **list_billing_campaigns**: List all campaigns
- **list_konnektive_products**: List all products
- **update_order_shipping_address**: Provide address as a JSON string.

Update the shipping address for an order
- **list_fulfillment_houses**: List fulfillment centers
- **get_konnektive_audit_logs**: Provide filters as a JSON string.

Retrieve system audit logs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Konnektive** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all orders from yesterday"

**🤖 AI Agent:**
> Searching Konnektive for orders placed yesterday… I've found 150 orders. Total revenue: $4,500. 120 are 'Shipped', 30 are 'Pending'. Would you like to see the pending ones?

---

**👤 You:**
> "Show details for order 'ORD-12345'"

**🤖 AI Agent:**
> Retrieved order 'ORD-12345'. Customer: John Doe. Items: 2x 'Premium Supplement'. Status: Shipped via FedEx. Shipping to: 123 Main St, NY. Would you like to track the package?

---

**👤 You:**
> "Find customer with email 'jane@example.com'"

**🤖 AI Agent:**
> Searching CRM… Found Jane Smith (ID: 98765). She has placed 3 orders in the last 6 months with a total value of $250. Current status is 'Active'.


## Installation & Usage

To install and use the **Konnektive** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/konnektive](https://vinkius.com/mcp/konnektive)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
