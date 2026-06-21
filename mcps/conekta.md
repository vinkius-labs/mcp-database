# Conekta MCP Server

Equip your AI agent to securely manage Latin American payments, view transactions, and track sales using the Conekta API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/conekta)

## Overview
**Category:** money-moves
**Tools Count:** 8

## Description
Integrate your AI assistant with **Conekta**, the leading online payment gateway in Mexico and Latin America. By providing seamless connectivity to your Conekta account, your conversational agent can instantly analyze transaction data, verify specific charges, and keep track of your core e-commerce metrics directly through natural language requests.

### What you can do

- **Transaction Lookups** — Instantly query the status of specific payments by providing a transaction ID or customer email.
- **Sales Analysis** — Ask for summaries of recent successful transactions, refunds, or chargebacks to keep track of store performance.
- **Customer Management** — Retrieve and review customer profiles and their associated payment history to provide faster support.

### How it works

1. Add the Conekta integration to your AI workspace.
2. Secure the connection using your Conekta Private API Key.
3. Chat seamlessly with your agent to pull transaction records, summarize daily sales, and more—without navigating complex dashboards.

### Who is this for?

- **E-commerce Managers** — Rapidly check if a customer's payment has cleared without needing to access the main billing platform.
- **Customer Support Teams** — Instantly verify refund requests and transaction details directly while assisting users.
- **Financial Analysts** — Quickly gather aggregate data on daily revenue, chargebacks, and successful orders.


## Available Tools
- **create_order**: Requires customer name, email, phone, and at least one line item with name, unit_price (in cents), and quantity. Currency defaults to MXN.

Create a new order in Conekta
- **get_customer**: Returns contact info, payment sources, and order history.

Retrieve detailed information about a specific customer
- **get_order**: Returns charges, line items, customer info, and payment status.

Retrieve detailed information about a specific order
- **list_customers**: Retrieve a list of customer records from Conekta
- **list_events**: Useful for debugging integrations.

Retrieve a list of API events (webhook history)
- **list_orders**: Use payment_status filter to narrow results. Supports limit for pagination.

Retrieve a paginated list of orders from Conekta
- **list_subscription_plans**: Retrieve a list of subscription plans in Conekta
- **search_customer_by_email**: Returns matching customer profiles.

Find a Conekta customer by their email address


## Installation & Usage

To install and use the **Conekta** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/conekta](https://vinkius.com/mcp/conekta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
