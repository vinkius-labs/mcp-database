# Drip MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/drip-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/drip-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/drip-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage subscribers, campaigns, and events in Drip via your AI Agent.

## Description
### What you can do
- Retrieve and list your subscribers, custom fields, and tags.
- Create or update subscribers with precise tags and custom attributes.
- Record custom events to trigger Drip workflows dynamically.
- Fetch live metrics from your single-email campaigns and workflows.

### How it works
1. Sign up for Drip and locate your API Token and Account ID.
2. Add those credentials here to authenticate the MCP server.
3. Chat with your AI Agent to orchestrate Drip marketing tasks.

### Who is this for?
Growth marketers, e-commerce managers, and developers who want an intelligent AI Agent to interact with their Drip CRM, update subscribers, and trigger custom events in real-time.


## Available Tools
- **apply_tag**: Apply a tag to a subscriber
- **create_or_update_subscriber**: Pass the email address and optionally any custom fields or tags.

Create or update a subscriber in Drip
- **delete_subscriber**: This action is irreversible.

Delete a subscriber from Drip permanently
- **fetch_subscriber**: Fetch a single subscriber by their ID or Email
- **list_broadcasts**: List all Single-Email Campaigns (Broadcasts)
- **list_campaigns**: List all Email Series Campaigns
- **list_custom_fields**: List all custom field identifiers
- **list_subscribers**: Use this to fetch all known contacts.

List all subscribers in the Drip account
- **list_tags**: List all Tags used in the account
- **list_workflows**: List all Workflows in Drip
- **record_event**: You can pass additional properties associated with the event.

Record a custom event for a subscriber in Drip
- **unsubscribe_subscriber**: Unsubscribe a subscriber from all mailings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Drip** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new Drip subscriber with the email 'leads@example.com' and tag them as 'VIP'."

**🤖 AI Agent:**
> The subscriber 'leads@example.com' has been successfully created and tagged as 'VIP'.

---

**👤 You:**
> "List all active workflows in my Drip account."

**🤖 AI Agent:**
> Here are the workflows currently available in your account: ...

---

**👤 You:**
> "Record a custom event called 'Signed Up' for user 'john@doe.com' in Drip."

**🤖 AI Agent:**
> The custom event 'Signed Up' has been recorded for 'john@doe.com' in Drip.


## Installation & Usage

To install and use the **Drip** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/drip-alternative](https://vinkius.com/mcp/drip-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
