# Freshmarketer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freshmarketer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/freshmarketer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/freshmarketer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage marketing automation, sync contacts, and trigger email journeys via AI agents with Freshmarketer.

## Description
Connect your **Freshmarketer** account (part of the Freshsales Suite) to any AI agent to automate your marketing operations through the Model Context Protocol (MCP). Freshmarketer helps you engage your audience with personalized email campaigns and automated journeys. This MCP server enables you to manage your contact database, organize mailing lists, and trigger transactional emails directly through natural conversation.

### Key Features

- **Contact Management** — List all marketing contacts, retrieve detailed profiles, and create or update contacts instantly.
- **Audience Segmentation** — Access and list your configured mailing lists to understand how your audience is segmented.
- **Transactional Emails** — Trigger specific transactional campaigns to individual contacts directly from the chat interface.
- **Journey Insights** — Monitor your active and paused marketing automation journeys.
- **Event Tracking** — Post custom events to a contact's timeline to programmatically trigger specific automation flows.
- **Real-time Data Sync** — Keep your marketing data synchronized with your CRM seamlessly.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Freshmarketer Domain prefix and API Key (found in your Admin Settings)
3. Start managing your marketing campaigns from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Managers** — quickly check active lists and journeys without manual dashboard navigation.
- **Growth Engineers** — automate the posting of custom events to trigger specific customer journeys.
- **Sales Teams** — verify contact details and trigger personalized follow-up emails via simple AI commands.


## Available Tools
- **create_mailing_list**: Create new mailing list
- **check_account_status**: Verify API status
- **get_contact_details**: Get contact metadata
- **list_contacts**: List marketing contacts
- **list_custom_events**: List configured events
- **list_journeys**: List marketing journeys
- **list_mailing_lists**: List mailing lists
- **post_custom_event**: Trigger custom event
- **send_transactional_email**: Trigger an email
- **upsert_contact**: Create or update contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freshmarketer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my 5 most recent marketing contacts."

**🤖 AI Agent:**
> Retrieving contacts... I found 5 recent records, including 'john@example.com' (Subscribed) and 'jane@example.com' (Bounced). Would you like their full profiles?

---

**👤 You:**
> "Show me all active mailing lists in my account."

**🤖 AI Agent:**
> Fetching lists... You have 3 active mailing lists: 'Newsletter Subscribers', 'Beta Testers', and 'Churned Users'.

---

**👤 You:**
> "Trigger the 'Welcome Email' (Campaign ID: 123) for 'newuser@example.com'."

**🤖 AI Agent:**
> Email triggered! The transactional 'Welcome Email' has been successfully dispatched to newuser@example.com.


## Installation & Usage

To install and use the **Freshmarketer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freshmarketer](https://vinkius.com/mcp/freshmarketer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
