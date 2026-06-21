# Memberful MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/memberful)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/memberful-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/memberful-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Monetize your content with membership subscriptions that integrate seamlessly into your existing website and WordPress setup.

## Description
Connect your **Memberful** account to any AI agent and take full control of your membership site orchestration and subscription efficiency through natural conversation. Memberful provides a powerful GraphQL platform for managing gated content and recurring revenue, and this integration allows you to retrieve member metadata, monitor active subscriptions, and oversee sales orders directly from your chat interface.

### What you can do

- **Member & Profile Orchestration** — List all managed members and retrieve detailed profile metadata programmatically to ensure your audience database is always synchronized.
- **Subscription Lifecycle Management** — Access and monitor active subscriptions, expiration dates, and assigned plans directly from the AI interface to track recurring revenue health.
- **Order & Financial Intelligence** — List and oversee recent sales orders and retrieve detailed transaction metadata via natural language to maintain a clear overview of organizational liquidity.
- **Plan & Discount Control** — Retrieve master data for membership plans and available discounts using simple AI commands to facilitate better promotional alignment.
- **Operational Monitoring** — Track system responses and manage webhook metadata to ensure your automation workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Memberful API Key and Site Name (subdomain) from your dashboard settings
3. Start managing your membership business from Claude, Cursor, or any MCP-compatible client

No more manual status checking in the dashboard for new subscribers. Your AI acts as a dedicated membership coordinator or operations assistant.

### Who is this for?

- **Publishers & Creators** — quickly retrieve member summaries and monitor churn without switching apps.
- **Operations Managers** — automate the retrieval of subscription metadata and track plan distribution via natural conversation.
- **Developers** — integrate real-time membership data and site metadata directly within the chat.


## Available Tools
- **create_member**: Create a new member
- **get_account_info**: Get site info
- **get_member**: Get member details
- **get_order**: Get order details
- **list_coupons**: List active coupons
- **list_discounts**: List member discounts
- **list_downloads**: List member downloads
- **list_members**: List all members
- **list_orders**: List recent orders
- **list_plans**: List subscription plans
- **list_subscriptions**: List all subscriptions
- **list_webhooks**: List configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Memberful** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active membership plans in Memberful."

**🤖 AI Agent:**
> I've retrieved your plans. You have 3 active options: 'Premium Monthly', 'Annual Supporter', and 'Founding Member'. Which one would you like to see subscriber counts for?

---

**👤 You:**
> "Show the last 5 orders in my Memberful site."

**🤖 AI Agent:**
> I've retrieved your recent orders. You had 5 transactions today totaling $450, including new subscriptions for 'Alice Miller' and 'Robert Chen'.

---

**👤 You:**
> "Get details for member ID '12345'."

**🤖 AI Agent:**
> I've retrieved the metadata for member ID 12345. It belongs to Sarah Jones (sarah@example.com), who is currently on the 'Annual Supporter' plan expiring in 6 months.


## Installation & Usage

To install and use the **Memberful** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/memberful](https://vinkius.com/mcp/memberful)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
