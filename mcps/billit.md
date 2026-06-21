# Billit MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/billit)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/billit-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/billit-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your e-invoicing via Billit — list invoices, clients, and expenses directly from any AI agent.

## Description
Connect your **Billit** account to any AI agent and orchestrate your e-invoicing and accounting workflows through natural conversation.

### What you can do

- **Invoicing Oversight** — List and retrieve detailed e-invoices across the Peppol network.
- **Party Management** — Manage your CRM of customers and suppliers (Parties) within Billit.
- **Expense Tracking** — Query incoming expenses and receipts.
- **Product Catalog** — Access your products and services list.
- **Company Information** — Retrieve the authenticated company's core details.

### How it works

1. Subscribe to this server
2. Enter your Billit API Key and Environment (e.g., api.sandbox for testing)
3. Start managing your billing operations from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **create_invoice**: Create a new invoice
- **create_party**: Create a new party (customer)
- **get_company_info**: Get your company information
- **get_invoice**: Get specific invoice details
- **get_party**: Get specific party details
- **list_expenses**: List all expenses
- **list_invoices**: List all invoices
- **list_parties**: List all parties (customers/suppliers)
- **list_products**: List all products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Billit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active invoices."

**🤖 AI Agent:**
> I've retrieved your invoices. You have 5 recent invoices, including 'INV-2024-001' (Status: Paid) and 'INV-2024-005' (Status: Draft).

---

**👤 You:**
> "Find the contact details for 'Acme Corp'."

**🤖 AI Agent:**
> I found one matching party: 'Acme Corporation' (ID: party_992). Their primary contact is John Smith, and their tax ID is BE0123456789.

---

**👤 You:**
> "Show my last 3 expenses."

**🤖 AI Agent:**
> Retrieving expenses... Your 3 most recent expenses include 'Office Supplies' (€45.50), 'Cloud Hosting' (€120.00), and 'Internet Bill' (€60.00).


## Installation & Usage

To install and use the **Billit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/billit](https://vinkius.com/mcp/billit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
