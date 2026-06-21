# Brokermint MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brokermint)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/brokermint-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/brokermint-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Manage real estate back-office via Brokermint — track transactions, contacts, and commissions directly from any AI agent.

## Description
Connect your **Brokermint** account to any AI agent and orchestrate your real estate back-office, transaction management, and commission tracking through natural conversation.

### What you can do

- **Transaction Oversight** — List all real estate deals, retrieve detailed metadata, and update statuses directly from your workspace.
- **Contact Management** — List and create contacts for buyers, sellers, and other participants in your transactions.
- **Commission Tracking** — Retrieve detailed commission structures and payouts associated with specific deals.
- **Team Coordination** — Access your directory of agents and users managed within the platform.
- **Account Insights** — Retrieve core account and site information straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Brokermint API Key and Account ID
3. Start managing your real estate operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Real Estate Brokers & Admins** — quickly check transaction statuses and commission details without manual dashboard work.
- **Transaction Coordinators** — retrieve and update deal information straight from their editor.
- **Agents** — monitor their own transactions and contact lists using natural language.


## Available Tools
- **create_contact**: Create a new contact
- **create_transaction**: Create a new real estate transaction
- **get_account_info**: Retrieve core account information
- **get_contact**: Get details of a specific contact
- **get_transaction**: Get details of a specific transaction
- **list_commissions**: List commissions for a specific transaction
- **list_contacts**: List all contacts (buyers, sellers, etc)
- **list_transactions**: List all real estate transactions
- **list_users**: List all users/agents in the account
- **update_transaction**: Update an existing transaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brokermint** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 real estate transactions in Brokermint."

**🤖 AI Agent:**
> I've retrieved your transactions. You have 5 recent deals, including '742 Evergreen Terrace' (Status: Listing) and '123 Maple St' (Status: Pending).

---

**👤 You:**
> "Show the commission structure for transaction tr_99283."

**🤖 AI Agent:**
> Retrieving commissions for tr_99283... The total commission is $15,000, with a 3% split for the listing agent ($7,500) and 3% for the buyer's agent ($7,500).

---

**👤 You:**
> "Create a new contact named John Doe with email john@example.com."

**🤖 AI Agent:**
> Contact 'John Doe' has been successfully created in your Brokermint account with ID cont_123.


## Installation & Usage

To install and use the **Brokermint** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brokermint](https://vinkius.com/mcp/brokermint)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
