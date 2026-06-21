# Conekta MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/conekta)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/conekta-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/conekta-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Equip your AI agent to securely manage Latin American payments, view transactions, and track sales using the Conekta API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Conekta** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if the Conekta payment with ID 'ord_2nx...4kx' was successfully processed or declined."

**🤖 AI Agent:**
> The transaction 'ord_2nx...4kx' was successfully processed. It is a charge of $1,250.00 MXN made via credit card. The payment was cleared today at 10:45 AM and the associated customer is 'Carlos Mendoza'.

---

**👤 You:**
> "Summarize today's approved transactions and total revenue in MXN."

**🤖 AI Agent:**
> Today, you have 24 successfully approved transactions through Conekta. The total processed revenue is $34,800.00 MXN. There are also 2 transactions marked as 'declined' due to insufficient funds. Would you like a breakdown of the processing fees?

---

**👤 You:**
> "List the last 5 chargebacks or disputed claims in our account."

**🤖 AI Agent:**
> Here are the 5 most recent chargebacks:
1. ord_9ak - $800.00 MXN (Fraud alert)
2. ord_7bz - $1,200.00 MXN (Unrecognized charge)
3. ord_4cw - $500.00 MXN (Product not received)
4. ord_8dy - $2,500.00 MXN (Duplicate charge)
5. ord_1ex - $350.00 MXN (Fraud alert)
Shall I pull the customer details for ord_9ak?


## Installation & Usage

To install and use the **Conekta** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/conekta](https://vinkius.com/mcp/conekta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
