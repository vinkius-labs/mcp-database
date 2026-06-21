# NachoNacho MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nachonacho)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nachonacho-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nachonacho-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Optimize your SaaS spending with virtual cards, subscription tracking, and vendor management that reveals hidden savings.

## Description
Connect your **NachoNacho** account to any AI agent and manage SaaS spend through natural conversation.

### What you can do

- **Virtual Cards** — Create, list, update, freeze, and unfreeze cards
- **Transactions** — Browse and inspect card transactions
- **Balances** — Monitor account funds
- **Subscriptions** — List and inspect managed SaaS subscriptions

### Who is this for?

- **Finance Teams** — control SaaS spend with virtual cards
- **Procurement** — manage vendor subscriptions
- **Startups** — track subscription costs


## Available Tools
- **check_nachonacho_status**: Verify connectivity
- **create_card**: Create a virtual card
- **freeze_card**: Freeze a card
- **get_card**: Get card details
- **get_subscription**: Get subscription details
- **get_transaction**: Get transaction details
- **list_balances**: List balances
- **list_cards**: List virtual cards
- **list_subscriptions**: List subscriptions
- **list_transactions**: List transactions
- **unfreeze_card**: Unfreeze a card
- **update_card**: Update a card


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NachoNacho** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all virtual cards and their spend."

**🤖 AI Agent:**
> Cards: 5. 1) 'Slack' ($50 limit, $42 spent). 2) 'Notion' ($20 limit, $15 spent). 3) 'Figma' ($45 limit, $45 spent ⚠️). 4) 'AWS' ($500 limit, $320 spent). 5) 'GitHub' ($25 limit, Frozen 🧊). Total spend: $422.

---

**👤 You:**
> "Create a virtual card for a new Notion subscription with $25 limit."

**🤖 AI Agent:**
> Card created ✅. Name: Notion Pro. Limit: $25/month. Card Number: ****4892. Status: Active.

---

**👤 You:**
> "Freeze the Figma card and show account balance."

**🤖 AI Agent:**
> Figma card frozen 🧊. Balance: $1,250.00 available. Active cards: 3. Frozen: 2.


## Installation & Usage

To install and use the **NachoNacho** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nachonacho](https://vinkius.com/mcp/nachonacho)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
