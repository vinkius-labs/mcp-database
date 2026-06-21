# Fresha MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fresha)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fresha-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fresha-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Query and analyze your Fresha salon data — list appointments, clients, locations, services, staff, and sales transactions directly from any AI agent.

## Description
Connect your **Fresha** workspace to any AI agent and gain deep insights into your salon or spa operations through natural conversation using OData-powered queries.

### What you can do

- **Appointments & Bookings** — List scheduled appointments and detailed appointment services to track your calendar
- **Client Management** — Retrieve customer profiles, contact details, and saved history from your workspace
- **Sales & Financials** — Query sales transactions, invoices, and individual line items generated at checkout
- **Business Structure** — Inspect physical locations, service menus, and staff/professional profiles

### How it works

1. Subscribe to this server
2. Enter your Fresha Data Connector Token
3. Start querying your salon data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Salon & Spa Owners** — instantly analyze booking trends, check daily sales, and monitor staff schedules without manual exports
- **Operations Managers** — track client retention, service performance, and multi-location metrics through simple questions
- **Data Analysts** — run advanced OData filters and queries to build custom reports on appointments and revenue


## Available Tools
- **list_appointment_services**: List Fresha appointment services via OData
- **list_appointments**: List Fresha appointments via OData
- **list_clients**: List Fresha clients via OData
- **list_inventory**: List Fresha inventory via OData
- **list_locations**: List Fresha locations via OData
- **list_products**: List Fresha products via OData
- **list_reviews**: List Fresha reviews via OData
- **list_sale_items**: List Fresha sale items via OData
- **list_sales**: List Fresha sales via OData
- **list_services**: List Fresha services via OData
- **list_staff**: List Fresha staff via OData


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fresha** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 completed appointments with client details."

**🤖 AI Agent:**
> I will query `list_appointments` with `$filter=Status eq 'Completed'`, `$orderby=StartTime desc`, `$top=5`, and `$expand=Client`. Here are the 5 most recent completed bookings, including appointments for Sarah M. (Haircut) and John D. (Massage).

---

**👤 You:**
> "Show me our physical business locations and active staff members."

**🤖 AI Agent:**
> Retrieving data... Using `list_locations` and `list_staff`, I found 2 active locations ('Downtown Salon' and 'Westside Spa') and 8 registered staff members. Would you like to see which staff members are assigned to a specific location?

---

**👤 You:**
> "Find all sales transactions from today."

**🤖 AI Agent:**
> Running the query on `list_sales` with a filter for today's date... I found 12 sales transactions totaling $1,450. The largest transaction was Invoice #1042 for $220. Would you like me to list the individual items for that invoice using `list_sale_items`?


## Installation & Usage

To install and use the **Fresha** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fresha](https://vinkius.com/mcp/fresha)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
