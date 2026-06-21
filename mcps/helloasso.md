# HelloAsso MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/helloasso)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/helloasso-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/helloasso-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [event-management](../categories/event-management.md)

Automate association management via HelloAsso — manage payments, forms, and orders for French non-profits directly from any AI agent.

## Description
Connect your **HelloAsso** account to any AI agent and take full control of your French non-profit management workflows through natural conversation.

### What you can do

- **Organization Oversight** — List and inspect all organizations where you have administrative rights.
- **Campaign Management** — List all active and past forms (Donations, Memberships, Events, Shop).
- **Payment Monitoring** — Access your financial history, track donations, and retrieve detailed payment metadata.
- **Order Handling** — List and inspect orders to understand payer behavior and item distribution.
- **Checkout Intents** — Generate redirect links for payments directly from the chat interface.
- **Member & Subscription Tracking** — Manage your membership base and monitor recurring donation plans.

### How it works

1. Subscribe to this server
2. Enter your HelloAsso Client ID and Client Secret
3. Start managing your association from Claude, Cursor, or any MCP-compatible client

No more manual exporting of transaction CSVs. Your AI assistant acts as a dedicated Association Coordinator or Financial Manager.

### Who is this for?

- **Non-Profit Directors** — instantly retrieve donation totals and campaign progress without digging through the dashboard.
- **Community Managers** — check membership statuses and event registration counts in real-time.
- **Financial Officers** — automate the oversight of payments and subscriptions across multiple associations.


## Available Tools
- **create_checkout_intent**: Pass the amount in cents (EUR) and other required fields as a JSON string in "body_json". Returns a redirect URL for the payer.

Generate a checkout link to receive a payment
- **get_member_details**: Get details for a specific member ID
- **get_order_details**: Get details for a specific order ID
- **get_organization_details**: Get detailed information about a specific organization by its slug
- **get_payment_details**: Get details for a specific payment ID
- **list_forms**: Each form has a "formType" and "formSlug" used for detailed lookups.

List all campaigns/forms (Donations, Memberships, Events) for an organization
- **list_sold_items**: g., ticket, membership tier) that were part of orders.

List all individual items sold/distributed by an organization
- **list_my_organizations**: Use this to find the "slug" required for other tools.

List all organizations where the user has administrative rights
- **list_orders**: An order represents one or more items purchased or donated by a user in a single session.

List all orders (group of items/payments) for an organization
- **list_payments**: Returns amounts in cents (EUR). Use this to track donations or membership payments.

List all payments received by an organization
- **list_subscriptions**: List recurring payments (subscriptions) for an organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HelloAsso** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active campaigns for my association 'Protect Oceans'."

**🤖 AI Agent:**
> I've retrieved your forms for 'Protect Oceans' (slug: protect-oceans). You have 3 active campaigns: 'Annual Donation Drive', 'Membership 2024', and 'Gala Dinner Tickets'. Which one would you like to see statistics for?

---

**👤 You:**
> "Show me the last 5 payments received today."

**🤖 AI Agent:**
> Fetching today's payments... I found 5 recent transactions totaling 245.00 EUR. The largest was a 100.00 EUR donation from Jean Dupont. Should I list the individual items for each payment?

---

**👤 You:**
> "Generate a checkout link for a 50 EUR donation."

**🤖 AI Agent:**
> I've initiated the checkout process. I need your association's slug to complete the link. Once you provide it, I'll generate a redirect URL for a 50.00 EUR donation (5000 cents). What is the association slug?


## Installation & Usage

To install and use the **HelloAsso** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/helloasso](https://vinkius.com/mcp/helloasso)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
