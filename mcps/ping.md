# Ping++ MCP Server

Bring unified payment intelligence to your AI with Ping++. Integrate WeChat, Alipay, and UnionPay through a single clean API interface.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ping)

## Overview
**Category:** money-moves
**Tools Count:** 7

## Description
Empower your Agent to seamlessly manage Chinese payment ecosystems with **Ping++**, the ultimate multi-channel payment aggregator. Connect to WeChat Pay, Alipay, UnionPay, and multiple other networks through a single, elegant interface, replacing complex point-to-point integrations.

### What you can do

- **Unified Charges** — Create and manage transactions across any supported payment channel
- **Refund Management** — Process and retrieve refunds across any network without learning specific gateway APIs
- **Customer Synchronization** — Create and track customer profiles and saved payment methods across platforms

### How it works

1. Subscribe to this server
2. Obtain your Secret API Key from your [Ping++ Developer Dashboard](https://dashboard.pingxx.com)
3. Inject the server into your LLM client and instantly manage multi-channel billing flows

### Who is this for?

- **E-Commerce Agents** — Automate refunds, track transaction states, and manage cross-channel payments seamlessly
- **Financial Operators** — Consolidate the management of WeChat and Alipay transactions without touching backend code
- **Developers in China** — Connect multiple SDK backends to a single MCP endpoint to rapid prototype monetization


## Available Tools
- **create_charge**: Requires the order_no, amount, app ID, channel, currency, subject, and body.

Create a new charge (payment request)
- **create_customer**: Create a new Customer
- **create_refund**: Create a refund for a specific charge
- **list_charges**: List existing charges
- **list_customers**: List existing Customers
- **retrieve_charge**: Retrieve the details of an existing charge
- **retrieve_customer**: Retrieve Customer details


## Installation & Usage

To install and use the **Ping++** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ping](https://vinkius.com/mcp/ping)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
