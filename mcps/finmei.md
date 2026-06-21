# Finmei MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/finmei)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/finmei-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/finmei-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage expenses, tax rates, and payments through conversational AI agents with Finmei.

## Description
Connect your **Finmei** account to any AI agent and automate your financial operations through the Model Context Protocol (MCP). Finmei is the ideal companion for freelancers and small businesses that need to track expenses and manage invoices without the complexity of traditional accounting software.

### What you can do

- **Expense Tracking** — Digitally record and list all business expenses. Fetch details or delete entries directly through natural conversation.
- **Tax Management** — List and manage your tax types (Tax Rates) to ensure your financial records are always accurate and compliant.
- **Payment Monitoring** — Keep track of all payments associated with your business. List recent payments or drill down into specific transaction details.
- **Business Profiling** — Access your business profile metadata to ensure your agent has the right context for generating reports or invoices.
- **Global Support** — Fetch supported currencies and manage international transactions with support for over 180 currencies.
- **Category Organization** — Organize your finances by listing and applying expense categories to your records.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Finmei API Token (found in your Settings > Integrations)
3. Start managing your business expenses and payments from Claude, Cursor, or any MCP client

### Who is this for?

- **Freelancers & Solopreneurs** — quickly log expenses and check payment statuses while you work, without opening a separate browser tab.
- **Small Business Owners** — get a quick overview of your tax types and recent expenses to keep your finger on the pulse of your cash flow.
- **Agency Leads** — automate the retrieval of financial data for client reports or internal audits.


## Available Tools
- **create_expense**: Create a new expense
- **delete_expense**: Delete an expense
- **delete_payment**: Delete a payment
- **get_expense**: Get expense details
- **get_payment**: Get payment details
- **get_profile**: Get business profile
- **list_categories**: List expense categories
- **list_currencies**: List supported currencies
- **list_expenses**: List expenses
- **list_payments**: List payments
- **list_tax_types**: List tax rates
- **update_expense**: Update an expense


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Finmei** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my 10 most recent business expenses."

**🤖 AI Agent:**
> Fetching your expenses... I found your 10 most recent entries, including 'Office Supplies' ($45.00) and 'Cloud Hosting' ($120.00). Would you like to see the full details for any of these?

---

**👤 You:**
> "Add a new expense: 'Monthly Internet Subscription', 50 USD, for today."

**🤖 AI Agent:**
> Expense recorded! I've added 'Monthly Internet Subscription' for 50 USD to your Finmei account. The entry is now tracked and categorized.

---

**👤 You:**
> "Show me all available tax rates for my account."

**🤖 AI Agent:**
> Retrieving tax types... Your account has 3 tax rates configured: 'VAT 20%', 'Sales Tax 5%', and 'Zero Rated'. Which one should I apply to your next entry?


## Installation & Usage

To install and use the **Finmei** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/finmei](https://vinkius.com/mcp/finmei)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
