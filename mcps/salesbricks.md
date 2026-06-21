# Salesbricks MCP Server

Integrate Salesbricks seamlessly into your AI. Quickly manage B2B customer billing, track active subscriptions, list available software plans, and audit invoices natively.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/salesbricks)

## Overview
**Category:** money-moves
**Tools Count:** 10

## Description
Connect your conversational assistant natively to **Salesbricks**, the fastest way to turn your SaaS products into purchasable assets with its simple quote-to-cash B2B checkout platform. Seamlessly instruct your AI to orchestrate customer billing, manage monthly subscriptions, and track usage data instantly via conversational prompts.

### What you can do

- **Client Administration** — Easily search for your enterprise users or create brand new B2B customer accounts directly from chat (`list_customers`, `create_customer`). You can also retrieve their robust global profile covering active subscriptions and payments (`get_customer`).
- **Usage and Events Tracking** — Securely log system usage events natively utilizing the (`record_usage`) tool to feed Salesbricks accurate billing intelligence.
- **Subscriptions and Invoices** — Audit your entire library of commercial software subscriptions and cross-reference them with actual active clients globally (`list_subscriptions`). Fetch and inspect comprehensive revenue ledgers outlining successfully delivered invoices effortlessly (`list_invoices`).
- **Product Offerings** — View your complete list of monetized products securely (`list_products`).

### How it works

1. Enable the Salesbricks application suite in your hub.
2. Navigate to your secure web dashboard on Salesbricks and find the Developer Tools page.
3. Create an API Key and copy the 'X-SALESBRICKS-KEY'.
4. Paste it exclusively in the required secure parameters beneath to validate communication natively.
5. Ask the AI: "Enumerate my latest software subscription plans currently assigned to active users in my platform."


## Available Tools
- **create_customer**: Specify company name and email.

Creates a new customer in Salesbricks
- **create_subscription**: Provide a JSON object with customerId and plan details.

Creates a new subscription for a customer
- **delete_customer**: This action is irreversible.

Deletes a customer from Salesbricks
- **get_customer**: Retrieves details for a specific customer
- **list_customers**: Lists all customers in the Salesbricks account
- **list_invoices**: Lists all generated invoices
- **list_products**: Lists all available product plans
- **list_subscriptions**: Lists all active and historical subscriptions
- **record_usage**: Provide a JSON object with event details.

Records a usage event for a customer
- **update_customer**: Updates an existing customer's name


## Installation & Usage

To install and use the **Salesbricks** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salesbricks](https://vinkius.com/mcp/salesbricks)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
