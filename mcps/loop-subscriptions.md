# Loop Subscriptions MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/loop-subscriptions)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/loop-subscriptions-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/loop-subscriptions-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Subscription management for Shopify — manage recurring orders and customers via Loop.

## Description
Empower your AI agents to handle **Loop Subscriptions** directly. This server allows you to monitor and manage recurring revenue, customer profiles, and subscription lifecycles on Shopify.

### What you can do

- **Subscription Control** — List, inspect, pause, resume, or cancel subscriptions instantly
- **Order Orchestration** — Monitor upcoming orders and skip next deliveries when requested by customers
- **Customer Management** — Access detailed profiles and subscription history for your users
- **Operational Visibility** — Track the status and health of your recurring business through simple natural language commands

### How it works

1. Subscribe to this server
2. Enter your **Loop Admin API Token**
3. Start managing your Shopify subscriptions from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **cancel_subscription**: Optional reason can be provided.

Cancel a subscription
- **get_customer**: Get customer details
- **get_subscription**: Get detailed info for a single subscription
- **list_customers**: List all customers with active or past subscriptions
- **list_orders**: List subscription orders
- **list_subscriptions**: List all Loop Subscriptions
- **pause_subscription**: You can optionally provide a resume date.

Pause an active subscription
- **resume_subscription**: Resume a paused subscription
- **skip_next_order**: Skip the next scheduled order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Loop Subscriptions** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my active subscriptions."

**🤖 AI Agent:**
> Fetching subscriptions... I've found 15 active subscriptions. Here are the most recent ones...

---

**👤 You:**
> "Pause subscription #12345 until 2026-12-01."

**🤖 AI Agent:**
> Pausing subscription #12345... Success! It is now scheduled to resume on December 1st, 2026.

---

**👤 You:**
> "Skip the next delivery for customer 'John Doe'."

**🤖 AI Agent:**
> Finding John Doe's subscription... Found! Skipping the next scheduled order as requested.


## Installation & Usage

To install and use the **Loop Subscriptions** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/loop-subscriptions](https://vinkius.com/mcp/loop-subscriptions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
