# Daftra MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/daftra-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/daftra-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/daftra-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [crm](../categories/crm.md)

Run your Arabic-first business with invoicing, inventory, CRM, and accounting designed for the Middle East and North Africa.

## Description
Connect your **Daftra** account to any AI agent and take full control of your business accounting and ERP operations through natural conversation.

### What you can do

- **Invoicing Orchestration** — Create and manage professional invoices programmatically, including monitoring payment status and line item configurations in real-time
- **Client Relationship Management** — Access complete client profiles and interaction history to maintain high-fidelity customer records across the MENA region
- **Inventory & Product Intelligence** — Access your complete product catalog and retrieve real-time stock levels and service metadata directly through your agent
- **Financial Visibility** — Monitor business expenses, treasury balances, and client payments to maintain a high-fidelity overview of your financial health
- **Staff Coordination** — Retrieve directories of staff members and manage account-level metadata directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from Daftra dashboard (Settings > API > API Keys)
3. Identify your **Subdomain** (e.g., 'yourcompany' from yourcompany.daftra.com)
4. Start automating your business operations from Claude, Cursor, or any MCP client

No more manual deal logging or digging through complex accounting tables. Your AI acts as your dedicated ERP specialist and financial coordinator.

### Who is this for?

- **Business Owners in MENA** — instantly retrieve sales summaries and update client details using natural language commands
- **Accountants & Finance Leads** — monitor invoice statuses and track business expenses without leaving your communication tools
- **Operations Managers** — automate product catalog management and verify treasury balances through simple AI queries


## Available Tools
- **create_client**: Create a new client
- **create_invoice**: Requires client_id and invoice items.

Create a new invoice
- **create_product**: Create a new product
- **get_account_info**: Get account details
- **get_invoice**: Get invoice details
- **list_staff**: List staff members
- **list_treasuries**: List treasuries/accounts
- **list_clients**: List all clients
- **list_expenses**: List business expenses
- **list_invoices**: List all invoices
- **list_payments**: List recent payments
- **list_products**: List all products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Daftra** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all unpaid invoices in my account."

**🤖 AI Agent:**
> I've retrieved your unpaid invoices. You have 3 pending payments, including Invoice #4501 for 'Ali Hassan' and #4502. Would you like the full item details for the largest invoice?

---

**👤 You:**
> "Create a new client 'Ahmed Khalid' with email 'ahmed@example.com'."

**🤖 AI Agent:**
> Client created! Ahmed Khalid has been added to your Daftra database (ID: cl_123). He is now available for invoicing and project assignments. Shall I create an initial invoice for him?

---

**👤 You:**
> "Show me the current treasury balances."

**🤖 AI Agent:**
> Accessing financial records... Your Main Cash account has $5,420.00 and the Business Bank account (ID: tr_456) shows $12,800.00. Both are in good standing. Need a summary of recent expenses?


## Installation & Usage

To install and use the **Daftra** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/daftra-alternative](https://vinkius.com/mcp/daftra-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
