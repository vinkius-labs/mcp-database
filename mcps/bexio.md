# Bexio MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bexio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bexio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bexio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage your business via Bexio — list contacts, invoices, and projects directly from any AI agent.

## Description
Connect your **Bexio** account to any AI agent and orchestrate your business workflows, including CRM, accounting, and project management, through natural conversation.

### What you can do

- **Contact Management** — List, create, and retrieve detailed information for customers, suppliers, and partners.
- **Invoicing & Sales** — Query invoices, offers, and orders to stay on top of your sales pipeline and receivables.
- **Project Oversight** — List all business projects and monitor their status and progress.
- **Inventory & Items** — Access your product catalog and list items with pricing and stock metadata.
- **Team Collaboration** — Retrieve lists of users within your Bexio organization for better task coordination.

### How it works

1. Subscribe to this server
2. Enter your Bexio Personal Access Token
3. Start managing your business from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Small Business Owners** — quickly check invoice statuses and client details without manual dashboard navigation.
- **Accountants & Bookkeepers** — retrieve financial documents and contact data straight from their workflow.
- **Sales Reps** — verify offer details and create new contacts using natural language.


## Available Tools
- **create_contact**: Create a new contact
- **get_contact**: Get specific contact details
- **get_invoice**: Get specific invoice details
- **list_contacts**: List all contacts
- **list_invoices**: List all invoices
- **list_items**: List all products/items
- **list_offers**: List all offers
- **list_orders**: List all orders
- **list_projects**: List all projects
- **list_users**: List all Bexio users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bexio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in Bexio."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active projects: 'Q2 Marketing' (ID: proj_1), 'Website Overhaul' (ID: proj_2), and 'Customer Feedback Survey' (ID: proj_3).

---

**👤 You:**
> "Find the contact details for 'Acme Corp'."

**🤖 AI Agent:**
> I found one matching company: 'Acme Corporation' (ID: con_992). Their primary contact is John Smith, and their email is info@acme.com.

---

**👤 You:**
> "Show my last 5 invoices."

**🤖 AI Agent:**
> Retrieving invoices... Your 5 most recent invoices include 'INV-2024-001' (Status: Paid) and 'INV-2024-005' (Status: Draft). Would you like the details for any of these?


## Installation & Usage

To install and use the **Bexio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bexio](https://vinkius.com/mcp/bexio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
