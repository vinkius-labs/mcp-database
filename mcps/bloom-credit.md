# Bloom Credit MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bloom-credit)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bloom-credit-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bloom-credit-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Unified access to credit data and reporting via Bloom Credit — manage consumers, order reports, and monitor scores directly from any AI agent.

## Description
Connect your **Bloom Credit** account to any AI agent and orchestrate your credit data and reporting workflows through natural conversation.

### What you can do

- **Consumer Management** — Create and retrieve individual consumer profiles for credit analysis or reporting.
- **On-Demand Credit Pulls** — Order standardized credit reports and scores from all major bureaus (Equifax, Experian, TransUnion).
- **Report Deep Dives** — Retrieve detailed credit report data, including tradelines and payment histories.
- **Furnishment Oversight** — Monitor and list credit reporting furnishment accounts to ensure accurate data submission.
- **Organization Coordination** — Access and manage multiple organizations and account profile metadata.

### How it works

1. Subscribe to this server
2. Enter your Bloom Credit Client ID, Client Secret, and Environment
3. Start managing your credit operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fintech Founders** — quickly check consumer statuses and order reports without a custom frontend.
- **Lending Operations** — retrieve detailed credit data and scores straight from their workflow tools.
- **Compliance Teams** — monitor furnishment accounts and organization structures using natural language.


## Available Tools
- **create_consumer**: Create a new consumer profile
- **create_order**: Order credit data for a consumer
- **get_account_info**: Get authenticated account profile info
- **get_consumer**: Get specific consumer details
- **get_order**: Get specific order details
- **get_report_data**: Get detailed credit report data for an order
- **list_consumers**: List all consumers in the system
- **list_furnishments**: List credit reporting furnishment accounts
- **list_orders**: List all credit data orders
- **list_organizations**: List all accessible organizations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bloom Credit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all consumers registered in my account."

**🤖 AI Agent:**
> I've retrieved your consumers. You have 3 recent profiles: 'John Doe' (ID: con_1), 'Jane Smith' (ID: con_2), and 'Alice Brown' (ID: con_3).

---

**👤 You:**
> "Order a credit score for consumer con_1."

**🤖 AI Agent:**
> Triggering credit data order for 'John Doe'... Done! Order ID 'ord_99283' has been created. You can retrieve the score results once processed using `get_order`.

---

**👤 You:**
> "Show the report data for order ord_99283."

**🤖 AI Agent:**
> Retrieving data for order ord_99283... I found a FICO score of 720 and 5 active tradelines. Would you like a detailed summary of the payment history?


## Installation & Usage

To install and use the **Bloom Credit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bloom-credit](https://vinkius.com/mcp/bloom-credit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
