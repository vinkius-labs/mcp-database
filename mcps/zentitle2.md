# Zentitle2 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zentitle2)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zentitle2-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zentitle2-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage software licenses and entitlements with a cloud platform that handles activation, metering, and feature gating for ISVs.

## Description
Connect your **Zentitle2** licensing account to any AI agent and simplify how you provision software, manage customer rights, and track activation codes through natural conversation.

### What you can do

- **Customer Management** — List and create customer records to organize your user base.
- **Entitlement Provisioning** — Grant and manage software rights (licenses) to specific customers for your products.
- **Activation Logic** — List and generate new activation codes to facilitate software deployment.
- **Product Catalog** — Browse your licensed products and features to understand your offering.
- **Management Overview** — Retrieve account metadata and monitor your licensing operations in real-time.

### How it works

1. Subscribe to this server
2. Enter your Zentitle2 Management API Key
3. Start managing your software licenses from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **License Administrators** — quickly provision new licenses and verify customer entitlements via simple AI queries.
- **Customer Support** — retrieve activation codes and check license status to resolve user issues instantly.
- **Product Operations** — monitor product distribution and customer adoption directly from the workspace.


## Available Tools
- **create_activation_code**: Generate a new activation code
- **create_customer**: Create a new customer in Zentitle2
- **create_entitlement**: Provision a new entitlement
- **get_activation_code_details**: Get details of an activation code
- **get_customer_details**: Get details of a specific customer
- **get_entitlement_details**: Get details of a specific entitlement
- **get_me**: Get management account information
- **list_activation_codes**: List activation codes
- **list_customers**: List Zentitle2 customers
- **list_entitlements**: List licensing entitlements
- **list_products**: List licensed products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zentitle2** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all customers registered in Zentitle2."

**🤖 AI Agent:**
> I've fetched your customer directory. You have 15 registered customers including 'Acme Corp', 'Tech Solutions Ltd', and 'Global Industries'. Would you like to check entitlements for any of them?

---

**👤 You:**
> "Create a new license (entitlement) for product 'P-100' for customer 'C-552'."

**🤖 AI Agent:**
> Provisioning successful! A new entitlement for product 'P-100' has been granted to customer 'C-552'. The entitlement ID is ENT-99023.

---

**👤 You:**
> "Generate an activation code for entitlement 'ENT-99023'."

**🤖 AI Agent:**
> Code generated! The activation code for entitlement 'ENT-99023' is: 'ABCD-1234-EFGH-5678'. You can now provide this to the customer.


## Installation & Usage

To install and use the **Zentitle2** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zentitle2](https://vinkius.com/mcp/zentitle2)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
