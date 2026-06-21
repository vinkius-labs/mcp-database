# Tithe.ly MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tithely)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tithely-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tithely-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [payment-processing](../categories/payment-processing.md)

Manage church giving and nonprofit fundraising via Tithe.ly — list organizations, manage payment categories, and process transactions directly from your AI agent.

## Description
Connect your **Tithe.ly** account to any AI agent to streamline your ministry's financial operations and donor management through natural conversation.

### What you can do

- **Organization Management** — Search for and retrieve details for your organizations or specific account owners.
- **Payment Categories** — List, create, and update giving types, shop items, or cafe categories to organize your revenue streams.
- **Transaction Processing** — Create new transactions and manage financial records seamlessly.
- **Automated Communication** — Send receipts and update emails to donors using specific templates directly from the agent.
- **Account Insights** — Authenticate and retrieve account details to ensure your API credentials and permissions are correctly configured.

### How it works

1. Subscribe to this server
2. Enter your Tithe.ly API ID and API Token
3. Start managing your church or nonprofit finances from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Church Administrators** — quickly update giving categories and check organization details without manual dashboard navigation.
- **Nonprofit Finance Teams** — automate the creation of transactions and sending of receipts to donors.
- **Ministry Leads** — get instant reports on organization owners and active payment types.


## Available Tools
- **create_payment_category**: Create a new payment category
- **create_transaction**: Process a new transaction
- **login**: Authenticate and retrieve account details
- **list_organization_owners**: Search for organization owners
- **list_organizations**: Search for and retrieve organization details
- **list_payment_categories**: List or search payment categories
- **send_email**: API credentials must have admin permissions or belong to the recipient.

Send emails (e.g., receipts) to recipients
- **update_payment_category**: Update an existing payment category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tithe.ly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all organizations I manage on Tithe.ly."

**🤖 AI Agent:**
> I've retrieved your organizations. You have access to 'Grace Community Church' (ID: 77482) and 'Hope Outreach' (ID: 99231). Which one would you like to manage?

---

**👤 You:**
> "Create a new giving category called 'Youth Ministry' for organization 77482."

**🤖 AI Agent:**
> Successfully created the 'Youth Ministry' category (Type: giving_type) for organization 77482. It is now active and ready to receive donations.

---

**👤 You:**
> "Send a receipt for transaction 55021 to donor@example.com."

**🤖 AI Agent:**
> The receipt for transaction 55021 has been queued and sent to donor@example.com using the official receipt template.


## Installation & Usage

To install and use the **Tithe.ly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tithely](https://vinkius.com/mcp/tithely)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
