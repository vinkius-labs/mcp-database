# Wayfront MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wayfront)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wayfront-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wayfront-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Manage your parking operations with digital permits, enforcement tracking, and revenue analytics for parking facility operators.

## Description
Connect your **Wayfront** client portal (SPP) to any AI agent and streamline your service delivery workflows through natural conversation.

### What you can do

- **Client Management** — List all clients, retrieve detailed profile metadata, and create new client accounts programmatically
- **Order Tracking** — Query active orders, check their status, and update order progress directly from your agent
- **Billing & Invoices** — Monitor generated invoices to stay on top of your accounts receivable
- **Service Catalog** — List the services and products available in your portal
- **Ticketing** — Retrieve support tickets to monitor client communication and satisfaction
- **Team Overview** — List teams and departments to understand your internal structure

### How it works

1. Subscribe to this server
2. Enter your Wayfront Subdomain and API Key
3. Start managing your client portal resources from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **create_client**: Create a new client
- **get_client**: Get details for a specific client
- **get_order**: Get details for a specific order
- **list_clients**: List Wayfront clients
- **list_invoices**: List all Wayfront invoices
- **list_orders**: List Wayfront orders
- **list_services**: List available services
- **list_teams**: List organizational teams
- **list_tickets**: List support tickets
- **update_order**: Update an existing order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wayfront** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active orders in my Wayfront portal."

**🤖 AI Agent:**
> I've retrieved your orders. You have 8 active orders, including 'Order #1001' (Status: In Progress) and 'Order #1002' (Status: Pending Review). Which one would you like more details on?

---

**👤 You:**
> "Find support tickets from last week."

**🤖 AI Agent:**
> Analyzing tickets... I found 5 tickets from last week. Notable ones include 'Issue with billing' from client Alice and 'Login problem' from client Bob. Would you like the full text of Alice's ticket?

---

**👤 You:**
> "Get details for client '123'."

**🤖 AI Agent:**
> Client '123' is Marcus R. (marcus@example.com). They have 3 active orders and have been a client since Jan 2024. Their primary contact is through the portal dashboard.


## Installation & Usage

To install and use the **Wayfront** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wayfront](https://vinkius.com/mcp/wayfront)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
