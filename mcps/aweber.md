# AWeber MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aweber)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/aweber-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/aweber-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage subscribers, mailing lists, and email campaigns via AWeber — orchestrate newsletters natively via AI.

## Description
Connect your **AWeber** account to any AI agent and manage your entire email marketing ecosystem through natural conversation.

### What you can do

- **Audience Management** — Create, search, and update subscriber profiles across all your mailing lists
- **Campaign Orchestration** — List and audit automated campaigns and broadcasts to ensure your messaging is on track
- **List Coordination** — Retrieve and manage your organizational mailing lists and their respective settings
- **Subscriber Auditing** — Deeply inspect individual subscriber metadata, tags, and engagement history

### How it works

1. Subscribe to this server
2. Enter your AWeber Access Token
3. Start managing your email marketing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — instantly retrieve list statuses, check campaign progress, and update subscriber tags without the dashboard
- **Content Strategists** — coordinate broadcasts and audit audience segments directly from their planning workspace
- **Automation Engineers** — programmatically manage subscriber flows and list metadata through natural language


## Available Tools
- **add_subscriber**: Add a new subscriber to a list
- **find_subscriber**: Find a subscriber by email across the entire account
- **get_account_check**: Verify AWeber connection and list available accounts
- **get_account**: Get details for a specific AWeber account
- **get_broadcast_stats**: Get engagement statistics for a specific broadcast
- **get_list**: Get details for a specific mailing list
- **list_accounts**: List all accounts associated with the authenticated user
- **list_broadcasts**: List all sent or scheduled broadcasts
- **list_campaigns**: List automated campaigns
- **list_lists**: List all mailing lists for an account
- **list_subscribers**: List subscribers for a specific list
- **update_subscriber**: Update an existing subscriber details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWeber** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all mailing lists in my AWeber account."

**🤖 AI Agent:**
> I've retrieved your mailing lists. You currently have 3 active lists: 'Weekly Newsletter' (ID: 12345), 'Product Updates', and 'Internal Team'. Which list would you like to inspect for subscriber data?

---

**👤 You:**
> "Find the subscriber with email '[email protected]'."

**🤖 AI Agent:**
> I found the subscriber '[email protected]'. They are currently 'subscribed' to your 'Weekly Newsletter' list and have been tagged with 'VIP' and 'Early-Adopter'. Shall I update any of their tags?

---

**👤 You:**
> "Show the statistics for the latest broadcast."

**🤖 AI Agent:**
> Retrieving stats... Your latest broadcast 'July Promo' reached 1,200 recipients with a 24% open rate and a 5% click-through rate. There were 2 unsubscribes reported. Would you like a detailed breakdown?


## Installation & Usage

To install and use the **AWeber** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aweber](https://vinkius.com/mcp/aweber)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
