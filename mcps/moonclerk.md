# MoonClerk MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moonclerk)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/moonclerk-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/moonclerk-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage recurring payments and customers via MoonClerk — track transactions and view payment forms directly from your AI agent.

## Description
Connect your **MoonClerk** account to your AI agent and take control of your recurring revenue and customer billing through natural conversation.

### What you can do

- **Payment Tracking** — List all transactions and get real-time status updates, amounts, and currency info.
- **Customer & Plan Management** — Access customer profiles, recurring payment plans, and active subscriptions.
- **Form Oversight** — List and inspect your payment forms to stay organized.
- **Deep Data Inspection** — Fetch complete metadata for specific customers, payments, or plans using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your MoonClerk API Key
3. Start managing your billing from Claude, Cursor, or any MCP client

### Who is this for?

- **Subscription-based Businesses** — quickly check if a subscriber's payment has cleared or verify plan details.
- **Support Teams** — verify customer billing status and subscription info while providing assistance.
- **Finance Operations** — automate the retrieval of transaction and plan lists for reporting.


## Available Tools
- **get_customer**: Get specific customer details
- **get_form**: Get specific form details
- **get_payment**: Get details for a specific payment
- **get_plan**: Get specific plan details
- **get_subscription**: Get specific subscription info
- **list_customers**: List MoonClerk customers
- **list_forms**: List payment forms
- **list_payments**: List all payments
- **list_plans**: List available payment plans
- **list_subscriptions**: List active subscriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MoonClerk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 payments received on MoonClerk."

**🤖 AI Agent:**
> I've retrieved your recent payments. You have 5 recent transactions: three for $50.00 (Status: Succeeded) and two for $25.00. Would you like details on the customer for the most recent one?

---

**👤 You:**
> "What recurring payment plans do I have configured?"

**🤖 AI Agent:**
> Retrieving your plans... You have 3 recurring plans: 'Monthly Membership' ($29/mo), 'Annual Pro' ($290/yr), and 'Starter Kit' (One-time). Shall I list the active subscribers for the Monthly Membership?

---

**👤 You:**
> "Show me the details for the payment form with ID form_123."

**🤖 AI Agent:**
> Inspecting form_123... This form is titled 'Donation Page', it is currently 'active', and has been used for 45 successful transactions. Would you like the checkout URL for this form?


## Installation & Usage

To install and use the **MoonClerk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moonclerk](https://vinkius.com/mcp/moonclerk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
