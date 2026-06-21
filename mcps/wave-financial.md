# Wave Financial MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wave-financial)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wave-financial-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wave-financial-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage your accounting via Wave Financial — query businesses, invoices, customers, and transactions directly from any AI agent.

## Description
Connect your AI agent to **Wave Financial**, the all-in-one accounting software for small businesses. This integration utilizes Wave's powerful GraphQL API to provide real-time access to your financial data through natural conversation.

### What you can do

- **Business Oversight** — List and inspect all businesses associated with your Wave account
- **Invoice Management** — Retrieve summaries of sent invoices, including statuses, totals, and due dates
- **Customer & Vendor Directory** — Quickly lookup contact details for your customers and suppliers
- **Accounting Intelligence** — Monitor your chart of accounts and current balances across different categories
- **Expense Tracking** — List recent bills and accounting transactions to stay on top of your cash flow
- **Tax Configuration** — Retrieve active sales tax rates and configurations for your business

### How it works

1. Subscribe to this server
2. Enter your **Wave Personal Access Token** (generated in your Wave Developer Portal)
3. Start managing your business finances directly through chat

### Who is this for?

- **Small Business Owners** — quickly check invoice statuses and account balances without logging into the dashboard
- **Accountants & Bookkeepers** — retrieve transaction lists and customer data for reporting
- **Financial Analysts** — audit business performance and cash flow via AI


## Available Tools
- **get_user_info**: Retrieve the authenticated user information
- **list_accounts**: List the chart of accounts for a specific business
- **list_bills**: List bills (accounts payable) for a specific business
- **list_businesses**: List all businesses associated with the user account
- **list_customers**: List customers for a specific business
- **list_invoices**: List invoices for a specific business
- **list_products**: List products and services for a specific business
- **list_sales_taxes**: List sales taxes configured for a specific business
- **list_transactions**: List accounting transactions for a business
- **list_vendors**: List vendors associated with a specific business


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wave Financial** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my businesses in Wave."

**🤖 AI Agent:**
> You have 2 businesses: 'Design Studio' (ID: 123) and 'E-commerce Shop' (ID: 456). Which one would you like to inspect?

---

**👤 You:**
> "Show me the latest invoices for business ID 123."

**🤖 AI Agent:**
> Fetching invoices for 'Design Studio'... I found 3 recent invoices: #INV-001 (Paid, $500), #INV-002 (Sent, $1,200), and #INV-003 (Overdue, $300).


## Installation & Usage

To install and use the **Wave Financial** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wave-financial](https://vinkius.com/mcp/wave-financial)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
