# Clientjoy MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clientjoy-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clientjoy-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clientjoy-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Manage your entire client lifecycle from proposals and contracts through invoicing and payments in one streamlined platform.

## Description
Connect your **Clientjoy** CRM and billing account to any AI agent and simplify how you coordinate your sales pipeline, client directory, and invoicing through natural conversation.

### What you can do

- **Lead Management** — List and query potential sales leads, and create new prospect profiles programmatically via AI.
- **Client CRM** — List all customer organizations and retrieve detailed metadata, contact info, and transaction histories.
- **Billing Oversight** — List and monitor generated invoices and their payment status to keep your finances organized.
- **Sales Proposals** — Query your catalog of sent and drafted proposals to track your business development efforts.
- **Service Catalog** — List available products and services defined in your account to verify pricing and offerings.
- **Lifecycle Control** — Manage the entire journey from lead to paid customer directly from Claude, Cursor, or any MCP client.

### How it works

1. Subscribe to this server
2. Enter your Clientjoy API Token (found in your account settings under API)
3. Start managing your business ecosystem from your favorite AI assistant

### Who is this for?

- **Agency Owners & Freelancers** — quickly retrieve client details and check invoice statuses via simple AI commands.
- **Sales & BD Teams** — monitor lead progress and verify proposal availability directly from the workspace.
- **Ops & Finance Leads** — track received payments and manage the service directory via the AI assistant.


## Available Tools
- **create_new_lead**: Register a new lead
- **get_customer_details**: Get details for a specific customer
- **list_customers**: List Clientjoy customers
- **list_billing_invoices**: List invoices
- **list_service_items**: List items and services
- **list_leads**: List Clientjoy leads
- **list_sales_proposals**: List proposals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clientjoy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active leads in my Clientjoy account."

**🤖 AI Agent:**
> I've retrieved your sales pipeline. You have 3 active leads: 'Acme Corp Expansion', 'New Retail Project', and 'Tech Solutions Lead'. Which one would you like more details on?

---

**👤 You:**
> "Show me the details for customer 'John Miller' (ID: 10293)."

**🤖 AI Agent:**
> Fetching profile... John Miller is a 'VIP Client' from 'Miller Industries'. He has 2 paid invoices and 1 active proposal. Would you like to see his full transaction history?

---

**👤 You:**
> "Are there any overdue invoices?"

**🤖 AI Agent:**
> Checking billing... Yes, you have 1 overdue invoice: #INV-88231 ($450.00) from 'Global Logistics'. It was due 5 days ago. Shall I retrieve the contact info for follow-up?


## Installation & Usage

To install and use the **Clientjoy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clientjoy-alternative](https://vinkius.com/mcp/clientjoy-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
