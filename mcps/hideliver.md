# HiDeliver MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hideliver)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hideliver-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hideliver-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage email lists and marketing broadcasts via HiDeliver exactly from any AI agent.

## Description
Connect your **HiDeliver** broadcasting account to an AI agent to execute bulk email campaigns directly through conversations.

### What you can do

- **Client Lists** — Fetch stored customer addresses and list segments immediately to verify delivery rules
- **Audience Management** — Inspect or create subscriber leads straight from within conversational prompts
- **Campaign Insights** — Pull real-time delivery performance lists and broadcast statistics without entering the application

### How it works

1. Subscribe dynamically to this endpoint
2. Provide your core HiDeliver API key string
3. Engage your new marketing assistant via Cursor or Claude

### Who is this for?

- **Marketers** — add new segmented emails right into campaigns from your live discussions
- **Sales Representatives** — instantly check whether a key lead is verified safely inside your lists
- **Agency Developers** — construct custom dispatch rules dynamically testing mailing flows from the editor


## Available Tools
- **cancel_delivery**: Cancel a mapped delivery trace
- **create_delivery**: Log and schedule a fresh pickup delivery
- **get_account_balance**: Evaluate remaining tokens or cash thresholds
- **get_delivery**: Get parameters surrounding an explicit delivery
- **get_profile**: Get HiDeliver authenticated account logic
- **get_transaction**: Isolate a single API key transaction
- **list_deliveries**: Retrieve active or listed delivery requests
- **list_transactions**: Check global ledger events
- **update_delivery**: Adjust active route parameters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HiDeliver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Display all the actively loaded marketing lists right now."

**🤖 AI Agent:**
> Connecting... I found currently 3 deployed lists on your marketing gateway block. Let me show you the primary fields.

---

**👤 You:**
> "Fetch the underlying metadata and info associated with list ID 55102."

**🤖 AI Agent:**
> I received all configured limits concerning that base block. Notice its double opt-in flag stands enforced against cold drops.

---

**👤 You:**
> "Add the new email address 'lead@example.com' to list 55301."

**🤖 AI Agent:**
> Done! Subscriber successfully securely injected into list 55301 matching the platform parameters.


## Installation & Usage

To install and use the **HiDeliver** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hideliver](https://vinkius.com/mcp/hideliver)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
