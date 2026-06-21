# Sage Accounting MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sage-accounting)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sage-accounting-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sage-accounting-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate business finances via Sage Accounting — manage invoices, banking, and contacts directly from any AI agent.

## Description
Connect your **Sage Business Cloud Accounting** account to any AI agent and take full control of your financial orchestration through natural conversation. Sage is a leading cloud accounting platform, and this integration allows you to retrieve ledger metadata, monitor bank transactions, and manage professional contacts directly from your chat interface.

### What you can do

- **Invoice & Financial Orchestration** — List sales and purchase invoices programmatically to maintain a clear overview of your accounts receivable and payable.
- **Banking & Transaction Intelligence** — Access bank accounts and retrieve real-time transaction metadata to keep your cash flow synchronized directly from the AI interface.
- **Contact & CRM Control** — List and search through your customer and supplier database to maintain accurate records via natural language.
- **Inventory & Ledger Management** — Access product catalogs, service lists, and ledger accounts to ensure your accounting data is always optimized.
- **Operational Monitoring** — Track tax rates and retrieve business profile metadata using simple AI commands to ensure compliance.

### How it works

1. Subscribe to this server
2. Enter your Sage OAuth 2.0 Access Token from your developer application
3. Start managing your business finances from Claude, Cursor, or any MCP-compatible client

No more manual report exports or multiple dashboard logins. Your AI acts as a dedicated financial analyst or assistant accountant.

### Who is this for?

- **Small Business Owners** — quickly retrieve balance summaries and monitor unpaid invoices without switching apps.
- **Finance Teams** — automate the retrieval of transaction metadata and track tax rates via natural conversation.
- **Accountants** — streamline the monitoring of ledger accounts and monitor client business health directly within the chat.


## Available Tools
- **get_sales_invoice**: Get details for a specific sales invoice
- **list_bank_accounts**: List business bank accounts
- **list_businesses**: List accessible businesses
- **list_contacts**: ) in the accounting system.

List customers and suppliers
- **list_ledger_accounts**: List Chart of Accounts
- **get_user_info**: Get Sage user information
- **list_products**: List physical products
- **list_purchase_invoices**: List purchase invoices
- **list_sales_invoices**: List sales invoices
- **list_services**: List service items
- **list_tax_rates**: List configured tax rates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sage Accounting** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active sales invoices in my Sage account."

**🤖 AI Agent:**
> I've retrieved your invoices. You have 5 active records including #INV-1001 (Sent) and #INV-1002 (Draft). Would you like to see the customer details for the sent invoice?

---

**👤 You:**
> "Show me all outstanding sales invoices and the total accounts receivable balance."

**🤖 AI Agent:**
> 23 outstanding sales invoices totaling $156,400. Overdue (8): $67,200 (oldest: INV-2025-089 from Meridian Corp, $12,400, 34 days past due). Due this week (6): $42,800. Due within 30 days (9): $46,400. Top debtors: Meridian Corp ($28,400 across 3 invoices), TechVentures ($18,600 across 2 invoices), DataFlow ($14,200). Average collection period: 28 days. Payment terms breakdown: Net 30 (65%), Net 15 (25%), Due on receipt (10%). 4 invoices have partial payments recorded.

---

**👤 You:**
> "List all bank accounts with their current balances and recent transaction activity."

**🤖 AI Agent:**
> 4 bank accounts configured. "Business Current Account" (ending 4521): Balance $234,500. Last 7 days: 23 deposits ($89,200), 45 payments ($67,400), net +$21,800. "Savings Account" (ending 7834): Balance $450,000 (reserve fund). "Tax Reserve" (ending 2156): Balance $67,800. "PayPal Business" (ending 9012): Balance $12,340. Total cash position: $764,640. Unreconciled transactions: 12 items ($8,900). Automatic bank feed: synced 1 hour ago.


## Installation & Usage

To install and use the **Sage Accounting** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sage-accounting](https://vinkius.com/mcp/sage-accounting)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
