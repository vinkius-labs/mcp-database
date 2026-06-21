# Billplz MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/billplz)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/billplz-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/billplz-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage your payment collections via Billplz — list collections, bills, and transactions directly from any AI agent.

## Description
Connect your **Billplz** account to any AI agent and orchestrate your payment workflows through natural conversation.

### What you can do

- **Collection Management** — List, create, and inspect collections to organize your bills.
- **Bill Creation & Tracking** — Query, create, and delete individual bills and track payment statuses.
- **Transaction Oversight** — Retrieve detailed transactions for specific bills to reconcile payments.
- **Bank Account Auditing** — Check bank account details attached to collections.
- **FPX Insights** — List available FPX banks supported by the platform.

### How it works

1. Subscribe to this server
2. Enter your Billplz API Key and Environment (production or sandbox)
3. Start managing your payments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Merchants** — quickly check payment statuses without opening the Billplz dashboard.
- **Finance Teams** — audit collections and transaction histories using natural language.
- **Developers** — generate test bills and manage sandboxes directly from their editor.


## Available Tools
- **activate_collection**: Activate a collection
- **create_bill**: Create a new bill for collection
- **create_collection**: Create a new bill collection
- **deactivate_collection**: Deactivate a collection
- **delete_bill**: Delete an unpaid bill
- **get_bank_account**: Get bank account details for a collection
- **get_bill**: Get specific bill details
- **get_collection**: Get specific collection details
- **get_fpx_banks**: List supported FPX Banks
- **list_collections**: List all bill collections
- **list_transactions**: List transactions for a specific bill


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Billplz** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active collections."

**🤖 AI Agent:**
> I've retrieved your collections. You have 3 active collections: 'E-store Payments' (ID: col_1), 'Monthly Subs' (ID: col_2), and 'Donations' (ID: col_3).

---

**👤 You:**
> "Show the status of bill bill_99283."

**🤖 AI Agent:**
> The bill bill_99283 for RM 50.00 is currently in 'paid' status. It was paid via FPX on March 28th.

---

**👤 You:**
> "List the last 5 transactions for bill_99283."

**🤖 AI Agent:**
> Retrieving transactions... I found one successful payment transaction for bill_99283. Amount: RM 50.00, Payment Method: Maybank2u.


## Installation & Usage

To install and use the **Billplz** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/billplz](https://vinkius.com/mcp/billplz)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
