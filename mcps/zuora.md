# Zuora MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zuora)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zuora-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zuora-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage subscriptions, billing accounts, and unified orders on Zuora — the leading monetization platform for the subscription economy.

## Description
Connect your **Zuora** account to any AI agent and manage your enterprise monetization infrastructure through natural conversation.

### What you can do

- **Subscription Lifecycle** — List all active and historical subscriptions for any account and retrieve deep details including rate plan charges
- **Billing Account Management** — Create new billing accounts, retrieve full account metadata, and update customer profiles directly from your agent
- **Unified Orders** — Create and manage complex Zuora Orders for subscriptions, renewals, or amendments using structured JSON payloads
- **Product Catalog Discovery** — Browse your entire billable product catalog and available rate plans to understand your monetization inventory
- **Invoice Auditing** — List and monitor all generated invoices for a specific account to track billing history and payment requirements
- **Billing Engine Simulation** — Preview subscription charges and generate quotes to verify billing logic before committing any changes
- **Deep Discovery** — Quickly find unique account, subscription, and order IDs required for automated revenue operations workflows

### How it works

1. Subscribe to this server
2. Enter your Zuora API Access Key ID, Secret Access Key, and REST Host
3. Start managing your subscription monetization through Claude, Cursor, or any MCP-compatible client

No more manual navigation through complex billing dashboards to verify a charge. Your AI agent becomes your monetization operations coordinator.

### Who is this for?

- **Revenue Operations (RevOps)** — monitor subscription lifecycles and audit order details through simple chat commands
- **Billing Analysts** — reconcile invoices and preview subscription charges without manual data entry
- **Finance Teams** — verify customer billing account metadata and monitor account standings through conversation
- **Developers** — test Zuora Order payloads and verify product catalog configurations rapidly


## Available Tools
- **create_account**: Create a new billing account
- **create_order**: Create a Zuora unified Order
- **get_account**: Get account details
- **get_invoices**: Get invoices for an account
- **get_order**: Get order details
- **get_subscription**: Get subscription details
- **list_products**: List product catalog
- **list_subscriptions**: List account subscriptions
- **preview_subscription**: Preview subscription charges
- **update_account**: Update account details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zuora** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active subscriptions for account ID 'acc-123'."

**🤖 AI Agent:**
> I found 2 active subscriptions for acc-123: 1. 'SaaS Premium' (No: S-00001, Status: Active), 2. 'API Add-on' (No: S-00002, Status: Active). Would you like to see the rate plan details for either of these?

---

**👤 You:**
> "Show me the last 3 invoices for 'Acme Corp'."

**🤖 AI Agent:**
> Retrieving invoices for Acme Corp (acc-456)... The last 3 invoices are: 1. INV-001 ($1,250.00, Status: Paid), 2. INV-002 ($1,250.00, Status: Posted), and 3. INV-003 ($1,250.00, Status: Posted). Would you like me to pull the PDF download link for any of these?

---

**👤 You:**
> "Preview the charges for subscription 'S-00001'."

**🤖 AI Agent:**
> Billing simulation for S-00001 complete. The projected charge for the next period (2026-04-01 to 2026-05-01) is $1,250.00 plus tax. No amendments were detected. Would you like me to generate a formal quote?


## Installation & Usage

To install and use the **Zuora** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zuora](https://vinkius.com/mcp/zuora)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
