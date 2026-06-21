# Acelle Mail MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/acelle-mail)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/acelle-mail-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/acelle-mail-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Launch email campaigns, grow subscriber lists, and track open rates with a self-hosted email marketing platform built for scale.

## Description
Connect your **Acelle Mail** self-hosted or cloud account to any AI agent and simplify how you manage your mailing lists, subscriber data, and email campaigns through natural conversation.

### What you can do

- **List Management** — List all your mailing lists, create new directories, and retrieve detailed configuration metadata.
- **Subscriber Control** — List and query subscribers for specific lists, and add new members programmatically via AI.
- **Campaign Monitoring** — List active and past email campaigns and retrieve detailed status and metadata for each outreach.
- **Audience Oversight** — Fetch list details and verify subscriber counts to manage your marketing reach.
- **Automation Readiness** — Manage your subscriber lifecycle and list organization directly from Claude, Cursor, or any MCP client.

### How it works

1. Subscribe to this server
2. Enter your Acelle Mail API Token and Base URL
3. Start managing your email marketing machine from your favorite AI assistant

### Who is this for?

- **Marketing Managers** — quickly retrieve subscriber counts and campaign metadata via simple AI commands.
- **Customer Success Teams** — add new subscribers and verify list membership directly from the workspace.
- **Email Outreach Specialists** — monitor campaign statuses and manage audience segments via the AI assistant.


## Available Tools
- **add_acelle_subscriber**: Add a subscriber
- **create_acelle_list**: Create a new list
- **get_acelle_campaign**: Get campaign details
- **get_acelle_list**: Get list details
- **list_acelle_campaigns**: List all campaigns
- **list_acelle_lists**: List all mailing lists
- **list_acelle_subscribers**: List subscribers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Acelle Mail** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my mailing lists in Acelle Mail."

**🤖 AI Agent:**
> I've retrieved your mailing lists. You have 3 active directories: 'Main Newsletter', 'Beta Testers', and 'Old Customers'. Which one would you like to see subscribers for?

---

**👤 You:**
> "Add 'john.doe@example.com' to the 'Main Newsletter' list (UID: 10293)."

**🤖 AI Agent:**
> Subscriber added! I've registered john.doe@example.com in the 'Main Newsletter' list. He is now active and ready to receive your upcoming campaigns.

---

**👤 You:**
> "Show me the status of my latest email campaign."

**🤖 AI Agent:**
> I've fetched your campaigns. The 'November Product Update' (UID: camp_88231) is currently 'Sending'. It has already reached 85% of its recipients with an open rate of 12%.


## Installation & Usage

To install and use the **Acelle Mail** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/acelle-mail](https://vinkius.com/mcp/acelle-mail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
