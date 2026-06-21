# MoonClerk MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moonclerk-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/moonclerk-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/moonclerk-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Accept recurring and one-time payments with beautifully designed checkout pages that embed anywhere on your website.

## Description
Connect your **MoonClerk** account to any AI agent to streamline your payment monitoring and customer oversight. MoonClerk provides a robust API for programmatically retrieving your payment records, customer plan details, and active payment forms.

### What you can do

- **Customer Monitoring** — List all your customers (plans) and retrieve detailed metadata including status and plan types
- **Payment Tracking** — Access your full payment history and monitor the status of recurring and one-time transactions
- **Form Orchestration** — List all your active payment forms and retrieve their public URLs and configurations
- **Coupon Intelligence** — Access your list of active coupons to understand your promotional landscape
- **Real-time Oversight** — Get a comprehensive overview of your payment volume and customer growth using natural language commands

### How it works

1. Subscribe to this server
2. Enter your MoonClerk API Key from your account settings
3. Start monitoring your payments from Claude, Cursor, or any MCP client

### Who is this for?

- **Finance Managers** — monitor transaction statuses and payment volumes using natural language
- **Business Owners** — get a real-time overview of customer growth and form performance
- **Developers** — integrate real-time payment data into custom financial dashboards


## Available Tools
- **get_customer**: Get customer details
- **get_form**: Get form details
- **get_payment**: Get payment details
- **list_coupons**: List all coupons
- **list_customers**: List all MoonClerk customers
- **list_forms**: List all payment forms
- **list_payments**: List all payments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MoonClerk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active customers in my MoonClerk account."

**🤖 AI Agent:**
> I've retrieved your customer list. You have 50 active customers (plans), including 'John Doe' and 'Maria Garcia'. Would you like to see the payment history for any of them?

---

**👤 You:**
> "Show the last 5 payments received today."

**🤖 AI Agent:**
> I've fetched today's payments. You have 5 new transactions totaling $450.00 USD, with all transactions marked as 'Successful'.

---

**👤 You:**
> "List all my active payment forms."

**🤖 AI Agent:**
> I've retrieved your payment forms. You have 3 active forms: 'Basic Subscription', 'Premium Monthly', and 'Annual Pass'. Which URL would you like to retrieve?


## Installation & Usage

To install and use the **MoonClerk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moonclerk-alternative](https://vinkius.com/mcp/moonclerk-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
