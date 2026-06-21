# Invoice Ninja MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/invoice-ninja)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/invoice-ninja-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/invoice-ninja-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage clients, invoices, and products directly through AI.

## Description
### What you can do
- **List and retrieve clients:** Instantly access client details, contacts, and custom fields.
- **Create and manage invoices:** Generate invoices, fetch specific invoice details, and streamline your billing process.
- **Handle products and payments:** Track your products, record payments, and manage financial operations seamlessly via AI.

### How it works
1. Sign up for Invoice Ninja or use your self-hosted instance.
2. Generate an API Token in Settings > Advanced Settings > API Tokens.
3. Enter the token (and optional custom Base URL) in the agent setup, and start managing your billing operations.

### Who is it for?
Freelancers, small businesses, and agencies who need a powerful, automated way to handle invoicing and client management directly from their AI assistant.


## Available Tools
- **create_client**: Create a new client
- **create_invoice**: Create a new invoice
- **create_product**: Create a new product
- **get_client**: Get details for a specific client
- **get_invoice**: Get an invoice by ID
- **get_payment**: Get a payment by ID
- **get_product**: Get a product by ID
- **list_clients**: List clients in Invoice Ninja
- **list_invoices**: List invoices
- **list_payments**: List payments
- **list_products**: List products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Invoice Ninja** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my latest clients."

**🤖 AI Agent:**
> I've fetched your clients. You have Acme Corp, Globex, and Initech.

---

**👤 You:**
> "Create a new product called 'Consulting Hours' with a price of 150."

**🤖 AI Agent:**
> The product 'Consulting Hours' has been successfully created with a price of 150.

---

**👤 You:**
> "Get the details for invoice ID 12345."

**🤖 AI Agent:**
> Invoice 12345 is for $500, assigned to Acme Corp, and is currently marked as 'Sent'.


## Installation & Usage

To install and use the **Invoice Ninja** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/invoice-ninja](https://vinkius.com/mcp/invoice-ninja)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
