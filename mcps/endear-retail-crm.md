# Endear Retail CRM MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/endear-retail-crm)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/endear-retail-crm-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/endear-retail-crm-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to manage retail customers, track orders, and monitor clienteling notes via the Endear API.

## Description
Integrate **Endear**, the leading retail CRM and clienteling platform, directly into your AI workflow. Manage your customer profiles and purchase history, track clienteling notes and interactions, monitor product catalogs and team tasks, and oversee your retail operations using natural language.

### What you can do

- **Customer Oversight** — List and retrieve detailed profiles, email addresses, and total spend for all your retail customers.
- **Purchase Intelligence** — Monitor customer order history, resolving order numbers, amounts, and fulfillment statuses.
- **Clienteling Management** — Access and monitor customer notes and interactions, tracking tasks and follow-ups for your sales team.
- **Retail Auditing** — Retrieve high-level summaries of customer volume, order activity, and organizational retail health instantly.

### How it works

1. Connect the Endear integration to your AI assistant.
2. Authorize using your Endear API Key (found in your account settings).
3. Orchestrate your clienteling strategy and customer relations through intuitive conversation.

### Who is this for?

- **Retail Managers** — Quickly check customer spend and order statuses on the go.
- **Sales Associates** — Research customer notes and profile details via chat to personalize service.
- **Operations Teams** — Monitor task completion and organizational retail metadata instantly.


## Available Tools
- **get_endear_account_metadata**: Retrieve metadata and settings for your Endear account
- **get_customer_profile**: Get detailed profile and history for a specific customer
- **quick_retail_performance_audit**: Retrieve a high-level summary of customers, orders, and products
- **list_customer_clienteling_notes**: List all clienteling notes and interactions for a specific customer
- **list_customer_purchase_history**: List all orders and purchase history for a specific customer
- **list_retail_customers**: List all customers in your Endear CRM
- **list_retail_products**: List all products available in your retail catalog
- **list_clienteling_tasks**: List all clienteling and follow-up tasks
- **list_retail_team_members**: List all team members and sales associates in the organization
- **search_customers_by_name_or_email**: Search for customers using a name or email keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Endear Retail CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all customers with high total spend."

**🤖 AI Agent:**
> I've identified several high-value customers, including 'Alice Johnson' ($4,500 spent) and 'Robert Smith' ($3,200 spent). Both have recent purchase activity. Would you like to see the notes for Alice Johnson?

---

**👤 You:**
> "Show me the last 5 orders for customer ID 'CUST-12345'."

**🤖 AI Agent:**
> Customer ID 'CUST-12345' (John Doe) has 5 recent orders, including '#ORD-9988' ($150, Fulfilled) and '#ORD-9977' ($240, Shipped). Should I pull the items included in the most recent order?

---

**👤 You:**
> "Search for customers matching 'Sarah'."

**🤖 AI Agent:**
> I've found 3 customers matching 'Sarah': 'Sarah Miller', 'Sarah Connor', and 'Sarah Williams'. All are in the 'Loyalty Member' segment. Would you like the profile details for Sarah Miller?


## Installation & Usage

To install and use the **Endear Retail CRM** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/endear-retail-crm](https://vinkius.com/mcp/endear-retail-crm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
