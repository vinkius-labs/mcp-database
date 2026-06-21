# Whop MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/whop)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/whop-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/whop-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage digital products, payments, and memberships on Whop with AI agents.

## Description
Connect your **Whop** account to any AI agent to automate your digital commerce and membership operations. Whop provides an all-in-one platform for selling digital access, managing subscriptions, and tracking customer payments through natural conversation.

### What you can do

- **Product Orchestration** — List and manage your digital products and subscription plans with detailed pricing metadata.
- **Membership Management** — Retrieve active user memberships, monitor subscription statuses, and process cancellations programmatically.
- **Financial Monitoring** — Track payment histories and retrieve customer invoices directly from the AI interface to monitor revenue streams.
- **Marketing Automation** — Create and manage promo codes for your digital storefront to drive sales through natural language commands.
- **Customer Experience** — Monitor product reviews and user feedback to stay updated on your community's health.

### How it works

1. Subscribe to this server
2. Enter your Whop Company API Key from your developer settings
3. Start managing your digital storefront from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Digital Creators** — manage software access and community memberships more efficiently without leaving the chat.
- **E-commerce Operations** — automate the tracking of payments, invoices, and promo codes.
- **Community Managers** — quickly check user membership statuses and process administrative tasks via natural conversation.


## Available Tools
- **cancel_membership**: Cancel a user membership
- **create_promo_code**: Create a new promo code
- **get_membership**: Get details for a specific membership
- **list_invoices**: List customer invoices
- **get_me**: Get current Whop user or company details
- **list_memberships**: List user memberships
- **list_payments**: List payment transactions
- **list_plans**: List all Whop subscription plans
- **list_products**: List all Whop products
- **list_promo_codes**: List promotional codes
- **list_reviews**: List product reviews


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Whop** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new promo code 'SUMMER2024' that gives a 20% discount on the 'Premium VIP Signals' subscription plan."

**🤖 AI Agent:**
> I've successfully created the promo code 'SUMMER2024' offering a 20% discount. It is now active and linked to the 'Premium VIP Signals' plan. Your customers can start using it immediately at checkout.

---

**👤 You:**
> "Find the membership details for user ID 'usr_89231' and cancel their active subscription immediately."

**🤖 AI Agent:**
> I located the membership for user 'usr_89231', which was active on the 'Pro Access' plan. I have successfully processed the cancellation. The user will retain access until the end of their current billing cycle on October 15th.

---

**👤 You:**
> "Check our most recent customer reviews for the 'Trading Masterclass' product and verify if the latest transaction from today was successful."

**🤖 AI Agent:**
> I found 5 recent reviews for the 'Trading Masterclass', averaging 4.8 stars, with the latest praising the new video modules. I also checked today's payments; the most recent transaction (TXN-9402) for $149.00 was successfully processed and cleared.


## Installation & Usage

To install and use the **Whop** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/whop](https://vinkius.com/mcp/whop)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
