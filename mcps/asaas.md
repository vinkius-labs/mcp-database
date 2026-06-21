# Asaas MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/asaas)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/asaas-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/asaas-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage payments, customers, and subscriptions with Asaas — the complete digital account for Brazilian businesses via AI.

## Description
The **Asaas MCP Server** provides a powerful natural language interface to your Asaas digital account. Specifically designed for Brazilian businesses, this integration allows your AI agent to manage your entire billing cycle, from customer registration to payment collection and financial transfers.

### Key Features

- **Billing Management** — Create and list payments via Boleto, Credit Card, and PIX with automated status tracking.
- **Customer Inventory** — Manage your customer base, including CPF/CNPJ verification and contact details synchronization.
- **Subscription Automation** — Monitor active recurring billings and subscription statuses for your clients.
- **Financial Oversight** — Check your account balance and track transfers in real-time.
- **Workflow Integration** — Seamlessly connect your payment operations with your AI-assisted support and sales processes.
- **Secure API Access** — Uses the Asaas `access_token` for authenticated communication and supports sandbox mode for safe testing.

### Who is this for?

- **Small Business Owners** — Quickly audit receivables and check your balance using simple natural language commands.
- **Sales Teams** — Register new customers and generate payment links (PIX/Boleto) instantly during conversations.
- **Finance Departments** — Monitor payment statuses and manage recurring subscriptions without manual dashboard exports.


## Available Tools
- **create_customer**: Register a new customer in Asaas
- **create_payment**: Create a new payment (charge) for a customer
- **get_account_check**: Verify Asaas account connection
- **get_balance**: Get current financial balance in Asaas
- **list_customers**: List all registered customers in Asaas
- **list_payments**: List all payments (charges)
- **list_subscriptions**: List all active subscriptions
- **list_transfers**: List all financial transfers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Asaas** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my current Asaas balance."

**🤖 AI Agent:**
> Your current balance in Asaas is R$ 5,240.50, with R$ 1,200.00 pending settlement.

---

**👤 You:**
> "List the last 5 payments received."

**🤖 AI Agent:**
> I've retrieved your recent payments. You received 5 payments today, totaling R$ 850.00, including 3 via PIX and 2 via Credit Card.

---

**👤 You:**
> "Create a PIX charge of R$ 100 for customer 'cus_12345' due tomorrow."

**🤖 AI Agent:**
> The PIX charge for R$ 100.00 has been successfully created for customer 'cus_12345'. The due date is set for tomorrow.


## Installation & Usage

To install and use the **Asaas** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/asaas](https://vinkius.com/mcp/asaas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
