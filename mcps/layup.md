# Layup MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/layup)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/layup-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/layup-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage digital lay-by orders, track deposits, and fetch checkout customer data via Layup straight from your AI agent.

## Description
Connect your **Layup** operational account to any AI agent and manage lay-by e-commerce checkout infrastructures effortlessly.

### What you can do

- **Order Metrics** — List all captured lay-by checkouts and inspect target order data instantly
- **Track Payments** — Check the deposit status, timeline, and pending metrics on Layup checkouts
- **Customer Data** — Cross-reference buyer metrics with internal logs
- **Store Automation** — Programmatically create new virtual lay-bys dynamically based on AI discussions

### How it works

1. Subscribe to this server
2. Enter your Layup Merchant API Key
3. Start fetching and creating installments right from Claude or Cursor

### Who is this for?

- **E-Commerce Operators** — check if an installment was completely matched directly via chat
- **Support Teams** — quickly check customer balances and order logs organically
- **Developers** — audit tracking and debugging logs directly from within your IDE


## Available Tools
- **cancel_order**: Void an existing Layup order
- **create_deposit**: Register a new lay-by deposit manually
- **create_order**: Initialize a new lay-by order
- **get_customer**: Retrieve customer explicit parameters
- **get_order**: Get parameters surrounding an explicit order
- **get_payment**: Fetch targeted payment details
- **list_customers**: Read globally saved shopper customers
- **list_orders**: Retrieve active lay-by payment plan orders
- **list_payments**: Retrieve all payments linked to an order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Layup** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find order ID 900 and tell me its completion balance."

**🤖 AI Agent:**
> Understood. Fetching from your Layup module... Order 900 holds a remaining balance of 20.00ZAR with status set as Incomplete.

---

**👤 You:**
> "Fetch all recorded incoming deposits."

**🤖 AI Agent:**
> Connecting to API... You have 15 recent deposit lines mapped over your active lay-bys in the last window.

---

**👤 You:**
> "Search for customer details on the Layup platform."

**🤖 AI Agent:**
> Querying customer list... Retrieved 3 profiles. Should I filter by email?


## Installation & Usage

To install and use the **Layup** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/layup](https://vinkius.com/mcp/layup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
